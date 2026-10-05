# 11 — Internal Audit Report

## Audit objective
Determine whether the ISMS is implemented and operating as planned and whether it conforms to the organization's ISO/IEC 27001 requirements and selected Annex A controls.

## Audit scope
Clauses 4–10 plus risk management and a sample of Annex A controls covering governance, access, supplier security, incident response, continuity, vulnerability management, logging and secure development.

## Audit criteria
- ISO/IEC 27001:2022 requirements
- Approved Northstar ISMS policies and procedures
- Statement of Applicability
- Risk treatment plan

## Audit approach
Document review, interviews, sampling, configuration review and evidence inspection. The audit sampled 15 controls and 10 operational records.

## Findings
### NC-01 — Minor nonconformity
**Area:** Incident response exercises  
**Observation:** The tabletop exercise was completed, but two improvement actions were not tracked to closure in the corrective-action system.

**Risk:** Lessons learned may not translate into completed improvements.

**Required action:** Transfer actions to CAPA, assign owners and verify completion.

### OBS-01 — Observation
**Area:** Supplier security  
Some lower-tier suppliers had security questionnaires completed, but evidence of annual reassessment was inconsistent.

**Recommendation:** Add automated supplier review dates and escalation for overdue assessments.

### OBS-02 — Observation
**Area:** Asset inventory  
Two recently issued engineering laptops were added after the monthly inventory cycle.

**Recommendation:** Integrate device enrollment with asset-record creation.

## Positive practices
- Strong MFA adoption
- Clear source-code access controls
- Centralized security logging
- Defined risk owners
- Good secure-development evidence
- Restore testing performed rather than relying only on backup-success alerts

## Audit conclusion
The ISMS is substantially implemented and operating, with one minor nonconformity and two observations requiring follow-up. The audit does not itself constitute certification.

## Follow-up
CAPA is tracked in `12-capa-register.csv`. Effectiveness will be verified before the certification-readiness decision.
