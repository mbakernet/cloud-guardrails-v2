# Protect Tier 0 Accounts

([Back](../README.md))

## Objective

Protect Tier 0 accounts that are used to establish the cloud service. A Tier 0 account is one that has enhanced privileges of the control plane and addresses all aspects of access control.

## Key Considerations

- [ ] Implement phishing-resistant multi-factor authentication (MFA) for Tier 0 privileged accounts (such as root or global admins or equivalent) , in accordance with GC Account Management Requirements.
- [ ] Implement a mechanism for enforcing access authorizations for Tier 0 accounts.
- [ ] Configure alerting on Tier 0 accounts to ensure the prompt detection of a potential compromise, in accordance with the [GC Event Logging Guidance](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf)
- [ ] Ensure that Tier 0 accounts are only accessible from approved and trusted locations (with the exception of break glass accounts).
- [ ] Use separate accounts for managing on-premise services and a separate non-federated account to administer cloud services to minimize the blast radius.

## Validation

- [ ] Confirm that MFA is enabled for root/Global Admin accounts through screenshots, compliance reports, or compliance check enabled through a reporting tool.

  Confirm and report the count of root/Global Admin accounts registered (should have at least two)

  Confirm and report the count of root/Global Admin accounts properly configured to require MFA

  Confirm and report the count of root/Global Admin accounts not properly configured to require MFA

- [ ] Verify that Tier 0 account access is enforced via assignment of out of the box roles (i.e. Not via custom roles).

  Verify that a review of Tier 0 accounts role assignment is performed at a minimum every 12 months. (Evidence can include policy, procedures and report of last access review)

- [ ] Confirm if monitoring and auditing of the Tier 0 account is implemented.

  Confirm alert notification to the authorized personnel is implemented flagging mis-use, suspicious sign-in attempts, or when changes are made to the root/global admin account.

- [ ] Confirm that just-in-time access for Tier 0 accounts to provide time-based and approval-based role activation.

- [ ] Provide evidence that attribute-based access control (ABAC) mechanisms are in place to restrict access based on attributes/signals such as authentication factors (MFA), managed devices, device compliance, sign-in and user risks, and location.

- [ ] Provide evidence that Tier 0 role activation requires approval and that privilege elevation is time-bound (temporary activation).

## Additional Considerations

- [ ] Enforce just-in-time access for Tier 0 accounts to provide time-based and approval-based role activation to mitigate the risks of excessive, unnecessary, or misused access permissions.
- [ ] Enforce attribute-based access control (ABAC) to restrict access based on combination of authentication factors (MFA), managed devices, device compliance, sign-in and user risks, and location.
- [ ] Leverage SSC's Administrative Access Control System (AACS) to enforce access control to privilege functions by configuring roles that requires approval for activation and choose one or multiple users or groups as delegated approvers.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Proposed Timelines

- 30 Days

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. Directive on Service and Digital - Appendix G: Standard on Enterprise IT Service Common Configurations, Account Management Configuration Requirements, subsection 2.2.
3. Cloud Authentication Guidance
4. [Recommendations for Two-Factor User Authentication Within the Government of Canada Enterprise Domain](https://intranet.canada.ca/wg-tg/rtua-rafu-eng.asp)
5. [GC Event Logging Guidance](https://www.gcpedia.gc.ca/gcwiki/images/e/e3/GC_Event_Logging_Strategy.pdf)
6. CSE Top 10 #3
7. ITSP.50.104 Guidance on Defence in Depth for Cloud-Based Services - Canadian Centre for Cyber Security
8. ITSP.30.031 v3, User Authentication Guidance for Information Technology Systems
9. Related security controls: A-2(2), AC-3,IA-2(1), AC-5, AC-6, AC-6(5), AC-6(10), AC-19, AC-20(3), IA-2(8), IA-2(11), IA-5(8), SA-4(12), SI-4, SI-4(5)
