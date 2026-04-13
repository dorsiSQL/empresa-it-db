# IT Company Database 🖥️

A relational database built in SQLite that models the core commercial operations of an IT company — including customer management, product sales, employee records, and technical service tracking.

## Project Structure

```
empresa-it-db/
│
├── empresa_it.db       # SQLite database
└── README.md
```

## Database Schema

The database consists of 6 tables:

**Customers** — stores both individual and corporate clients, identified by `CustomerType` as `Person` or `Company`.

**Employees** — company staff with defined roles: `Technician`, `Sales`, and `Admin`.

**Products** — catalog of items sold, categorized as `Hardware`, `Software`, or `License`, with price and stock tracking.

**Orders** — sales header records linking a customer to an employee with a transaction date.

**OrderDetails** — line items for each order, recording product, quantity, and unit price at the time of sale.

**Tickets** — technical service records tracking support requests, installations, and repairs, with open/in-progress/closed status and assigned technician.

## Entity Relationship Overview

```
Customers ──< Orders >── Employees
               │
               └──< OrderDetails >── Products

Customers ──< Tickets >── Employees
```

## Technologies

- SQLite 3
- SQL (DDL + DML)

## Status

🚧 In progress — actively being developed as a learning project focused on SQL for data analysis.

## Author

David — Junior Data Analyst in training.
