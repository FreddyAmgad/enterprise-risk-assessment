# Enterprise GRC Risk Assessment Simulation

## 📌 Project Overview
This repository contains a comprehensive Governance, Risk, and Compliance (GRC) simulation for a hypothetical health-tech/e-commerce organization ("Saydalty"). The project demonstrates the ability to conduct a formal risk assessment, identify security gaps, and align organizational controls with industry-leading cybersecurity frameworks. 

## 🏢 Scenario Background
**Client:** Saydalty (Health-Tech Platform)
**Business Context:** A digital pharmacy platform integrating with a third-party financial service (FinHealth) to offer "Buy Now, Pay Later" installments. The organization operates a mix of on-premise infrastructure, physical pharmacy tablets, and a corporate open-plan office.
**Objective:** To identify physical, administrative, and technical vulnerabilities, calculate risk severity, and provide regulatory-aligned remediation strategies.

## 🛠️ Frameworks & Standards Applied
* **ISO/IEC 27001:2022** (Information Security Management Systems) 
* **NIST Cybersecurity Framework (CSF) v2.0**
* **PCI DSS v4.0** (Payment Card Industry Data Security Standard)

## 📂 Repository Contents
**`Saydalty_Risk_Register.csv`**: A detailed threat model and risk register evaluating 20+ risk scenarios across CIA (Confidentiality, Integrity, Availability) triads. It includes likelihood and impact scoring, residual risk calculations, and actionable remediation steps mapped to specific risk owners (e.g., CTO, COO, Legal Counsel).
* **`ISO_NIST_PCI_Mapping.csv`**: A custom compliance matrix mapping ISO 27001 Annex A controls (such as A.5.1 Policies for information security and A.8.2 Privileged access rights) directly to NIST CSF categories and PCI DSS requirements within a banking/fintech context.

## 🚨 Key Findings & Methodologies
The risk assessment uncovered critical vulnerabilities requiring immediate remediation, including:
1.  **Data Transmission & Integrity Risks:** Identified the transmission of sensitive National IDs and transaction values in plaintext via API calls, recommending HMAC Request Signing to prevent interception and tampering.
2.  **Cryptographic Weaknesses:** Highlighted the use of deprecated SHA-1 hashing and AES-128, recommending upgrades to industry-standard AES-256 to protect sensitive medical and financial data.
3.  **Physical & Environmental Security:** Assessed severe environmental risks to on-premise servers (e.g., broken AC leading to potential hardware failure) and unrestricted physical access to open-plan workspaces, proposing both physical and administrative access controls.
4.  **Network Architecture:** Discovered single points of failure and a lack of egress filtering or traffic monitoring, leaving the platform vulnerable to DoS attacks and data exfiltration.

* Regulatory Compliance Mapping
* Secure Software Development Lifecycle (SSDLC) Policy Enforcement
* Stakeholder Communication & Remediation Strategy
