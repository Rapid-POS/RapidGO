# RapidGo v1.09.01 Release Notes

**Release Date:** May 15th, 2026

## Bug Fixes and Performance Enhancements

### Sign-In Error Resolved
Fixed an issue where users could encounter a sign-in failure when launching RapidGo.

- Resolved a database constraint issue related to duplicate barcode entries.
- Updated the `IM_BARCOD` table unique index to include the `SEQ_NO` column.
- Barcode records are now validated using `ITEM_NO`, `BARCOD`, and `SEQ_NO`, improving data integrity and preventing login-related errors.

### Label Tag Printing Validation Fixed
Fixed an issue where users received an error when adding items to the list of tags to print.

- Updated validation logic so that From and To location validation only applies to Transfer Out transactions.
- Users can now successfully create labels from tags without unnecessary validation errors.
