# RapidGO v1.09.02 Release Notes
**Release Date:** TBD
_Bug fixes and validation improvements for Receiving and Linebusting, including item entry performance, description handling, and display field corrections._

## New Features & Improvements

### Inactive and Unstocked Item Validation in Receiving
Receiving now prevents inactive items and items not stocked at the receiving location from being added to receivers, aligning RapidGO behavior with CounterPoint.

- Items marked inactive in CounterPoint can no longer be added to a receiver.
- Items not stocked at the receiving location can no longer be added to a receiver.

## Bug Fixes

### Receiving — Slow Performance When Adding Items
Adding items in Receiving was slow, particularly for items with many grid dimensions. Performance has been improved.

### Receiving — Blank Item Descriptions
Item descriptions could be blank when receivers were sent to CounterPoint. RapidGO now falls back to the default item description when a short or long description is unavailable.

### Receiving — Label Code Missing from Display Information Options
Label Code was not available as an option in Change Display Information. It is now available.

### Receiving — Error When Scanning or Entering Certain Items
Scanning or entering certain items in Receiving could cause an error and prevent the item from being added. This has been resolved.

### Linebusting — Object Reference Error During Item Entry
An object reference error could occur during item entry when required pricing rule setup was missing or incomplete. This has been resolved.
