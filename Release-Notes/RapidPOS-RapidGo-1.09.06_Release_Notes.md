# RapidGO V1.09.06 Release Notes
**Release Date:** August 10, 2026

Bug fix release addressing an incorrect zero-price display during Line Busting when a price rule references a field unavailable on the device.

## Bug Fixes

### Line Busting: Incorrect $0.00 Ext Price
Ext Price no longer shows $0.00 when a configured price rule references a field the device doesn't have locally; the item is now priced normally instead.
