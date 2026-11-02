# STRIDE Threat Analysis – Student Portal

## 1. Spoofing
**Threat:** An attacker may try to access a student account using stolen login credentials.

**Affected Component:** Login System.

**Mitigation:** Use strong passwords and multi-factor authentication (MFA).

## 2. Tampering
**Threat:** An unauthorized user may try to modify student information.

**Affected Component:** Student Database.

**Mitigation:** Apply input validation and proper access controls.

## 3. Repudiation
**Threat:** A user may deny performing an action on the portal.

**Affected Component:** Backend Server.

**Mitigation:** Maintain secure activity logs with timestamps.

## 4. Information Disclosure
**Threat:** Private student information may be exposed to unauthorized users.

**Affected Component:** Student Database.

**Mitigation:** Use HTTPS and database access restrictions.

## 5. Denial of Service
**Threat:** Excessive requests may make the portal unavailable.

**Affected Component:** Web Application.

**Mitigation:** Implement rate limiting and request monitoring.

## 6. Elevation of Privilege
**Threat:** A normal student may try to access administrator functions.

**Affected Component:** Backend API.

**Mitigation:** Implement role-based access control (RBAC).