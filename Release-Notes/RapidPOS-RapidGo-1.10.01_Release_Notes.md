# RapidGO v1.10.01 Release Notes

**Release Date:** November 24, 2026

_This release fixes three issues in Transfer Out and Receiving._

## Bug Fixes

### Transfer Out keeps the unit you pick when scanning

When you scanned an item on a Transfer Out and picked a unit like a 48-count case, the transfer saved the item's stocking unit (often EACH) instead. Transfers now save the unit you picked on the device, so the quantity in Counterpoint matches what you pulled. Items added without scanning a barcode work the same as before.

### Linking a barcode during receiving no longer closes the app

RapidGO closed if linking an unknown barcode to a receiver line didn't go through. Now the app shows an error message and keeps you on the screen so you can try the link again.

### Sending a second Transfer Out from the same screen

After you sent one Transfer Out, sending another without leaving the screen showed "From Location and To Location are required," even though both locations were filled in. You can now send several transfers in a row without re-selecting the From Location.
