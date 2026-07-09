# Portfolio Project: Vulnerability Scanning and Risk Assessment using OpenVAS & NIST SP 800-30

## **Objective**
To demonstrate the ability to discover network vulnerabilities using **OpenVAS** and evaluate the associated business risks utilizing the **NIST SP 800-30 Rev. 1** framework, culminating in a detailed assessment report and actionable remediation strategies.

## **Scope**
This assessment targets a centralized Linux server hosting a MySQL database, which is critical for marketing operations and stores customer, campaign, and analytic data. The scope involves scanning for known CVE-based vulnerabilities, analyzing current access controls over a three-month period, and guiding risk analysis using NIST SP 800-30 Rev. 1 to evaluate information system risk.

## **Action: Methodology & Execution**

**Phase 1: Deployment and Scanning with OpenVAS**
*   **Deployment:** Deployed OpenVAS (Greenbone Vulnerability Management) using a Docker container on an Ubuntu machine to effectively manage installation dependencies.
*   **Execution:** Configured a "New Task" via the Greenbone Security Assistant web interface, targeting the database server's IP address to discover hosts and scan for known vulnerabilities.
*   **Analysis:** Reviewed the severity of discovered vulnerabilities using CVSS scores and exported the technical findings as a comprehensive report for further risk analysis.

*For a step-by-step technical breakdown of the scanner deployment, please see my [OpenVAS Technical Log](OpenVAS.md).*

**Phase 2: Risk Assessment using NIST SP 800-30 Rev. 1**
*   **Threat Modeling:** Correlated the OpenVAS technical findings with potential **threat sources** (such as external hackers or internal employees) and **threat events** (e.g., reconnaissance, exfiltration, or denial of service).
*   **Risk Calculation:** Calculated a customized risk score based on the **Likelihood** (scored 1-3) of a threat source initiating an event and the **Severity** (scored 1-3) of its potential impact on day-to-day business operations. 

## **Result: Vulnerability Assessment Report**
*(Date: 25th November 2024)*

Based on the technical scan and NIST methodology, the following risks were identified given the open access permissions of the information system:

| **Threat source** | **Threat event** | **Likelihood** | **Severity** | **Risk Score** |
| ------ | ------ | ------ | ------ | ------ |
| *Hacker (Outsider)* | *Obtain sensitive information via exfiltration* | *3 (High)* | *3 (High)* | *9 (Critical)* |
| *Employee (Standard user)* | *Disrupt mission-critical operations* | *2 (Moderate)* | *3 (High)* | *6 (High)* |
| *Customer (Standard user)* | *Alter/Delete critical information* | *1 (Low)* | *3 (High)* | *3 (Moderate)* |

**Remediation Strategy:**
To mitigate these identified risks, the following controls are recommended to secure the database server:
*   **Access Control:** Implement role-based access controls (RBAC), enforce strong passwords, and require multi-factor authentication (MFA) to ensure only authorized users can access the system.
*   **Network Security:** Enforce IP allow-listing strictly to corporate offices to prevent unauthorized external internet connections to the database.
*   **Encryption:** Upgrade data-in-motion encryption protocols from SSL to TLS.

*To view the complete, formal risk analysis deliverable, please see my [Vulnerability Assessment Report](Vulnerability_assessment_report.md).*
