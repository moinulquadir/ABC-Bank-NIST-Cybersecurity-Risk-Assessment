# ABC Bank — Security Control Catalog and Framework Mapping

## Purpose
This document converts the high-level NIST CSF 2.0 outcomes in this portfolio into operational controls that a bank could actually implement, own, test, and evidence.

NIST CSF 2.0 is outcome-oriented and does not prescribe a particular implementation. For this project, ABC Bank uses NIST CSF 2.0 as the governing cybersecurity framework and NIST SP 800-53 Rev. 5 as a detailed control reference. NIST SP 800-53 organizes controls into families such as Access Control, Audit and Accountability, Configuration Management, Contingency Planning, Identification and Authentication, Incident Response, Risk Assessment, System and Communications Protection, and System and Information Integrity.

Because ABC Bank is a fictional bank, the control IDs below are a portfolio implementation model, not a claim that a real institution has adopted them.

| Control ID | Control Name | NIST CSF 2.0 | NIST SP 800-53 Ref. | Bank Policy | Primary Owner | Key Evidence |
|---|---|---|---|---|---|---|
| IAM-01 | User Account Lifecycle | PR.AA | AC-2 | Identity & Access Management Policy | IAM Manager | JML tickets, account reports |
| IAM-02 | Privileged Access | PR.AA | AC-6 | Privileged Access Management Standard | IAM/Security | PAM logs, admin inventory |
| IAM-03 | MFA | PR.AA | IA-2 | Authentication Standard | IAM Manager | MFA enrollment report |
| IAM-04 | Access Recertification | PR.AA | AC-2, AC-6 | Access Review Procedure | IAM Manager | Quarterly certification |
| LOG-01 | Security Logging | DE.CM | AU-2, AU-12 | Logging & Monitoring Policy | SOC Manager | SIEM source inventory |
| LOG-02 | Log Review | DE.CM, DE.AE | AU-6 | SOC Monitoring Procedure | SOC Manager | SIEM review records |
| END-01 | Vulnerability/Patch Management | PR.PS | SI-2, RA-5 | Vulnerability Management Policy | IT Operations | Scan reports, patch reports |
| END-02 | Secure Configuration | PR.PS | CM-2, CM-6 | Configuration Management Standard | IT Operations | Baselines, exceptions |
| NET-01 | Network Segmentation | PR.IR | SC-7 | Network Security Standard | Network Manager | Firewall rules, diagrams |
| NET-02 | Remote Access | PR.AA, PR.PS | AC-17, IA-2 | Remote Access Standard | Network/IAM | VPN logs, MFA report |
| DATA-01 | Data Classification | ID.AM, PR.DS | AC-3, MP-4 | Data Classification Policy | DPO | Data inventory |
| DATA-02 | Encryption | PR.DS | SC-8, SC-13 | Encryption Standard | Security Engineering | TLS/config evidence |
| BCP-01 | Backup | PR.DS, RC.RP | CP-9 | Backup & Recovery Policy | Infrastructure | Backup reports |
| BCP-02 | Recovery Testing | RC.RP | CP-10 | DR Testing Procedure | Business Continuity | Test results |
| IR-01 | Incident Response | RS.MA, RS.AN | IR-4 | Incident Response Policy | CISO/SOC | Incident tickets |
| IR-02 | Evidence Preservation | RS.AN | AU-9, IR-4 | Incident Response Procedure | SOC | Evidence checklist |
| VEND-01 | Third-Party Risk | GV.SC | SR-3 | Third-Party Risk Policy | TPRM | Vendor assessment |
| RISK-01 | Risk Assessment | GV.RM, ID.RA | RA-3 | Enterprise Cyber Risk Policy | Risk Manager | Risk register |
| RISK-02 | Vulnerability Risk | ID.RA | RA-5 | Vulnerability Management Policy | Vulnerability Lead | Scan/remediation data |
| SDLC-01 | Secure Development | PR.PS | SA-11, SI-10 | Secure SDLC Standard | AppSec | SAST/DAST results |
| HR-01 | Security Awareness | PR.AT | AT-2 | Security Awareness Policy | HR/Security | Training report |
| PHY-01 | Data Center Security | PR.PS | PE-2, PE-3 | Physical Security Policy | Facilities | Badge review |
| AUD-01 | Independent Control Testing | GV.RM | CA-2, CA-7 | Security Assurance Policy | Internal Audit | Test workpapers |

## Control hierarchy

**Policy -> Standard -> Procedure -> Control -> Evidence -> Testing -> Finding -> Remediation -> Retest**

A policy states management's requirement. A standard defines the minimum technical or operational requirement. A procedure explains how employees perform the control. Evidence proves the control operated. Testing determines whether the control was designed and operating effectively.

## Bank control ownership model

- Board/Risk Committee: approves risk appetite and receives material cyber-risk reporting.
- CISO: accountable for the information security program.
- Risk Management: maintains enterprise cyber-risk methodology and reporting.
- IAM: identity lifecycle, authentication and privileged access.
- SOC: monitoring, detection, triage and incident response.
- Infrastructure/Network: systems, network controls, patching and resilience.
- Application Security: secure SDLC and application testing.
- Third-Party Risk Management: vendor cyber-risk assessments.
- Internal Audit: independent assurance; does not own management controls.

## Control status terminology

- Effective: design is adequate and operating evidence supports the control.
- Partially Effective: control exists but has exceptions, inconsistent operation, or incomplete coverage.
- Ineffective: control is absent or materially fails to address the risk.
- Not Tested: evidence was not sufficient to reach a conclusion.
