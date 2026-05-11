# RapidGO v1.9.0 Release Notes
**Release Date:** May 12th, 2026

## New Functionality

### Freight Allocation now respected
RapidGO now distributes Miscellaneous charges (e.g., freight) proportionally across receiver line items when posting to Counterpoint.

Allocation is based on the setting configured on the misc charge.

#### Example

- **Purchase Request:** 10 items totaling $1,000 + $100 freight
- Each item receives $10 freight allocation (1/10th)

If only 5 items are received:

- Total freight applied = $50
- Distributed across the 5 received items

#### Required Settings

When the settings below are enabled, Misc charges cost will be proportionally distributed across all receiver lines:

- **Use Misc Charge 1** = Checked
- **Include in Cost** = Checked
- **Allocate By** = Cost

Settings are sourced from Purchasing Control.

See:  
http://ncrcounterpointhelp.com/#3_back_office/purchasing/allocate_miscellaneous_charges.htm?Highlight=allocate%20misc

<br>

### Transfer To / Transfer From Workgroup Selection
In previous versions of RapidGO, users were unable to select their currently signed-in workgroup as a **Transfer To** location.

With this version of RapidGO, users can now select any location in either the **Transfer To** or **Transfer From** locations.

<br>

### Changing Receiving Header Information
RapidGO now allows users to edit receiver header information directly within the application.

Users can now modify:

#### Header Fields
- `REF`
- `COMMNT_1`
- `COMMNT_2`
- `COMMNT_3`

#### Line Fields
- `COMMNT_1`
- `COMMNT_2`
- `COMMNT_3`

This enhancement provides greater flexibility when updating receiving information without needing to return to CounterPoint.

#### API Information
- **Endpoint:** `Receivings`
- **Method:** `POST`

<br>

### Modifying Receiving Line Comments
Users can now edit receiver line comments directly in RapidGO.

This allows warehouse and receiving staff to:
- Update line-specific notes during the receiving process
- Correct or add additional receiving details
- Maintain more accurate documentation on individual receiver lines

These updates are now synchronized as part of the receiving workflow.

<br>

### Linking Barcodes
RapidGO now supports linking new barcodes directly to item units within the application.
This enhancement improves efficiency when onboarding new inventory and managing alternate unit barcodes.
## Linking New Barcodes in RapidGO

RapidGO now allows users to link new barcodes directly to items and units during the receiving process.

### Linking a Barcode

When scanning a barcode that does not currently exist, RapidGO will prompt the user to link the barcode to an item.
<img width="421" height="859" alt="image" src="https://github.com/user-attachments/assets/5f63b9ed-deef-41dc-9c3a-9d9421b9ed2a" />

After confirming, the barcode linking screen will open.
<img width="426" height="517" alt="image" src="https://github.com/user-attachments/assets/e5fb2ed8-a88c-4b3f-8446-8261e9b1ef77" />

Users can:
- Select an item from the receiver line list
- Or manually enter an item number

If the entered item exists on the receiver, the associated unit information will automatically load.
<img width="456" height="592" alt="image" src="https://github.com/user-attachments/assets/6dfe4a29-bb32-4c97-b26a-12f6e981c86a" />

<img width="457" height="535" alt="image" src="https://github.com/user-attachments/assets/9448e9db-fedf-4d13-8603-5d7acb170c23" />

If the item is not found on the receiver line, no unit information will be available.
<img width="451" height="541" alt="image" src="https://github.com/user-attachments/assets/2dc9a5e7-f697-4bdd-be4e-6de5d764b98f" />

Once a valid item is selected, users can choose the appropriate unit to associate with the barcode.
<img width="435" height="576" alt="image" src="https://github.com/user-attachments/assets/7365db92-1336-4a4e-be05-5fbf7def06de" />

Press **Link Barcode** to save the barcode association.
<img width="442" height="515" alt="image" src="https://github.com/user-attachments/assets/ab57dcfe-0ff7-405a-9e1c-f74eacba3382" />

<img width="427" height="544" alt="image" src="https://github.com/user-attachments/assets/9927bace-cb8a-4353-aa85-7ba5601ebcd6" />


After linking the barcode, RapidGO will automatically apply the scanned quantity to the selected item and unit.
<img width="438" height="550" alt="image" src="https://github.com/user-attachments/assets/41d5fad6-407e-46ac-9ffa-51f44d497888" />

<img width="461" height="667" alt="image" src="https://github.com/user-attachments/assets/90dbcf72-650a-45f5-ad60-c70d3014577b" />

The receiver line will then reflect the updated quantity using the newly linked barcode and unit.
<img width="446" height="705" alt="image" src="https://github.com/user-attachments/assets/8da5f60e-6586-4664-9f07-880bfc60d3a3" />

### Additional Notes

- Sliding downward on the barcode linking screen will cancel the form without saving changes.
<img width="438" height="817" alt="image" src="https://github.com/user-attachments/assets/a77e79f8-be2a-403d-865b-fdf1c4e966d3" />

- Newly linked barcodes become available in both CounterPoint and RapidGO.
<img width="983" height="422" alt="image" src="https://github.com/user-attachments/assets/9ed781cb-14f4-4988-a5d8-6cda80ca163e" />

<img width="1235" height="138" alt="image" src="https://github.com/user-attachments/assets/0275698d-531c-4939-b4e7-ea1ac0616a90" />


> **NOTE:** Other RapidGO devices must refresh their database to download newly linked barcodes.  
> Navigate to:  
> **Settings → Refresh Database**

![Refresh Database](image)

---

## Bug Fixes and Performance Enhancements


### Slow "Get Items" and Gridded Cell Cutoff
- Fixed an issue where gridded cells were cut off; users can now scroll to view all cells.
- Resolved app freezing and crashing related to slow performance.

### PO Comments and Selectable Units in Quantity Window
- PO line comments are now carried over to RapidGO.
- Removed non-selectable units from the quantity window.
