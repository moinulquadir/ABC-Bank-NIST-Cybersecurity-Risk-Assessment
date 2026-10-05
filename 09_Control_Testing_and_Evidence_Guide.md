# ABC Bank — Control Testing and Evidence Guide

## Testing principle

The tester should not simply ask whether a control exists. The test should determine:

1. Is the control properly designed?
2. Did the control operate during the review period?
3. Is there sufficient evidence?
4. Were exceptions identified?
5. Were exceptions remediated?
6. Is the remaining risk acceptable?

NIST SP 800-53A provides assessment procedures for evaluating security and privacy controls. This portfolio uses a simplified control-testing approach suitable for a bank security assurance exercise.

## Example test — MFA

**Control:** IAM-03  
**NIST:** IA-2  
**CSF:** PR.AA  
**Objective:** Verify MFA is enforced for privileged and remote access.

### Population
All privileged accounts and remote-access users.

### Sample
25 accounts selected using risk-based sampling.

### Evidence requested
- MFA configuration report
- IAM user export
- privileged account list
- VPN configuration
- authentication logs
- approved exception records

### Test procedure
1. Obtain the population from IAM.
2. Reconcile the population to the authoritative user directory.
3. Select sample.
4. Verify MFA status for each user.
5. Inspect exceptions and approvals.
6. Review authentication evidence.
7. Record exceptions.
8. Determine control effectiveness.

### Portfolio result
23 of 25 sampled accounts met the requirement.

**Conclusion:** Partially Effective.

**Finding:** Two privileged accounts were not enrolled in the required MFA mechanism.

**Risk:** An attacker obtaining either credential could bypass a key authentication layer.

**Management action:** Enroll both accounts, investigate why the accounts were excluded, and update the provisioning workflow.

---

## Example test — Patch Management

**Control:** END-01  
**NIST:** SI-2, RA-5  
**CSF:** PR.PS, ID.RA

### Evidence
- vulnerability scan report
- patch compliance report
- asset inventory
- remediation tickets
- approved exceptions

### Test
Select 30 critical/high-risk endpoints and servers. Compare current patch state to the bank's approved remediation SLA.

### Portfolio result
27 of 30 sampled assets were within the defined SLA.

**Conclusion:** Partially Effective.

**Finding:** Three assets exceeded the remediation SLA.

**Required action:** Patch or apply documented compensating controls; obtain risk approval for any exception.

---

## Example test — Backup Immutability

**Control:** BCP-01  
**NIST:** CP-9  
**CSF:** PR.DS, RC.RP

### Evidence
- backup architecture
- backup job reports
- immutability configuration
- restore test results
- privileged access list

### Test
Inspect whether critical production data has an isolated/immutable recovery copy and verify a restore test.

### Portfolio result
One critical application did not have the required immutable copy.

**Conclusion:** Ineffective for the affected application.

**Risk rating:** Critical.

**Remediation:** Enable immutable backup, restrict deletion privileges, and perform a documented restore test.

---

## Evidence quality rules

Good evidence should be:
- Relevant to the control objective.
- Dated or attributable to the review period.
- Complete enough to support the conclusion.
- Obtained from a reliable source.
- Protected from unauthorized alteration.
- Traceable to the tested population.

Avoid using screenshots alone when a system-generated report or export is available.

## Control testing workpaper fields

- Test ID
- Control ID
- Control objective
- NIST CSF reference
- NIST 800-53 reference
- Policy reference
- Procedure reference
- Control owner
- Review period
- Population
- Sample methodology
- Evidence requested
- Evidence received
- Test steps
- Exceptions
- Result
- Risk rating
- Finding ID
- Management response
- Retest date
- Final conclusion

## Three lines of defense

**First line:** business/technology control owners operate controls.

**Second line:** Information Security, Risk and Compliance establish standards, challenge control performance and monitor risk.

**Third line:** Internal Audit provides independent assurance.

Internal Audit should not be the owner of the control it independently tests.
