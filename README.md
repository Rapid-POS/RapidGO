# RapidGO
Updated June 17th 2026

RapidGO is a mobile inventory and retail operations application developed by Rapid POS, installed on a Zebra Android handheld device. It connects to CounterPoint to support a range of store tasks — from item lookup and inventory adjustments to receiving and line busting — directly from the sales floor or warehouse.

> **Note:** RapidGO cannot be used to complete transactions or process payments.

---

## Overview

RapidGO runs on a Zebra Android device and communicates with CounterPoint over a secure Wi-Fi connection or a 4G/5G cellular data plan. Because a SIM card can be installed in the device, RapidGO can be used anywhere with cellular connectivity — not just within the store.

- 📹 [Video Overview](https://www.youtube.com/watch?v=4oJQuaFQzIY)
- 🎓 [RapidGO Courses at CounterPoint University](https://counterpointuniversity.com/courses/rapidgo/)

---

## System Requirements - Software

| Requirement | Minimum Version |
|-------------|----------------|
| Counterpoint | 8.5.6.2 |
| SQL Server | 2016 |
| Windows Server | 2016 |
| PowerShell | 5.1 |

> [!WARNING]
> Your environment must meet our [CI/CD Connector Requirements](https://github.com/Rapid-POS/Miscellaneous-Documents/blob/main/CICD-Connector-Requirements.md) (server access, firewall rules, etc.) before any install or upgrade. Troubleshooting, manual installs, or follow-up work resulting from unmet requirements will be billed at standard T&M rates.

If your system does not meet these minimum requirements, please consult your Care Team Lead (vCIO) for an upgrade quote.

## Hardware Requirements

| Requirement | Details |
|---|---|
| **Device** | Zebra TC27 or compatible Zebra Android handheld |
| **OS** | Android 13 GMS |
| **Network** | Secure Wi-Fi and/or 4G/5G data plan (provided by StoreX) |
| **POS** | CounterPoint (compatible version required) |

---

## Table of Contents

- [Section 1: Features](#section-1-features)
- [Section 2: Hardware](#section-2-hardware)
- [Section 3: Pricing](#section-3-pricing)
- [Section 4: Item Lookup](#section-4-item-lookup)
- [Section 5: Inventory Adjustments](#section-5-inventory-adjustments)
- [Section 6: Transfer Out](#section-6-transfer-out)
- [Section 7: Tags / Labels](#section-7-tags--labels)
- [Section 8: Line Busting](#section-8-line-busting)
- [Section 9: Cycle Counts](#section-9-cycle-counts)
- [Section 10: Receivings](#section-10-receivings)
- [Section 11: Pick Verify](#section-11-pick-verify)
- [Section 12: Settings](#section-12-settings)
- [Training and Resources](#training-and-resources)

---

## Section 1: Features

RapidGO supports the following functions within CounterPoint:

| Feature | Description |
|---|---|
| **Item Lookup** | Check stock levels and pricing from anywhere on the floor |
| **Item Maintenance** | Update Min/Max, Bin, Price, and Barcode |
| **Inventory Adjustments** | Make quantity adjustments directly from the device |
| **Transfer Out** | Initiate inventory transfers between locations |
| **Tags / Labels** | Create a list of labels to print from CounterPoint |
| **Line Busting** | Assist customers in line by looking up items and building tickets |
| **Cycle Counts** | Perform physical inventory counts by location or department |
| **Receivings** | Receive inventory with or without a purchase order |
| **Pick Verify** | Pick and verify orders using the Pick Verify module |

Any new features added to the platform are included automatically during the active subscription period.

---

## Section 2: Hardware

RapidGO is installed on a **Zebra TC27 handheld device**.

### Zebra TC27 Specifications

- 6.0" display
- 1D/2D imager
- Android 13 GMS
- Includes: battery, protective boot, USB-C charging cable + adaptor, and Zebra OneCare Essential 3-year service plan

See the Zebra OneCare Essentials Fact Sheet for full service plan details.

### Hardware Pricing

| Item | Price |
|---|---|
| Zebra Handheld Device (TC27) | $2,148.00 |
| Trigger Handle | $353.00 |
| Single Slot Ethernet Charging Cradle *(optional)* | $650.00 |
| 5-Slot Charging Cradle *(optional)* | $1,242.00 |
| Extra Battery for TC27 | $129.00 |

> **Note on cradles:** The handheld charges via USB-C, similar to most modern phones. Cradles are optional and offer a more convenient charging method but are not required.

---

## Section 3: Pricing

| Item | Price |
|---|---|
| Initial Setup & Configuration (per store) | $99.00 |
| RapidGO Subscription (per device / per month) | $65.00/mo |
| Start-up Q&A session (up to 1.5 hours) | $234.00 |

**Important subscription notes:**

- If replication must be deployed, the setup and configuration fee applies per store.
- The RapidGO subscription is **month-to-month** and can be cancelled with 30 days written notice.
- Restarting a subscription after cancellation will require an additional configuration fee.
- Additional support services are available on a pay-as-you-go basis at the standard hourly rate, billed in quarter-hour increments.
- Physical Count support services are always billed at T&M 

---

## Section 4: Item Lookup

RapidGO allows staff to look up items directly from the device without returning to a fixed terminal. Item Lookup has view into your Counterpoint Item's Qty on Hand, last/average/historical costs, prices and vendor informatio.

---

## Section 5: Inventory Adjustments

Inventory Adjustments in RapidGO allow staff to make quantity changes to on-hand inventory directly from the device. Adjustments are submitted to CounterPoint in real time. Note: RapidGO does not post anything so posting of adjustments will need to be completed in standard Counterpoint.

---
## Section 6: Transfer Out

The Tranfer Out function allows stff to initiate inventory transfers between locations from the device. Transfer records are sent to Counterpoint where the transfer posting must be finalized.

---
## Section 7: Tags / Labels

RapidGO allows staff to create a list of labels to be printed from CounterPoint. Labels are queued from the device and printed through the standard CounterPoint label printing process.

---

## Section 8: Line Busting

Line Busting allows staff to assist customers in line by looking up items and building tickets from the device, reducing wait times during peak periods.

> **Note:** Line Busting does not support the ability to complete a ticket or take payment. Transactions must be finalized at a CounterPoint terminal.

---

## Section 9: Cycle Counts

RapidGO supports physical inventory cycle counts by location or department. Cycle Counts sent to Counterpoint need to be reviewed and posted in Counterpoint.

---

## Section 10: Receivings

Receivings allows staff to receive inventory directly from the device, with or without a purchase order. Receiving records are created in CounterPoint following standard receiving rules.

---

## Section 11: Pick Verify

The Pick Verify module supports order picking workflows. Staff can pick and verify orders from the device, with activity recorded in CounterPoint.

### How to Pick an Order Using Pick Verify

Refer to the Pick Verify course in CounterPoint University for step-by-step instructions:
🎓 [counterpointuniversity.com/courses/rapidgo](https://counterpointuniversity.com/courses/rapidgo/)

---

## Section 12: Settings

RapidGO Settings allow you to change functionality of various RapidGO features. Settings should be reviewed during initial setup and adjusted as needed in consultation with your Rapid POS representative.

---

## Training and Resources

Full training for RapidGO is available through **CounterPoint University**:
🎓 [counterpointuniversity.com/courses/rapidgo](https://counterpointuniversity.com/courses/rapidgo/)

### Course Topics

- Signing in to RapidGO
- Item Lookup Using RapidGO
- Inventory Adjustments with RapidGO
- Transfer Out Using RapidGO
- Using the Tags Function of RapidGO
- Using RapidGO for Line Busting
- Utilizing RapidGO for Cycle Counts
- Receiving Inventory Using RapidGO
- Pick Verify Module
- How to Pick an Order Using Pick Verify
- Learning RapidGO Settings

---

## Conclusion

RapidGO extends CounterPoint to the sales floor and warehouse, giving staff the tools to look up items, manage inventory, receive goods, and assist customers — all from a single handheld device. Before go-live, confirm that your network environment meets the connectivity requirements and that the device has been configured by a Rapid POS representative.

For assistance with setup, configuration, or troubleshooting, contact Rapid Support.	
