# University Network Security Architecture

## Overview

This document presents a comprehensive security architecture for a large university network spanning multiple campuses, academic buildings, research laboratories, and student dormitories.

**Course:** CS 478 — Network Security | **Date:** March 18, 2026

---

## What's Inside

The 20-page architecture blueprint includes:

### 1. Executive Summary
- Why universities are high-value targets for cyberattacks
- The tension between openness (core to education) and security
- Defense-in-Depth principle as the core strategy

### 2. Network Diagram & Topology
- Layered security zones with clear trust boundaries
- Perimeter firewalls, core routers, data center isolation
- VPN gateway architecture for remote access
- Visual topology showing all critical entry points

### 3. Security Requirements (20 areas)
Comprehensive technical controls covering:
- **Perimeter Defense:** Network scanning defenses, firewall deployment, onion routing blocking
- **Monitoring & Detection:** Packet capture, vulnerability scanning, IDS/IPS deployment, proxy systems
- **Identity & Authentication:** Multi-factor authentication (MFA), credential stealing prevention, session hijacking defenses, cryptographic key management
- **Transport & Routing:** Man-in-the-middle protections, BGP security, VPN policies, DDoS mitigation, network redundancy
- **Advanced Threats:** Fuzzing attack defenses, covert channel detection, malware beaconing detection

### 4. Accepted Risks & Compensating Controls
Explicitly acknowledges residual risks:
- Zero-day exploits → EDR agents and rapid response
- Sophisticated encrypted covert channels → Host-level behavioral detection
- Insider threats → User/Entity Behavior Analytics (UEBA)
- Third-party/REN partner risks → BGP filtering and traffic monitoring
- Supply chain attacks → Hardware integrity verification

---

## Key Design Principles

**Defense-in-Depth:** Multiple independent layers of protection ensure no single compromise cascades across the entire network.

**Network Segmentation:** Dividing infrastructure into isolated zones limits lateral movement and blast radius.

**Least Privilege:** Every user and system receives minimum access necessary for their function.

**Zero Trust:** All internal traffic is inspected; no implicit trust based on network location.

---

## Technical Highlights

| Area | Control |
|------|---------|
| **Authentication** | FIDO2 hardware tokens for admins; TOTP for users |
| **Encryption** | TLS 1.3, AES-256, RSA-2048 minimum |
| **Monitoring** | 24/7 IDS/IPS, SIEM correlation, passive anomaly detection |
| **Scanning** | Continuous passive + monthly/quarterly/annual active assessments |
| **Logging** | 365-day retention, encrypted in transit & at rest, immutable audit trail |
| **Resilience** | Active/Passive failover, RAID 6 with off-site replication, multi-ISP connections |

---

## Why This Matters for Cybersecurity

This project demonstrates:
- **Institutional thinking:** Security decisions require buy-in at all organizational levels
- **Risk frameworks:** CISA compliance, NIST standards, accepted risk analysis
- **Practical architecture:** Balancing security controls with operational reality
- **Incident response:** Detection, containment, and recovery planning
- **Compliance mindset:** FERPA, research data governance, legal liability considerations

---

## File

**`University_Network_Security_Jaden_Cao.docx`** — Complete 20-page architecture document with detailed justifications, technical specifications, and references.

---

*Part of my cybersecurity portfolio, demonstrating institutional security architecture and risk-based decision making.*
