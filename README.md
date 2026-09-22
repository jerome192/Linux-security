# Linux Security Lab

## Overview

This project is a practical Linux security case study focused on building, assessing, securing, and validating an enterprise-style Linux environment.

The purpose is to apply Linux administration and security concepts in a controlled environment while developing practical skills relevant to cybersecurity and penetration testing.

The project follows a complete security assessment lifecycle:

**Build → Baseline → Assess → Find → Remediate → Validate → Document**

---

## Project Scenario

A simulated company has deployed an Ubuntu Linux server for internal operations.

The server contains resources belonging to different departments:

- Finance
- Human Resources
- Development
- IT Operations

Each department requires controlled access based on business responsibilities.

The environment is designed to provide a realistic setting for investigating Linux configuration, access controls, services, permissions, and other security weaknesses.

---

## Learning Objectives

This project aims to develop practical skills in:

### Linux Fundamentals

- Linux filesystem structure
- Users and groups
- File ownership
- Linux permissions
- Services and processes
- System configuration

### Security Fundamentals

- Least privilege
- Role-based access control
- Security baseline creation
- System enumeration
- Security assessment
- Misconfiguration analysis
- Vulnerability identification
- Remediation and hardening
- Security validation

### Security Assessment

- Reconnaissance
- Enumeration
- Service analysis
- Configuration analysis
- Evidence collection
- Security findings
- Root-cause analysis
- Remediation
- Validation testing

### Automation

Future development includes:

- Bash scripting
- Python automation
- Security-related tools

---

## Environment

### Target System

- Operating System: Ubuntu 24.04.5 LTS
- Environment Type: Isolated Virtual Lab
- Purpose: Enterprise Linux security simulation

### Assessment System

- Kali Linux
- Purpose: Security assessment and penetration testing

### Department Structure

| Department | Resource |
|---|---|
| Finance | Payroll information |
| Human Resources | Employee records |
| Development | Application project files |
| IT Operations | Backup resources |

---

## Security Case Study Workflow

The project follows a continuous security assessment lifecycle.

### Phase 1: Environment Construction

Build and configure the enterprise-style Linux environment, including users, groups, departmental resources, ownership, permissions, and required services.

### Phase 2: Baseline Evidence

Capture and document the initial state of the environment using actual system output and screenshots.

The baseline provides the reference state for later assessment, remediation, and validation.

### Phase 3: Black-Box Security Assessment

Approach the Linux server from Kali Linux as a security tester.

Perform reconnaissance, enumeration, and analysis to identify potential security weaknesses.

### Phase 4: Findings Analysis

Document discovered weaknesses using supporting evidence.

Each finding will explain:

- What was discovered
- How it was discovered
- The affected component
- Why it represents a security issue
- Potential impact
- Underlying cause

### Phase 5: Remediation and Hardening

Apply appropriate changes to address identified weaknesses.

The original condition, remediation action, and reason for the change will be documented.

### Phase 6: Security Validation

Re-test the affected areas after remediation to determine whether the original weakness has been addressed.

Before-and-after evidence will be captured where appropriate.

### Phase 7: Final Documentation

Consolidate the assessment, findings, remediation actions, and validation results into a complete security case study.

---

## Evidence-Based Documentation

The project emphasizes actual evidence rather than unsupported claims.

Evidence may include:

- Terminal output
- Screenshots
- Configuration evidence
- Enumeration results
- Finding evidence
- Remediation evidence
- Before-and-after comparisons

Each piece of evidence is accompanied by an explanation of what it demonstrates and why it is relevant to the security assessment.

---

## Current Progress

### Completed

- Ubuntu Linux target deployment
- Kali Linux assessment environment
- Enterprise-style department structure
- User and group configuration
- Access control implementation
- File ownership and permission configuration
- Initial system baseline collection
- Environment documentation
- Baseline evidence documentation

### Current Phase

- Black-box security assessment

### Upcoming

- Reconnaissance and enumeration
- Security findings
- Remediation and hardening
- Validation testing
- Final security case study

---

## Security Principles

The project applies practical security principles including:

- Least privilege
- Role-based access control
- Departmental separation
- Attack surface analysis
- Evidence-based assessment
- Secure configuration
- Remediation
- Validation

---

## Future Expansion

After completing the current Linux security case study, additional practical scenarios may be developed around:

- Linux privilege escalation
- Web application security
- Active Directory security
- Network penetration testing
- Host-based penetration testing
- Security automation

---

## Project Philosophy

The objective is not simply to configure a Linux system.

The project demonstrates the reasoning, evidence, methodology, and practical security decisions involved in assessing and improving a Linux environment.

**Build → Baseline → Assess → Find → Remediate → Validate → Document**

---

## Author

**Jerome Danquah Amoako**  
Aspiring Penetration Tester | BSc Information Technology | MBA Candidate
