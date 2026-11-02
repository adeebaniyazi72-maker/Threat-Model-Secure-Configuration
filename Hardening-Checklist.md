# Security Hardening Checklist – Student Portal

## 1. Authentication Security
- [ ] Enforce strong password policies.
- [ ] Implement Multi-Factor Authentication (MFA).
- [ ] Configure login attempt limits.
- [ ] Use secure session management.

## 2. Data Protection
- [ ] Enforce HTTPS communication.
- [ ] Store passwords using secure password hashing.
- [ ] Restrict database access.
- [ ] Protect sensitive student information.

## 3. Input Validation
- [ ] Validate all user inputs on the server.
- [ ] Use parameterized database queries.
- [ ] Handle invalid inputs securely.

## 4. Access Control
- [ ] Implement Role-Based Access Control (RBAC).
- [ ] Restrict administrator functions.
- [ ] Verify authorization for protected resources.

## 5. Logging and Monitoring
- [ ] Record important login events.
- [ ] Monitor repeated failed login attempts.
- [ ] Protect activity logs from unauthorized modification.
- [ ] Never store passwords in logs.

## 6. Availability and Maintenance
- [ ] Configure rate limiting.
- [ ] Monitor unusual request patterns.
- [ ] Update software dependencies.
- [ ] Remove unnecessary services and permissions.

## Verification Plan

For every security control:
1. Review the relevant configuration.
2. Test it in the authorized localhost environment.
3. Record the test result.
4. Save supporting evidence.
5. Mark the control as verified only after successful testing.

## Status

Current status: Recommended controls – implementation and verification pending.

## Conclusion

This checklist provides a structured approach to improving the security of the Student Portal and reducing identified risks.