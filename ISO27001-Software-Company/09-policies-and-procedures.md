# 09 — Policies and Procedures

## Controlled document hierarchy
**Level 1:** Information Security Policy  
**Level 2:** Standards (access control, encryption, logging, secure development, vendor security)  
**Level 3:** Procedures (joiner/mover/leaver, incident response, vulnerability management, backup/restore, change management)  
**Level 4:** Records/evidence (tickets, logs, approvals, reports, training records)

## Core policies
1. Information Security Policy
2. Access Control Policy
3. Acceptable Use Policy
4. Asset Management Policy
5. Data Classification and Handling Standard
6. Cryptography Standard
7. Secure Development Policy
8. Vulnerability Management Procedure
9. Incident Response Procedure
10. Business Continuity / Disaster Recovery Policy
11. Supplier Security Policy
12. Privacy and PII Handling Policy
13. Logging and Monitoring Standard
14. Backup and Recovery Standard
15. Remote Work and Endpoint Security Policy
16. Change Management Procedure

## Example joiner/mover/leaver procedure
**Joiner:** HR creates approved identity record → manager confirms role → IT provisions minimum access → MFA enrolled → security training assigned.

**Mover:** Manager submits role change → access delta reviewed → obsolete access removed → new access approved → evidence retained.

**Leaver:** HR termination event triggers immediate account disablement → privileged sessions revoked → tokens/API keys assessed → equipment returned → records retained according to policy.

## Example incident procedure
Detect → validate → classify severity → contain → eradicate → recover → communicate → preserve evidence → lessons learned → corrective action.

## Example vulnerability procedure
Discover → validate → prioritize using severity/business context → assign owner → remediate → rescan → document exception if unresolved → report metrics.

## Document control
Every controlled document has an owner, version, approval date, review date and change history. Obsolete versions are protected from unintended use.
