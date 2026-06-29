# RapidGO v1.10.00 Release Notes

**Release Date:** July 1, 2026

_Adds Label Code editing to the Receiving line editor, and fixes silent search failures in Previously Saved Receiving and vendor lookup._

---

## New Features & Improvements

### Edit Item Label Code in Receiving

You can now change an item's Label Code directly from the device without going to Counterpoint.

* **Where:** Receiving → scan the item → swipe left on the line to open the line edit window.
* A Label Code dropdown defaults to the item's current code; select a new code from the available options, tap **Submit**, then tap **OK**.
* The change is applied to the item and a sync is triggered; the updated Label Code is reflected in both RapidGO and Counterpoint immediately.
* New label codes cannot be created in RapidGO — they must be added in Counterpoint first.

---

## Bug Fixes

### Previously Saved Receiving — Search Returns No Results

Typing in the Previously Saved Receiving search field found nothing, cleared the list, and left no selectable items until the Receiving module was closed and reopened. Search now returns matching receivers as expected.

### Vendor Lookup — Missing Results and Rendering Issues

Vendor searches were case-sensitive, so searching by name (e.g. `PANACEA`) returned no results if casing didn't match exactly. The lookup list also failed to render correctly — hiding the first result or dropping single-item results entirely. Vendor search is now case-insensitive, the list rebuilds reliably on every search, and all results are selectable.
