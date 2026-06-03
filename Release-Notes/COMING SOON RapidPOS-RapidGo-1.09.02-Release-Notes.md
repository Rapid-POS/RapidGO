# RapidGO v1.09.02 Release Notes

**Release Date:** TBD

## Bug Fixes

### Linebusting Hold Number Assignment

Resolved issues affecting hold-number creation and assignment during the Linebusting workflow.

* Fixed an issue where Linebusting hold documents could be sent to Counterpoint as `AUTO-ASSIGN` instead of receiving a usable hold number.
* Restored normal hold-number creation so newly created holds can be assigned correctly and retrieved in Counterpoint.

### Item Entry Error Handling

Improved error handling during item entry when pricing rule configuration is incomplete.

* Fixed an object reference error that could occur during item entry when required pricing rule setup was missing or incomplete.

