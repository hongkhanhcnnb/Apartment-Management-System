
# Apartment Management

## Overview

**Apartment Management** is a database-driven software project designed to support and automate the core operational processes of a modern apartment complex. It focuses on managing lease agreements, tracking tenant activity, handling amenity bookings, automating monthly billing, and providing a basic user interface to visualize apartment services.

This project is suitable as a prototype or academic demonstration of how structured database systems can support real-world facility and property management needs.

---

## Project Structure

```
Apartment Management/
├── Management System/     # Backend logic using SQL (stored procedures, triggers, views)
├── User System/           # Static website interface using HTML & multimedia
└── .git/                  # Version control directory (optional)
```

### Management System

Includes more than 40 SQL files, providing core business logic such as:

- Stored Procedures:
  - `add_lease.sql`, `BookAmenity.sql`, `Bill_unit_month.sql`, etc.
- Triggers:
  - Automatic updates on lease changes, tenant insert/update/delete
- Views:
  - Aggregated data: tenant list, booking history, payment records
- Utility Scripts:
  - Tenant count per month, unit availability, amenity popularity

> Database platform: **SQL Server**

---

### User System

A collection of static web pages used to showcase apartment types, amenities, and general building information.

- Key Pages:
  - `index.html`: Homepage
  - `studio.html`, `1-bedroom.html`, `2-bedroom.html`: Apartment types
  - `amenity.html`, `vendor.html`: Services and facilities
  - `contact.html`, `about.html`: Informational pages

- Media Assets:
  - JPEG, PNG, GIF, WebP images for UI illustration
  - Short demo videos (.mp4)

---

## Features

- Lease management via database procedures
- Amenity booking with conflict check
- Tenant and billing tracking
- Automatic data update using triggers
- Visual web interface (static HTML-based)

---

## Deployment

This is a prototype project and does **not include a backend API or dynamic integration** between frontend and database. However, you can run:

- SQL logic via Microsoft SQL Server or SSMS
- Frontend by opening `.html` files in any web browser

To extend the system:
- Add a backend API (Node.js, Python Flask, etc.)
- Connect frontend with dynamic data fetching

---

## Requirements

- [SQL Server](https://www.microsoft.com/en-us/sql-server) for database execution
- Modern browser for viewing HTML
- Optional: Web server (e.g., Apache, Nginx) to serve HTML files

---

## Potential Extensions

- Backend integration (RESTful API)
- Admin dashboard with authentication
- Real-time lease monitoring and payment history
- Mobile interface for tenants

---

## 📄 License

This project is for educational and demonstration purposes. Commercial usage requires prior permission.
