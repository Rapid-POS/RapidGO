# RapidGO v1.10.00 Release Notes

**Release Date:** July 1, 2026

_Bug fixes resolving vendor search failures, previously saved receiving lookup, and item description display in receiver lines._

---

## New Features & Improvements

### Label Code Visible on Item Records

The label code field is now visible when viewing item details from a receiving or purchase request, making it easier to verify and reference label assignments without leaving the app.

---

## Bug Fixes

### Vendor Search Returning No Results

Searching for a vendor by name when creating a receiver or purchase request was returning no results even when matching vendors existed in CounterPoint. Vendor lookup now correctly returns matching results when searching by name.

### Previously Saved Receiving Search Not Working

The search function on the Previously Saved Receiving screen was not returning results, preventing users from locating in-progress receivers. Search on the Previously Saved Receiving screen now returns results as expected.

### Item Description Not Shown on Receiver Lines

The item description was not being displayed on receiver lines created in RapidGO, leaving the description column blank in CounterPoint after posting. RapidGO now correctly writes the item description when creating receiver lines, consistent with CounterPoint's native behavior.
