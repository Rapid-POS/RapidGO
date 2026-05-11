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
- Reference numbers
- Receiver comments
- Additional header-level information associated with the receiver

This enhancement provides greater flexibility when updating receiving information without needing to return to CounterPoint.

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

![Scan Non-Existing Barcode](image)

After confirming, the barcode linking screen will open.

![Barcode Linking Screen](image)

Users can:
- Select an item from the receiver line list
- Or manually enter an item number

If the entered item exists on the receiver, the associated unit information will automatically load.

![Selecting an Item](image)

If the item is not found on the receiver line, no unit information will be available.

![Item Not Found on Receiver](image)

Once a valid item is selected, users can choose the appropriate unit to associate with the barcode.

![Selecting Unit](image)

Press **Link Barcode** to save the barcode association.

![Link Barcode Button](image)

After linking the barcode, RapidGO will automatically apply the scanned quantity to the selected item and unit.

![Quantity Automatically Applied](image)

The receiver line will then reflect the updated quantity using the newly linked barcode and unit.

![Updated Receiver Quantity](image)

### Additional Notes

- Sliding downward on the barcode linking screen will cancel the form without saving changes.
- Newly linked barcodes become available in both CounterPoint and RapidGO.

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
