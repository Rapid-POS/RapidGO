# RapidGO v1.10.00 Release Notes

**Release Date:** 11/16/2026

_This release adds a faster way to update bins from Item Lookup, makes sure documents sent from Line Busting and Item List always reach Counterpoint, and shows progress while data syncs after login._

## New Features & Improvements

### Open bins on scan

You can now have RapidGO open the bin editor as soon as you scan an item in Item Lookup, so you can update bin locations without extra taps.

- Turn on the new Open bins on scan setting on the Settings page, under Item Lookup. It only applies to the device where you turn it on.
- When it's on, scanning an item opens the Change Min/Max/Bin screen with Min qty and Max qty hidden, so you only edit Bin-1 to Bin-4.
- Tapping Done saves the bins to the server and updates them on the item's Inventory tab for the current location. A progress indicator shows while the save runs.
- If the save fails or you cancel, nothing changes on the Inventory tab.
- When the setting is off, scanning works the same as before.

### Progress while data syncs after login

The message you see while data syncs after login now names the step that's running, for example "Syncing item changes (2 of 5)...". Before, it showed one message that never changed.

## Bug Fixes

### Documents sent from Line Busting and Item List now always reach Counterpoint

We removed the "Auto create" slider from the Line Busting and Item List screens. RapidGO now always creates the document in Counterpoint when you send it.

- Before, sending with the slider off gave you a document number in RapidGO that didn't exist in Counterpoint.
- RapidGO ignores any slider setting saved on a device by an earlier version.
