# Environment Design

## Overview

This lab is a simulated enterprise Linux environment created to practice Linux administration and security assessment.

The goal is to build a realistic environment where access control, permissions, services, and security configurations can be analyzed.

---

## Lab Architecture

The environment consists of:

- Kali Linux (Security Testing Machine)
- Ubuntu Linux Server (Target System)

The Ubuntu server represents an internal company server hosting departmental resources.

---

## Target System

Operating System:

- Ubuntu 24.04.5 LTS

Hostname:

- linux-taarget

Purpose:

- Enterprise Linux simulation server

Network:

- Internal Lab Network
- IP Address: 192.168.100.101

---

## Company Structure

The server contains resources for different departments:

| Department | Resource |
|---|---|
| Finance | Payroll information |
| Human Resources | Employee records |
| Development | Application project files |
| IT Operations | Backup resources |

---

## Security Design

The environment uses Linux security principles:

- User-based access control
- Group-based permissions
- File ownership management
- Least privilege approach

Each department has its own Linux group to restrict access to relevant resources.

---

## Project Purpose

This environment will be used to practice:

- Linux enumeration
- Security assessment
- Permission analysis
- System hardening
- Security documentation
