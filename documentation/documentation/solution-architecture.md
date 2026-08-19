# Solution Architecture

## 1. Architecture Overview

The Hospital Inventory & Equipment Management System uses Microsoft Power Platform to provide a centralized application for inventory, equipment, approvals, automation, and reporting.

The solution consists of:

- Power Apps
- Microsoft Dataverse
- Power Automate
- Power BI
- Copilot Studio
- Microsoft Entra ID

---

## 2. High-Level Architecture

```text
                         Users
                           │
                           ▼
                    ┌──────────────┐
                    │  Power Apps  │
                    │ Canvas Apps  │
                    └──────┬───────┘
                           │
                           ▼
                  ┌──────────────────┐
                  │    Dataverse     │
                  │                  │
                  │ Inventory        │
                  │ Products         │
                  │ Departments      │
                  │ Stock Requests   │
                  │ Equipment        │
                  │ Maintenance      │
                  │ Procurement      │
                  └───────┬──────────┘
                          │
             ┌────────────┼────────────┐
             │            │            │
             ▼            ▼            ▼
      Power Automate   Power BI   Copilot Studio
             │            │            │
             ▼            ▼            ▼
        Approvals      Analytics    AI Assistance
        Notifications
        Alerts
