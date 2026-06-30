# Rapid POS GunBroker Integration Release Notes  
_Release Date: [Insert Release Date]_

---

## Overview  
This release includes several enhancements and bug fixes improving order processing, synchronization, connector reliability, and expanded GunBroker integration functionality.

---

## Bug Fixes  

### Extended Cost Calculation Update  
Fixed an issue where Extended Cost was not resetting correctly between GunBroker orders created in Counterpoint.  
- Prevents Extended Cost from incorrectly accumulating across multiple orders.  
- Extended Cost now calculates correctly for each new order.

### GunBroker Feedback & Shipping Status Sync Update  
Fixed an issue where shipping status and buyer feedback were not being sent to GunBroker after an order was released/completed and the drawer was posted in Touchscreen.  
- Released orders now properly send shipping status updates to GunBroker.  
- Buyer feedback comments now send successfully after order completion.  
- Default Buyer Feedback can be configured within the GunBroker.com settings in Counterpoint.

### Manual Connector Sync Update  
Improved the "Run Connector Manually" functionality for the GunBroker connector.  
- Provides improved reliability when manually triggering synchronization.

### GunBroker Paycode Refund Update  
Updated the EC_GUNBRKR paycode configuration to allow unlimited refunds.  
- Allows GunBroker orders to be refunded back to the EC_GUNBRKR paycode.  

_Note: This applies specifically to the GunBroker paycode. Customer refunds must still be completed through GunBroker._

---

## New Features & Enhancements  

---

### Consigned Item Support  
Added support for consigned items within the GunBroker integration.  
- Consigned inventory can now be listed and processed through GunBroker orders.

### GunBroker Message Management Update  
Added a "Mark All Messages as Read" option for GunBroker messages.  
- Allows users to clear multiple message notifications at once.

### Workgroup Numbering & Drawer Assignment Update  
Updated Workgroup numbering and store settings behavior.  
- 205 Workgroup numbers now populate correctly.  
- Drawer Assignment now defaults to "None" within Store Settings.

---

## Removed  

---

### Item Price Options Removed from GunBroker Configuration  
Removed the Item Price Options section from the GunBroker Configuration window.  
- This setting is no longer required or applicable.

### Item Price Options Removed from GunBroker Configuration  
Removed the Item Price Options section from the GunBroker Configuration window.  
- This setting is no longer required or applicable.
