# RapidGO v1.09.07 Release Notes - Coming Soon
**Release Date:** September 7, 2026

_Fixes a duplicate-receiver bug on retried receiving submissions, Receiving incorrectly blocking stocked items, a Transfer Out data issue, and an app freeze on certain warning messages._

## Bug Fixes

### Receiving no longer creates a duplicate receiver after a network error
If submitting a receiving failed because of a network error, resending it could create a second, duplicate receiver against the same purchase order or vendor instead of one.

- Retrying a receiving submission after a network error no longer creates a duplicate receiver.
- If a submission fails this way, the app now checks whether it actually went through. If it did, you're shown the real receiver number it created and the screen is reset, instead of being left ready to send the same receiving again.
- This protection now also covers receivings started from a vendor lookup, not just receivings tied to a purchase order.

### Receiving no longer wrongly blocks items as "Not Stocked"
Receiving could show "Item Not Stocked at Location" and refuse to receive an item that was genuinely stocked there, because the device's data hadn't fully refreshed since the last time you logged in.

- Logging in now always pulls the latest item and inventory information before you can start working, instead of relying on a slower background update.
- If Receiving still can't find an item locally, it now checks with the server before blocking it, and only shows "Not Stocked" if the server agrees. If there's no connection to check, it tells you to check your connection instead of wrongly saying the item isn't stocked.
- Logging out, or getting signed out automatically after sitting idle, now fully signs you out. Reopening the app takes you back to the Login screen instead of possibly resuming you straight into the main menu still logged in.
- Fixed an app freeze that could happen when certain warning or error messages appeared during login or while entering an item.

### Transfer Out no longer allows a blank List Number
The List Number field is now locked once a transfer is being set up, and the app automatically assigns a number if it's left blank when you submit — a blank List Number could previously go through and create a bad transfer record.
