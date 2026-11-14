# Findings Analysis

## 1. Introduction

This document evaluates observations obtained during the black-box security assessment of the target system.

The analysis is based on evidence collected remotely from Kali Linux. Its purpose is to determine whether the observed behaviour of exposed services indicates a security weakness that can be substantiated through assessment evidence.

The analysis distinguishes between:

- Confirmed security findings.
- Potential security concerns requiring further investigation.
- Informational observations that do not independently establish a vulnerability.
- Inconclusive assessment activities.

Only evidence-supported weaknesses will be classified as confirmed security findings.

This document currently covers the SSH service assessment. The analysis of other exposed services will be added as the assessment progresses.

## 2. SSH Service Analysis

### 2.1 Service Identification

The SSH service on `192.168.100.101` identified itself through its service banner as:

`SSH-2.0-OpenSSH_9.6p1 Ubuntu-3ubuntu13.19`

The version was also identified through Metasploit service fingerprinting.

**Evidence — SSH service banner:**

![SSH service banner](evidence/ssh-service-discovery.png)

**Evidence — Metasploit SSH version scan:**

![Metasploit SSH version scan](evidence/ssh-metasploit-version(1).png)

**Analysis:**

The banner identifies the SSH implementation and its reported version.

However, version identification alone does not establish that the service contains a known vulnerability. Ubuntu may incorporate security patches into its packages without changing the upstream OpenSSH version displayed in the banner.

Therefore, vulnerability status cannot be determined solely from the reported version.

**Disposition:** Informational observation. No vulnerability established.


