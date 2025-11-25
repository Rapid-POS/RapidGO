# Changelog

All notable changes to this project will be documented in this file.

---

## [Rapid CP API V1.6.26] - 2025-12-02
### Fixed
- Resolved issue causing the `RapidPOS.API.CP` service to crash during server restart, shutdown, or power loss.
- Fixed EOCD error occurring when switching databases in settings.

### Enhanced
- Improved stability and error handling.

---

## [RapidGo V1.5.10] - 2025-12-02
### Fixed
- Price 1 not showing during receiving.
- Expected quantity displayed as zero in receiving.
- Transfer “From Location” incorrectly defaulting to *Main*.

### Enhanced
- Inventory Adjustment workflow now alerts users about unposted adjustments.
- Added reminder to post adjustments in Counterpoint after making changes in RapidGo.

---
# Rapid CP API V1.6.26 Release Notes

## Fixes
- Resolved issue where the `RapidPOS.API.CP` service crashed during server shutdown, reboot, or power loss.
- Fixed EOCD error when switching databases in the application settings.

## Enhancements
- Minor internal improvements for stability and reliability.

---
# RapidGo V1.5.10 Release Notes

## Enhancements
- Added user reminder when unposted inventory adjustments exist.
- Display prompts users to post adjustments in Counterpoint after adjusting items in RapidGo.

## Fixes
- Corrected issue where Price 1 was not displaying in receiving.
- Fixed expected quantity always showing zero during receiving.
- Resolved issue where Transfer “From Location” defaulted to *Main* location.

---
## 📦 Latest Releases

### **Rapid CP API**
- **Version:** V1.6.26  
- **Release Notes:** [View Details](./releases/Rapid-CP-API/V1.6.26.md)

### **RapidGo**
- **Version:** V1.5.10  
- **Release Notes:** [View Details](./releases/RapidGo/V1.5.10.md)

For full historical changes, see the [CHANGELOG](./CHANGELOG.md).
