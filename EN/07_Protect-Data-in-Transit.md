# Protection of Data-in-Transit

([Back](../README.md))

## Objective

Protect data transiting networks through the use of appropriate encryption and network safeguards.

## Key Considerations

- [ ] Encrypt data in transit by default (e.g. TLS v1.2, etc.) to protect the confidentiality and integrity of data, including for all publicly accessible sites and external communications as per the GC Website and Services Configuration Requirements, and wherever possible for internal zone communication.
- [ ] Use CSE-approved cryptographic algorithms and protocols, in accordance with ITSP.40.111 and ITSP.40.062.
- [ ] Leverage non-person entity certificates from certificate authorities that align with the Recommendations for TLS Server Certificates.

## Validation

- [ ] Confirm that TLS v1.2 or above encryption is implemented for all cloud services (via HTTPS, TLS or other mechanism).

  While this is often the default, cloud platforms and cloud services often have configuration options to select the permitted TLS version.

- [ ] Cryptographic algorithms and protocols configurable by the consumer are leveraged in accordance with ITSP 40.111 and 40.062.
- [ ] Confirm that NPE certificates are issued from GC-approved certificate authorities.

## Applicable Service Models

- IaaS, PaaS, SaaS

## Proposed Timelines

- 60 Days

## References

1. [SPIN 2017-01](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/direction-secure-use-commercial-cloud-services-spin.html), subsection 6.2.4
2. Directive on Service and Digital - Appendix G: Standard on Enterprise IT Service Common Configurations, Web Sites and Services Management Configuration Requirements, section 1.
3. ITPIN Implementing HTTPS for Secure Web Connections: Information Technology Policy Implementation Notice (ITPIN) 2018-01 Appendix G, Web Sites and Services Management Configuration Requirements, subsection 1.
4. GC [Considerations for Cryptography in Commercial Cloud Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-consideration-use-cryptography-in-cloud.html)
5. [Recommendations for TLS Server Certificates](https://wiki.gccollab.ca/images/9/92/Recommendations_for_TLS_Server_Certificates_-_14_May_2021.pdf)
6. Refer to the cryptography guidance in [40.111](https://cyber.gc.ca/en/guidance/cryptographic-algorithms-unclassified-protected-and-protected-b-information-itsp40111) and [40.062](https://www.cse-cst.gc.ca/en/system/files/pdf_documents/itsp.40.062-eng.pdf).
7. Related security controls: SC‑8, SC‑8(1), SC‑12, SC‑13, SC‑17
