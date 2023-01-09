# Plan for Continuity

([Back](../README.md))

## Objective

Ensure that there is a plan for continuity of access and service that accommodates both expected and unexpected events.

## Key Considerations

- [ ] Document, implement, and test a break glass emergency account management process.
- [ ] Obtain signature from Departmental Chief Information Officer (CIO) and Chief Security Officer (CSO) to confirm acknowledgement and approval of the break glass emergency account management procedures.
- [ ] Develop a cloud backup strategy that takes into account where GC data is stored, replicated or backed up by the cloud service, in consideration of the IT continuity plan for the service/application.
- [ ] Ensure that cloud workloads are associated with the applicable Application ID in the TBS Application Portfolio Management (APM) tool, in support of the Standard on At-Risk Technology.
- [ ] Ensure departmental cyber security event management plans include cloud services, in alignment with the GC Cyber Security Event Management Plan.

## Validation

- [ ] Verify that a break glass emergency account management procedure has been developed

  Verify that break glass accounts are not subject to MFA, ABAC or AACS policies

  Verify that alerting is in place to report any use of break glass accounts

  Verify that testing of break glass account took place and that periodic testing is included in break glass emergency account management procedure.

- [ ] Confirm through attestation that the Departmental Chief Information Officer (CIO) and Chief Security Officer (CSO) have approved the break glass emergency account management procedure for the cloud service.
- [ ] Confirm through attestation that the cloud backup strategy procedure is developed and approved by the business owner.

  Verify if there are scripts that support the ability ot restore from code (e.g. infrastructure as code).

- [ ] Provide a list of all software, including versions, deployed on VMs associated with the application IDs from APM
- [ ] Confirm that the departmental event management plan includes contact information to reach the CSP in case of a security event or incident.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Proposed Timelines

- 60 Days

## References

1. SPIN 2017-01, subsection 6.2.9.
2. Directive on Service and Digital - Appendix G: Standard on Enterprise IT Service Common Configurations, System Management Configuration Requirements section
3. GC CSEMP
4. [Standard on at-risk technology](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32714).
5. [Considerations for Disaster Recovery in Cloud](https://www.gcpedia.gc.ca/gcwiki/images/3/39/Considerations_for_Disaster_Recovery_in_Cloud.pdf)
6. CSE Top 10 #3
7. ITSP.50.104 Guidance on Defence in Depth for Cloud-Based Services - Canadian Centre for Cyber Security
8. Refer to the following template for an example of a break glass emergency account management procedure.
9. Related security controls: AC-1, CP-1, CP-2, CP-9, PE-20, IR-4
