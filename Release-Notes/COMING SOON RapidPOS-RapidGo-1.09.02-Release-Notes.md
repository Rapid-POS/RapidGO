# RapidGO v1.09.02 Release Notes

**Release Date:** June 17, 2026

_New validation that keeps Receiving in step with CounterPoint, plus fixes across Receiving and Linebusting — faster item entry, correct item descriptions, a restored display option, and resolved item-entry errors._

## New Features & Improvements

### Receiving now blocks inactive and unstocked items

You can no longer add an inactive item, or an item that isn't stocked at the receiving location, to a receiver — keeping RapidGO in step with CounterPoint.

- Items marked inactive in CounterPoint can no longer be added to a receiver.
- Items not stocked at the receiving location can no longer be added to a receiver.

## Bug Fixes

### Adding certain items in Receiving no longer causes an error

We fixed an issue where scanning or entering certain items in Receiving could cause an error and stop the item from being added.

### Item descriptions no longer come through blank

We fixed an issue where item descriptions could be blank when receivers were sent to CounterPoint; RapidGO now falls back to the default item description when a short or long description isn't available.

### Linebusting no longer errors during item entry

We fixed an object reference error that could occur during item entry in Linebusting when required pricing rule setup was missing or incomplete.

### Faster item entry in Receiving

We improved performance when adding items in Receiving, especially for items with many grid dimensions.

### Label Code is now available in Change Display Information

We fixed an issue where Label Code was not available as an option in Change Display Information.
````
