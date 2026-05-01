# RapidGo v1.9.0 Release Notes

**Release Date:** May 4th, 2026

---

##  New Functionality
### Freight Allocation now respected

RapidGO now distributes **Miscellaneous charges (e.g., freight)** proportionally across receiver lines items when posting to Counterpoint.

* Allocation is based on the the setting configured on the misc charge.

**Example:**

* Purchase Request: 10 items totaling $1,000 + $100 freight
* Each item receives **$10 freight allocation** (1/10th)
* If only 5 items are received:

  * Total freight applied = **$50**
  * Distributed across the 5 received items

### Required Settings

When the settings below are enabled, **Misc charges cost will be proportionally distributed across all receiver lines**:

* **Use Misc Charge 1** = Checked
* **Include in Cost** = Checked
* **Allocate By** = Cost

*Settings are sourced from Purchasing Control.*

See http://ncrcounterpointhelp.com/#3_back_office/purchasing/allocate_miscellaneous_charges.htm?Highlight=allocate%20misc

---

##  Bug Fixes and Performance Enhancements

### Slow "Get Items" and Gridded Cell Cutoff
- Fixed an issue where gridded cells were cut off; users can now scroll to view all cells.
- Resolved app freezing and crashing related to slow performance.

### PO Comments and Selectable Units in Quantity Window
- PO line comments are now carried over to RapidGo.
- Removed non-selectable units from the quantity window.
