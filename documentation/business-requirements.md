# Business Requirements

## 1. Project Overview

The Hospital Inventory & Equipment Management System is designed to provide a centralized solution for managing medical consumables, hospital equipment, stock requests, approvals, maintenance activities, procurement, and inventory reporting.

The solution is intended to reduce manual processes, improve inventory visibility, and help hospital departments manage resources efficiently.

---

## 2. Business Objectives

The main objectives of the solution are:

- Centralize inventory and equipment information.
- Improve visibility of available stock.
- Track batch numbers and expiry dates.
- Reduce stock shortages and wastage.
- Implement a structured stock request and approval process.
- Track medical equipment throughout its lifecycle.
- Manage equipment maintenance and calibration.
- Track damaged, expired, quarantined, and disposed inventory.
- Improve procurement visibility.
- Provide management with reporting and analytics.
- Automate notifications and repetitive processes.

---

## 3. Users and Roles

### Inventory Staff

Responsible for:

- Adding and updating inventory.
- Recording stock received.
- Recording stock issued.
- Monitoring stock levels.
- Managing batch and expiry information.
- Handling damaged and expired items.

### Department User

Responsible for:

- Viewing available inventory.
- Creating stock requests.
- Checking request status.
- Viewing department inventory.

### Department Manager

Responsible for:

- Reviewing stock requests.
- Approving or rejecting requests.
- Monitoring department inventory usage.

### Equipment Manager

Responsible for:

- Registering equipment.
- Assigning equipment to departments.
- Tracking equipment movement.
- Monitoring maintenance and calibration.

### Procurement User

Responsible for:

- Monitoring stock requirements.
- Managing procurement information.
- Tracking replenishment activities.

### Administrator

Responsible for:

- Managing application configuration.
- Managing users and security.
- Maintaining master data.
- Monitoring overall system operations.

---

## 4. Inventory Requirements

The system should allow authorized users to:

- Create inventory records.
- Update inventory information.
- Record product details.
- Track batch numbers.
- Track expiry dates.
- Record stock quantity.
- Monitor minimum stock levels.
- Identify low-stock items.
- Identify expiring items.
- Record stock received.
- Record stock issued.
- Maintain inventory transaction history.

---

## 5. Stock Request Requirements

Department users should be able to:

1. Select required products.
2. Enter requested quantities.
3. Submit a stock request.
4. View request status.
5. Track approved and rejected requests.

The system should prevent users from requesting invalid quantities.

---

## 6. Approval Requirements

When a stock request is submitted:

```text
Stock Request Submitted
        ↓
Manager Review
        ↓
   ┌────┴────┐
   ↓         ↓
Approved   Rejected
   ↓         ↓
Inventory   Request
Updated     Closed
