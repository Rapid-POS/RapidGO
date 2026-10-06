# RapidGO v1.09.08 Release Notes

**Release Date:** October 11, 2026

_Cycle Count can now show item details like price and quantity on hand on each scanned line, plus fixes for Receiving and Android 15 devices._

## Feature Improvements

### Choose What Shows on Cycle Count Lines

You can now show an item's price and total quantity on hand on each scanned line during a cycle count, so you can check prices as you count and spot items that may have stock elsewhere in the store.

- Open the Cycle Count settings (cogwheel) and tap **Change Display Info** to pick fields such as **Price-1** and **Total QoH** and set their order. It's the same field picker used in Item Lookup and Receiving, and the fields show as read-only text on every line.
- Lines already on the list update as soon as you change your selection, and RapidGO remembers your choice the next time you open Cycle Count.
- **Total QoH** is the quantity on hand across all locations. We also added it to the Item Lookup and Receiving field pickers, where it only appears if you select it.

## Bug Fixes

### Pop-Up Screens Now Open on Android 15 Devices

On Android 15 devices, the Prompt for Quantity, Min/Max/Bin and Receiving pop-ups showed an error instead of opening. They open normally now.

### Quantity Expected Now Shows on Previously Saved Receivings

When you reopened a receiver from Previously Saved Receiving, the Quantity Expected column was missing. It now shows, just like it does when you receive against a purchase order.
