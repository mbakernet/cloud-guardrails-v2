# Enterprise Monitoring Accounts

([Back](../README.md))

## Objective

Create role-based account to enable enterprise monitoring and visibility.

## Key Considerations

- [ ] Enable enterprise visibility by establishing monitoring roles for GC approved stakeholders with read-only access following the least privilege principle to support validation of:

  - billing information
  - security configuration as part of cloud guardrails monitoring

- [ ] Review access privileges periodically, and remove access when it is no longer required.

## Validation

- [ ] Verify that roles required to enable GC visibility have been provisioned/assigned.
- [ ] Confirm if monitoring and auditing of the privileged and non-privileged accounts is implemented.

  Confirm alert notification to the authorized personnel is implemented flagging mis-use, suspicious sign-in attempts, or when changes are made to the privileged and non-privileged accounts.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Proposed Timelines

- 30 Days

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.3
2. Appendix G: Standard on Enterprise IT Service Common Configurations, Account Management Configuration Requirements, subsection 4 and 5
3. CSE Top 10 #2
4. Related security controls: AC‑2, AC‑2(1), AC‑3, AC‑5, AC‑6, AC‑6(5), AC‑6(10), AC‑7, AC‑9, AC‑19, AC‑20(3), IA‑2, IA‑2(1), IA‑2(2), IA‑2(11), IA‑4, IA‑5, IA‑5(1), IA‑5(6), IA‑5(7), IA‑5(13), IA‑6, IA‑8
