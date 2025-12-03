# RapidGo v1.05.08 Release Notes

_Release Date: July 29, 2025_

## New Functionality

### Multiple Receivings from the Same PO Without Posting

A new setting has been added: **Prevent Double Receiving**  

- **When checked (default & recommended):**  
  - Prevents users from creating a new receiver from the same purchase order until the first receiver has been posted.  
  - Ensures accuracy and avoids duplicate receiving.  

- **When unchecked:**  
  - Allows multiple receivers to be created from the same PO without posting any of them.  
  - This may lead to duplicate receiving events and cause **inventory count errors**.  

---

## Bug Fixes and Performance Enhancements

- **Change Display Info**  
  - Functionality has been restored.  
  - Users can now add or remove additional item information as expected.  

- **Line Busting Stability**  
  - Resolved a crash that occurred during Line Busting.  
  - A new prompt now notifies users if there is no default Walk-In Customer assigned.  
