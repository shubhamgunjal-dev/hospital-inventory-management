# Hospital Inventory & Equipment Management System

## 📌 Overview

The Hospital Inventory & Equipment Management System is a Microsoft Power Platform solution designed to help hospitals manage medical inventory, stock requests, medical equipment, maintenance activities, approvals, and reporting from a centralized application.

The solution is designed to improve inventory visibility, reduce manual processes, track expiry and equipment lifecycle, and provide management with actionable insights.

## 🎯 Business Problem

Hospitals need to manage a large number of medical consumables and equipment across different departments.

Manual inventory processes can make it difficult to:

- Track available stock
- Monitor batch numbers and expiry dates
- Prevent stock shortages
- Manage department stock requests
- Track medical equipment
- Manage equipment maintenance and calibration
- Handle damaged or expired items
- Track procurement activities
- Monitor inventory performance

This solution addresses these challenges using Microsoft Power Platform.

## 💡 Solution

The application provides a centralized platform for managing:

- Medical consumables
- Batch and expiry tracking
- Department-level inventory
- Stock requests and approvals
- Medical equipment
- Equipment allocation and movement
- Maintenance and calibration
- Damaged, expired and quarantined inventory
- Procurement
- Inventory analytics and reporting

## 🛠️ Technologies

| Technology | Purpose |
|---|---|
| Power Apps | Application interface |
| Dataverse | Data storage |
| Power Automate | Automation and approval workflows |
| Power BI | Reporting and analytics |
| Power Fx | Application logic |
| Copilot Studio | AI-assisted user interaction |

## ⭐ Key Features

- 📦 Inventory management
- 🏷️ Batch and expiry tracking
- ⏳ FEFO-based inventory management
- 🏢 Department-level stock management
- 📝 Stock request and approval process
- 🏥 Medical equipment lifecycle management
- 🔧 Equipment maintenance and calibration
- ⚠️ Damaged and expired inventory management
- 🛒 Procurement tracking
- 📊 Power BI analytics
- 🔐 Role-based access
- 🤖 Copilot/AI capabilities

## 🏗️ Solution Architecture

The solution uses Microsoft Power Platform components working together:

```text
Users
  │
  ▼
Power Apps
  │
  ├──────────────► Dataverse
  │                   │
  │                   ▼
  │             Business Data
  │
  └──────────────► Power Automate
                       │
                       ├── Approvals
                       ├── Notifications
                       └── Automated Processes
                              │
                              ▼
                          Power BI
                              │
                              ▼
                         Management
