# Risk Register – Student Portal

## Risk Scoring Method

Likelihood and Impact are rated from 1 to 5.

Risk Score = Likelihood × Impact

- 1–5: Low
- 6–14: Medium
- 15–25: High

## Risk Assessment

| ID | Threat | Likelihood | Impact | Score | Priority |
|---|---|---:|---:|---:|---|
| R1 | Account Spoofing | 4 | 5 | 20 | High |
| R2 | Data Tampering | 3 | 5 | 15 | High |
| R3 | Missing Activity Logs | 3 | 3 | 9 | Medium |
| R4 | Information Disclosure | 3 | 5 | 15 | High |
| R5 | Denial of Service | 3 | 4 | 12 | Medium |
| R6 | Privilege Escalation | 3 | 5 | 15 | High |

## Detailed Risk Assessment

### R1 – Account Spoofing
- Asset: Student Account
- Owner: Application Administrator
- Entry Point: Login Page
- Trust Boundary: User to Application
- Scenario: An attacker attempts to access a student account using stolen credentials.
- Existing Control/Evidence: Not verified.
- Risk Rationale: High impact because unauthorized account access may expose personal information.
- Mitigation: Strong authentication and MFA.
- Verification: Test authentication controls in the authorized local environment.

### R2 – Data Tampering
- Asset: Student Records
- Owner: Database Administrator
- Entry Point: Backend API
- Trust Boundary: Application to Database
- Scenario: Unauthorized modification of student information.
- Existing Control/Evidence: Not verified.
- Risk Rationale: High impact because student records may become incorrect.
- Mitigation: Input validation and access control.
- Verification: Check that unauthorized changes are rejected.

### R3 – Repudiation
- Asset: Activity Logs
- Owner: Application Administrator
- Entry Point: Backend Server
- Trust Boundary: Application Environment
- Scenario: A user denies performing an important action.
- Existing Control/Evidence: Not verified.
- Risk Rationale: Missing logs make investigations difficult.
- Mitigation: Secure activity logging.
- Verification: Check whether important events have timestamps and user references.

### R4 – Information Disclosure
- Asset: Personal Student Information
- Owner: Database Administrator
- Entry Point: Database/API
- Trust Boundary: Application to Database
- Scenario: Unauthorized users access private student information.
- Existing Control/Evidence: Not verified.
- Risk Rationale: High impact because private information may be exposed.
- Mitigation: HTTPS and restricted database access.
- Verification: Confirm unauthorized users cannot access protected records.

### R5 – Denial of Service
- Asset: Student Portal Availability
- Owner: Application Administrator
- Entry Point: Web Application
- Trust Boundary: Internet to Application
- Scenario: Excessive requests affect application availability.
- Existing Control/Evidence: Not verified.
- Risk Rationale: Service disruption may prevent students from using the portal.
- Mitigation: Rate limiting and request monitoring.
- Verification: Review rate-limit configuration in the local environment.

### R6 – Elevation of Privilege
- Asset: Administrator Functions
- Owner: Application Administrator
- Entry Point: Backend API
- Trust Boundary: Student to Admin Access
- Scenario: A normal student attempts to access administrator-only functions.
- Existing Control/Evidence: Not verified.
- Risk Rationale: High impact because unauthorized administrative access can affect multiple accounts.
- Mitigation: Role-Based Access Control (RBAC).
- Verification: Confirm student accounts cannot access administrator-only functions.

## Conclusion

The risk assessment identifies account spoofing, data tampering, information disclosure and privilege escalation as high-priority risks.

These risks should be addressed first through appropriate security controls and verification.
