# Users and Groups

## Overview

The Linux server uses local users and groups to represent different roles within the simulated company environment.

Access is organized according to departmental responsibilities using Linux group management.

---

## Users

| User | Role | Primary Group |
|---|---|---|
| labadmin | System administrator | labadmin |
| itadmin | IT administrator | it |
| finance01 | Finance employee | finance |
| hr01 | HR employee | hr |
| developer01 | Developer | developers |

---

## Groups

The following groups were created to separate departmental access:

| Group | Purpose |
|---|---|
| it | IT operations and backup responsibilities |
| finance | Finance department resources |
| hr | Human resources resources |
| developers | Development project resources |

---

## Administrative Access

The labadmin account is used for system administration tasks.

The account has sudo privileges to allow controlled administrative operations during environment configuration and security testing.

---

## Security Purpose

Separating users into groups allows the system to enforce:

- Role-based access control
- Department separation
- Least privilege
- Controlled resource access

Users should only access resources required for their responsibilities.
