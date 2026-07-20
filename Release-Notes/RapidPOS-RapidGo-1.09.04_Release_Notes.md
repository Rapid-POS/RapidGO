# RapidGO 1.09.04 Release Notes
**Release Date:** July 22, 2026

_Inventory adjustment quantity-entry fixes and a safeguard against duplicate-looking receivings._

## New Features & Improvements

### Clearer On-Hand Adjustment Label
The "Reset On-Hand" action in Item Adjustment is now labeled "Set On-Hand Qty" to better describe what it does.

## Bug Fixes

### Receiving Number Protection
The Receiving # and Vendor # fields are now locked and can no longer be edited by hand after opening a previously saved receiving or a vendor-based receiving.

* This closes off the only known way a receiving could be sent in a way that looks like a duplicate.

### Inventory Adjustment Quantity Entry
Entering 0 as an adjustment quantity now holds correctly instead of clearing back to blank, so Reset On-Hand adjustments post the correct on-hand quantity.

* Increase and Decrease adjustments now block submission when the quantity is zero, showing "Quantity must be greater than zero" instead of sending a no-op adjustment.
* Fixed two crashes in the quantity field: entering a lone zero and moving to the next field, and typing a decimal point on the numeric keyboard, no longer close the app unexpectedly.

### Gridded Item Quantity Entry
Scanning a barcode tied to one grid cell of a gridded item (e.g. a color/size combination) now lets you enter the quantity directly instead of leaving it locked at the default of 1.

* The app no longer loses track of the item's other grid cells after this kind of scan.
* The cell-selection popup now displays full-screen with all rows instead of appearing empty or cut off.
* The popup now reliably reopens for the next scan or after changing the adjustment type, without needing to leave and reopen the page.
