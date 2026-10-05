# ABC Bank — Operating Control Procedures

These procedures show what an analyst or control owner would actually do. They are the operational layer beneath the policies.

## PROC-IAM-01 Quarterly Access Review

**Frequency:** Quarterly  
**Owner:** IAM Manager  
**Evidence:** Access certification report, reviewer approvals, removal tickets

### Steps
1. Export active users and privileged accounts.
2. Reconcile users against HR's current employee population.
3. Identify terminated and transferred employees.
4. Send application/role listings to business owners.
5. Business owner confirms each user's continuing need.
6. IAM removes inappropriate access.
7. Evidence of removal is attached to the review record.
8. Exceptions are documented and escalated.
9. IAM Manager signs off the review.
10. Internal Audit/Security Assurance may sample the completed review.

**Control:** IAM-04  
**NIST:** AC-2, AC-6  
**CSF:** PR.AA

---

## PROC-IAM-02 Privileged Access Request

1. Requester submits a ticket with business justification.
2. Manager approves the request.
3. System owner confirms required role.
4. IAM verifies least privilege.
5. Security approval is required for sensitive administrative access.
6. Access is provisioned through PAM where applicable.
7. Session logging is enabled.
8. Access is assigned an expiration/review date.
9. Ticket is closed with evidence.

**Control:** IAM-02  
**NIST:** AC-6  
**CSF:** PR.AA

---

## PROC-IAM-03 MFA Enrollment Verification

1. Obtain current user population for in-scope systems.
2. Export MFA enrollment status.
3. Compare privileged and remote-access populations.
4. Identify users without MFA.
5. Open remediation tickets.
6. Verify enrollment after remediation.
7. Record exceptions and management approvals.
8. Retain report and evidence.

**Control:** IAM-03  
**NIST:** IA-2  
**CSF:** PR.AA

---

## PROC-SOC-01 Daily SIEM Alert Triage

1. Review high and critical severity alerts.
2. Validate whether the alert represents expected behavior.
3. Check user, endpoint, source IP, destination and timing.
4. Correlate related events.
5. Search for additional affected systems.
6. Assign severity.
7. Escalate confirmed or suspected incidents.
8. Record analyst disposition.
9. Preserve relevant evidence.
10. Close false positives only with a documented reason.

**Control:** LOG-02  
**NIST:** AU-6, AU-12, SI-4  
**CSF:** DE.CM, DE.AE

---

## PROC-VULN-01 Vulnerability Remediation

1. Run authorized authenticated and unauthenticated scans as applicable.
2. Reconcile scanner results to the asset inventory.
3. Remove duplicates and false positives.
4. Prioritize by severity, exploitability, exposure and asset criticality.
5. Assign remediation owner.
6. Create a ticket with SLA.
7. Apply patch/configuration change.
8. Rescan the asset.
9. Close only after remediation evidence is verified.
10. Escalate overdue items.

**Control:** END-01  
**NIST:** RA-5, SI-2  
**CSF:** ID.RA, PR.PS

---

## PROC-IR-01 Suspected Account Compromise

1. Open an incident record.
2. Confirm the affected user and systems.
3. Disable or restrict the compromised account when appropriate.
4. Revoke active sessions/tokens.
5. Preserve authentication and endpoint logs.
6. Review recent privileged or sensitive activity.
7. Search for lateral movement.
8. Reset credentials using approved procedures.
9. Determine whether customer/payment data was affected.
10. Escalate to Fraud, Legal, Compliance and management as required.
11. Document root cause and corrective actions.
12. Conduct a post-incident review.

**Control:** IR-01  
**NIST:** IR-4, IR-6  
**CSF:** RS.MA, RS.AN, RS.MI

---

## PROC-BCP-01 Critical System Restore Test

1. Select an in-scope critical application.
2. Confirm approved RTO/RPO.
3. Identify the backup set to be restored.
4. Restore to the approved test environment.
5. Validate data integrity.
6. Measure actual recovery time.
7. Compare actual results to RTO/RPO.
8. Record failures and dependencies.
9. Create remediation actions.
10. Obtain Infrastructure and Business Continuity sign-off.

**Control:** BCP-02  
**NIST:** CP-9, CP-10  
**CSF:** RC.RP

---

## PROC-TPRM-01 Vendor Security Review

1. Classify vendor criticality.
2. Identify data/system access.
3. Obtain security questionnaire and available independent assurance reports.
4. Review authentication, encryption, incident response, vulnerability management and continuity controls.
5. Record gaps.
6. Determine inherent vendor risk.
7. Establish remediation or compensating controls.
8. Obtain business/security approval.
9. Review material vendors periodically.

**Control:** VEND-01  
**NIST:** SR-3, SR-5, SR-6  
**CSF:** GV.SC
