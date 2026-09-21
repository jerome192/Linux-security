# Access Control Design

## Overview

The Linux server uses ownership, groups, and file permissions to control access to company resources.

The access control model follows the principle of least privilege, where users receive access based on their department responsibilities.

---

## Department Resource Access Model

Each department has its own Linux group. Resources are assigned to the appropriate group to separate access between departments.

| Resource                | Department      | Owner | Group      |
| ----------------------- | --------------- | ----- | ---------- |
| `/srv/company/finance`  | Finance         | root  | finance    |
| `/srv/company/hr`       | Human Resources | root  | hr         |
| `/srv/company/projects` | Development     | root  | developers |
| `/srv/company/backups`  | IT Operations   | root  | it         |

---

## Permission Model

The baseline permission model is:

### Directories

```text
rwxrwx---
```

Meaning:

| Permission | Applies To       | Access               |
| ---------- | ---------------- | -------------------- |
| Owner      | root             | Read, Write, Execute |
| Group      | Department group | Read, Write, Execute |
| Others     | All other users  | No access            |

Example:

```text
drwxrwx--- root finance finance/
```

Only root and members of the finance group can access the directory.

### Files

```text
rw-rw----
```

Meaning:

| Permission | Applies To       | Access      |
| ---------- | ---------------- | ----------- |
| Owner      | root             | Read, Write |
| Group      | Department group | Read, Write |
| Others     | All other users  | No access   |

Example:

```text
-rw-rw---- root hr employees.txt
```

Only root and HR group members can read or modify the file.

---

## Security Principles Applied

### Least Privilege

Users should only access resources required for their job responsibilities.

Examples:

* Finance users access finance resources.
* HR users access HR resources.
* Developers access project resources.
* IT users access backup resources.

### Role-Based Access Control

Access is managed through Linux groups rather than individual user permissions.

This makes administration easier because users can be added or removed from departments without changing every file permission.

### Department Separation

Resources are isolated between departments to reduce unauthorized access.

A user belonging to one department should not automatically access another department's resources.

---

## Security Objective

This access control configuration creates a controlled baseline environment.

During later security assessment phases, this baseline will be used to identify:

* Incorrect permissions
* Excessive privileges
* Unauthorized access paths
* Configuration weaknesses
