# RapidGO v1.09.08 Release Notes - Coming Soon

**Release Date:** TBD

_Cycle Count can now show item details like price and quantity on hand on each scanned line, plus fixes for Receiving and Android 15 devices._

## Feature Improvements

### Choose What Shows on Cycle Count Lines

You can now show an item's price and total quantity on hand on each scanned line during a cycle count, so you can check prices as you count and spot items that may have stock elsewhere in the store.

- Open the Cycle Count settings (cogwheel) and tap **Change Display Info** to pick fields such as **Price-1** and **Total QoH** and set their order. It's the same field picker used in Item Lookup and Receiving, and the fields show as read-only text on every line.
- Lines already on the list update as soon as you change your selection, and RapidGO remembers your choice the next time you open Cycle Count.
- **Total QoH** is the quantity on hand across all locations. We also added it to the Item Lookup and Receiving field pickers, where it only appears if you select it.

### Dedicated SQL Login for the Connector

The connector now connects to the Counterpoint database with its own dedicated SQL login, instead of sharing the main SQL login used by Counterpoint. Because the connector's database activity can now be identified separately from Counterpoint's, Rapid can limit how much of the SQL Server's CPU the connector uses, so that connector activity does not slow down Counterpoint for store users.

- The SQL login is created automatically during the connector upgrade. It is named with the client name followed by the connector name (for example, `CLIENTNAME_SHOPIFY`).
- The new login receives the same server and database permissions as the existing Counterpoint SQL login, so the connector continues to work the same way as before.
- A unique, strong password is generated for the login and is stored only in encrypted form in the connector's configuration. A new password is generated each time the connector is upgraded.
- Do not change the password for this SQL login or remove the login. The connector depends on it, and its password is managed automatically by the upgrade process.


## Bug Fixes

### Pop-Up Screens Now Open on Android 15 Devices

On Android 15 devices, the Prompt for Quantity, Min/Max/Bin and Receiving pop-ups showed an error instead of opening. They open normally now.

### Quantity Expected Now Shows on Previously Saved Receivings

When you reopened a receiver from Previously Saved Receiving, the Quantity Expected column was missing. It now shows, just like it does when you receive against a purchase order.
