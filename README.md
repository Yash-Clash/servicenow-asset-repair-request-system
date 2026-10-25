# ServiceNow Asset Repair Request System

## Overview

The Asset Repair Request System is a ServiceNow application designed to manage and track repair requests for company assets. It provides a structured way to record asset issues, assign requests to service desk personnel, prioritize repairs, and monitor request progress.

## Objectives

- Create and maintain asset repair requests.
- Associate requests with assets and requesting users.
- Assign repair requests to service desk personnel.
- Prioritize requests according to urgency.
- Track request status throughout the repair lifecycle.
- Maintain work notes for repair-related updates.

## Technology Stack

- **Platform:** ServiceNow
- **Development Environment:** ServiceNow App Engine Studio
- **Data Storage:** ServiceNow Tables
- **Access Control:** ServiceNow Roles and Access Control Rules

## Application Features

### Repair Request Management

Each request contains a unique request number, requested-by user, asset reference, priority, status, assigned technician, description, and work notes.

### Priority Management

Requests can be classified as Critical, High, Moderate, or Low.

### Status Tracking

The application supports request statuses including New, In Progress, On Hold, Completed, Closed, and Cancelled.

### Role-Based Access

The application defines Employee, Service Desk, and Admin roles to support different levels of access.

## Data Model

The application uses the `Asset Repair Request` table.

**Table name:** `x_2190305_asset_0_asset_repair_request`

Important fields include:

| Field | Purpose |
|---|---|
| Number | Unique repair request identifier |
| Requested by | User who raised the request |
| Asset | Asset associated with the repair |
| Priority | Urgency of the repair |
| Status | Current request state |
| Assigned to | Person responsible for the request |
| Description | Details of the reported issue |
| Work notes | Repair-related updates |

## Testing

A test repair request was created successfully to verify record submission, automatic request numbering, and display in the request list.

## Repository Structure

```text
servicenow-asset-repair-request-system/
├── documentation/
├── screenshots/
└── README.md
```

## Project Evidence

Screenshots and supporting documentation will be added to this repository as the project progresses.

## Disclaimer

This project is developed for learning and demonstration purposes. The application and its access controls should be tested thoroughly before use in a production environment.
