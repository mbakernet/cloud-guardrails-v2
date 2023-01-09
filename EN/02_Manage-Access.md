# Manage Access

([Back](../README.md))

## Objective

Establish access control policies and procedures for management of accounts.

## Key Considerations

- [ ] Document a process for managing accounts, access privileges, and access credentials for organizational users, non-organizational users (if required), and processes based on the principles of separation of duties and least privilege (for example, operational procedures and active directory). This process should be approved by Chief Security Officer (CSO) (or delegate) and designated official for cyber security.
- [ ] Implement a mechanism for enforcing access authorizations based on assigned roles.
- [ ] Implement phishing-resistant multi-factor authentication (MFA) for access to cloud-based services, in accordance with GC Account Management Requirements.
- [ ] Favor the use of built-in roles with known privilege assignments. Document any custom roles created.
- [ ] Change default passwords to one that is unique with at least 12 characters.
- [ ] Configure password policy in accordance with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/online-security-privacy/password-guidance.html).
- [ ] Implement password protection mechanisms to protect against password brute force attacks.
- [ ] Establish a guest user access policy and procedures that minimizes the number of guest users and manages their lifecycle where accounts are deprovisioned when access is no longer needed.

## Validation

- [ ] Confirm that the Access Control procedure for management of administrative accounts have been documented for the cloud service. (This can be confirmed through attestation)

  Verify that administrative account management procedures include provision for:

  1. Validating that role assignment is for a unique organization user account (not a shared account, nor a non-organization user);
  2. Documenting rational for role assignment;
  3. Validating that the least privilege role is assigned;
  4. Requiring and documenting approval for such role assignment;
  5. Terminating of role assignment upon job change or termination;
  6. Performing periodic reviews of role assignment (minimum yearly);
  7. Disabling default and dormant accounts;
  8. Avoiding use of user generic accounts.
  9. ensuring Segregation of duties for roles such as Security, system administration

  Demonstrate access configurations and policies are implemented for different classes of users.

  Confirm that mechanism to uniquely identify and authenticate users to the cloud service is implemented.

- [ ] Confirm that MFA is enabled for each class of user (non-privileged, and privileged users) through screenshots, compliance reports, or compliance check enabled through a reporting tool.

  Confirm and report the count Admin accounts registered

  Confirm and report the count of Admin accounts properly configured to require MFA

  Confirm and report the count of Admin accounts not properly configured to require MFA

  Confirm that the MFA mechanism(s) used meets the requirement for authentication level of assurance (SMS, phone should be avoided, while authenticator app, hard token, FIDO2 should be favored)

- [ ] Demonstrate that cloud platform built-in roles are used. Custom roles can be used but rationale should be documented and approved.

- [ ] Confirm that the default passwords have been changed for all the built-in accounts for the cloud-service.

- [ ] Confirm password policy aligns with [GC Password Guidance](https://www.canada.ca/en/government/system/digital-government/online-security-privacy/password-guidance.html) as appropriate.

- [ ] Confirm that account lock out policies are enabled for all users.

  Demonstrate that password policy for the cloud platform has been configured as per the GC Password Guidance:

  1. Require longer passwords – At least 12 characters in length without a maximum length limit;
  2. Blacklist common passwords and combinations, such as “Password1!”;
  3. Counter online guessing or brute forcing of passwords using throttling, account lockout policies, monitoring, and multi-factor authentication;
  4. Protect against offline attacks using effecting hashing, salting, and keyed hashing.

- [ ] Confirm only the required guest user accounts are enabled.

  Provide list of non-organizational users with elevated privileges.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Proposed Timelines

- 30 Days

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. Directive on Service and Digital - Appendix G: Standard on Enterprise IT Service Common Configurations, Account Management Configuration Requirements, subsection 3
3. CSE Top 10 #2
4. Refer to the [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
5. Related security controls: AC-1, AC‑2, AC‑2(1), AC-2(7), AC‑3, AC-3(7), AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(3), IA‑2(11), IA-3, IA‑4, IA‑5, IA‑5(1), IA‑5(6), SI-4, AU-6, AU-12
