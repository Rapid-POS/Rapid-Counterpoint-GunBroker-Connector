# Rapid POS GunBroker Integration Release Notes  
Release Date: July 1, 2026

---

## Overview  
This release includes several bug fixes and enhancements improving GunBroker order processing, synchronization, connector functionality, and configuration options.

---

## Bug Fixes  

### Ext Cost Calculation Fix  
Fixed an issue where Extended Cost was not resetting to zero between orders when creating orders from GunBroker in Counterpoint.  
- Previously, this caused Ext Cost to incorrectly accumulate and increase with each new order.  
- Ext Cost now calculates and resets correctly for every order.

### GunBroker Feedback & Ship Status Sync Fix  
Fixed an issue preventing Ship Status and Buyer Feedback from sending to GunBroker after an order was Released/Completed and the drawer was posted in Touchscreen.  
- Previously, neither the shipped status nor the "Perfect Buyer" feedback comment was being sent to GunBroker following order release.  
- Orders released the prior day will now properly send the shipped status update to GunBroker, followed by buyer feedback.  
- Default Buyer Feedback can be set as part of the GunBroker.com configuration in Counterpoint.

### Run Connector Manually Button Update  
Updated the functionality of the "Run Connector Manually" button for the GunBroker connector to improve behavior and reliability when manually triggering a sync.

### EC_GUNBRKR Paycode Refund Setting  
Updated the EC_GUNBRKR paycode configuration to allow unlimited refunds.  
- Allows a GunBroker order to be refunded to the EC_GUNBRKR paycode.

Note: This is specifically for the GunBroker paycode. If a refund to the customer is necessary, that must still be completed via GunBroker._

---

## New Features & Enhancements  

### Consigned Item Support  
Added support for listing and processing consigned items through the GunBroker integration.  
- Consigned inventory can now be listed for sale and processed through orders.

### Mark All Messages as Read  
Added a "Mark All Messages as Read" option for GunBroker messages.  
- Allows users to clear message notifications in bulk instead of marking each message individually.

### 205 Workgroup Numbering & Drawer Assignment Update  
Updated the 205 Workgroup to populate numbers correctly.  
- Updated Store Settings so that Drawer Assignment defaults to "None."

---

## Removed  

### Item Price Options Removed from GunBroker Configuration  
Removed the Item Price Options section from the GunBroker Configuration window.  
- This option is no longer needed/applicable. 
- This setting is no longer required or applicable.

### Item Price Options Removed from GunBroker Configuration  
Removed the Item Price Options section from the GunBroker Configuration window.  
- This setting is no longer required or applicable.
