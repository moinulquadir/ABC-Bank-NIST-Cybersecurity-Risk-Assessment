# ABC Bank — Security Policy Set

These are portfolio-level policy documents. They are intentionally written as practical bank policy summaries rather than pretending to be legal or regulatory documents.

## POL-01 Information Security Policy

**Owner:** CISO  
**Approver:** Board Risk Committee  
**Review:** At least annually and after material changes

### Policy
ABC Bank shall maintain an information security program based on risk assessment, regulatory obligations, business requirements, and recognized security practices.

The program shall protect confidentiality, integrity and availability of customer information, payment systems, banking applications, employee systems and supporting infrastructure.

### Requirements
1. Security responsibilities shall be assigned to accountable business and technology owners.
2. Critical assets shall be identified and classified.
3. Cybersecurity risks shall be documented in the enterprise risk register.
4. Security controls shall be implemented according to risk.
5. Material exceptions shall be formally approved and tracked.
6. Security controls shall be periodically tested.
7. Material control deficiencies shall have remediation owners and target dates.
8. Management shall receive periodic cybersecurity risk reporting.

**NIST mapping:** GV.OC, GV.RM, GV.RR, ID.RA; NIST SP 800-53 PM-1, RA-3, CA-7.

---

## POL-02 Identity and Access Management Policy

**Owner:** IAM Manager

### Policy
Access to ABC Bank information systems shall be authorized based on job responsibilities, business need and least privilege.

### Requirements
- Unique user IDs are required.
- Joiner/mover/leaver events must trigger access changes.
- Privileged accounts must be separately identified and controlled.
- MFA is required for privileged, remote and other risk-sensitive access.
- Access must be reviewed periodically.
- Dormant accounts must be disabled according to the bank's retention standard.
- Shared privileged accounts are prohibited unless specifically approved and monitored.
- Terminated-user access must be removed promptly.

**NIST mapping:** PR.AA; AC-2, AC-3, AC-6, IA-2.

---

## POL-03 Security Logging and Monitoring Policy

**Owner:** SOC Manager

### Policy
ABC Bank shall collect and protect security-relevant logs from critical systems and review alerts for unauthorized access, fraud indicators, malware, privilege abuse and other suspicious activity.

### Requirements
- Critical systems must forward required security logs to the SIEM.
- Logs must include sufficient time, user, source and event information for investigation.
- Security logs must be protected against unauthorized modification.
- Detection rules shall be reviewed and tuned.
- High-severity alerts require documented triage.
- Log retention shall meet business, legal and regulatory requirements.

**NIST mapping:** DE.CM, DE.AE; AU-2, AU-6, AU-9, AU-12.

---

## POL-04 Vulnerability and Patch Management Policy

**Owner:** IT Operations Manager

### Policy
ABC Bank shall identify, prioritize and remediate vulnerabilities according to severity, asset criticality and exploitability.

### Requirements
- Authorized vulnerability scanning shall cover production assets.
- Critical vulnerabilities shall have defined remediation SLAs.
- Exceptions require documented risk acceptance or compensating controls.
- Internet-facing systems receive enhanced monitoring and remediation priority.
- Scan results shall be reconciled against the asset inventory.

**NIST mapping:** ID.RA, PR.PS; RA-5, SI-2.

---

## POL-05 Data Protection and Encryption Policy

**Owner:** Data Protection Officer / CISO

### Policy
Customer and sensitive bank information shall be classified and protected according to its sensitivity.

### Requirements
- Restricted data requires enhanced access controls.
- Sensitive data in transit shall use approved cryptographic protocols.
- Sensitive data at rest shall use approved encryption where required by risk and architecture.
- Access shall follow least privilege.
- Data handling and retention shall be documented.

**NIST mapping:** ID.AM, PR.DS; AC-3, SC-8, SC-13.

---

## POL-06 Incident Response Policy

**Owner:** CISO / SOC Manager

### Policy
ABC Bank shall maintain an incident response capability for detecting, analyzing, containing, eradicating and recovering from cybersecurity incidents.

### Requirements
- Incidents shall be classified by severity.
- Escalation paths shall be defined.
- Evidence shall be preserved.
- Business, legal, compliance, fraud and executive stakeholders shall be notified when appropriate.
- Regulatory/customer notification decisions shall be made by authorized functions.
- Significant incidents shall receive post-incident review.

**NIST mapping:** RS.MA, RS.AN, RS.CO, RS.MI; IR-4, IR-6.

---

## POL-07 Business Continuity and Disaster Recovery Policy

**Owner:** Business Continuity Manager

### Policy
Critical banking services shall have documented recovery objectives and tested recovery procedures.

### Requirements
- Critical services shall have defined RTO/RPO values.
- Backups shall be protected from unauthorized deletion and ransomware.
- Recovery procedures shall be documented.
- Restoration testing shall be performed periodically.
- Material test failures shall become tracked remediation items.

**NIST mapping:** RC.RP, RC.CO; CP-2, CP-9, CP-10.

---

## POL-08 Third-Party Cybersecurity Risk Policy

**Owner:** Third-Party Risk Management

### Policy
Third parties with access to ABC Bank systems, data or critical services shall be assessed according to risk before onboarding and periodically thereafter.

### Requirements
- Vendor criticality shall be established.
- Security due diligence shall be performed.
- Contractual security requirements shall be defined for material vendors.
- Vendor access shall be limited and reviewed.
- Material vendor findings shall be tracked to remediation.

**NIST mapping:** GV.SC; SR-3, SR-5, SR-6.

---

## POL-09 Security Awareness Policy

**Owner:** HR / Information Security

### Policy
Personnel shall receive security awareness training appropriate to their roles.

### Requirements
- New employees receive security awareness training.
- Annual refresher training is required.
- Privileged and specialized personnel receive role-based training.
- Phishing exercises may be performed.
- Completion exceptions are tracked.

**NIST mapping:** PR.AT; AT-2, AT-3.

---

## POL-10 Security Exception Policy

**Owner:** CISO / Risk Management

### Policy
A control exception shall not be treated as an informal waiver. Exceptions must document the affected asset, risk, business justification, compensating control, owner, expiration date and approval.

**NIST mapping:** GV.RM, ID.RA; PM-1, RA-3.
