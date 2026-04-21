# GiFo-RFC-0150 (V0.9.5)

G-PaC Integration Profile - Combined Credential- and Platform-bound Enforcement (CCPE-B)

New Request for Comments of Gimel Foundation (GiFo RFC) - G-PaC Integration Profile - Combined Credential- and Platform-bound Enforcement (CCPE-B)

Abstract of RFC: A second integration pattern within the “Combined Credential- and Platform-Bound Enforcement (CCPE)” family is now sufficiently visible to specify. Where GiFo-RFC 0140 (G-AGT Integration Profile) defines how GAuth's credential-bound enforcement integrates with “enterprise governance toolkits” (AGT-class engines, designated CCPE-A), this RFC defines how GAuth integrates with standalone Policy-as-Code (PaC) engines - Open Policy Agent (OPA / Rego), Cedar (AWS), and Zanzibar / SpiceDB (Authzed) - designated CCPE-B.

The two profiles share a common credential layer (GAuth's Power-Enforcement Point and the 16-check pipeline of GiFo-RFC 0117) and differ in the architectural shape of the platform-bound Phase 2 evaluator they integrate with. CCPE-A and CCPE-B are not alternatives in the sense that one displaces the other; they address different deployment realities - organizations whose authorization story is anchored in an AGT-class governance toolkit (CCPE-A) versus organizations whose authorization story is anchored in an existing PaC deployment with its own bundle servers, policy administrators, and pre-existing application embedments (CCPE-B).

This RFC is the engine-neutral integration profile. Its purpose is to specify how GAuth's Power-PEP chains to a downstream Policy-as-Code Policy-PDP, what must be true of the PaC engine for the integration to be conformant, and what the credential layer (and optionally the Gimel Auth Platform as the proprietary value-add layer) must supply that the PaC engine does not. Per-vendor cookbooks are explicitly out of scope and are deferred to companion documents or vendor-led contributions.

This document is published as a v0.9 draft under vendor review. Standards-body amplification to OPA / CNCF, AWS Cedar working group, and Authzed is sequenced after RFC 0140 v1.2 (which introduces the CCPE term and family taxonomy) has had its initial circulation period. The publication date itself is the relevant artifact — it establishes the credential-bound + Policy-as-Code integration architecture specification.


You are more than welcome to contribute !

Legal Provisions for users of this page

Please see the Legal Provisions under https://gimelfoundation.com

In particular the following terms apply:

GiFo RFC 0080 Legal Provisions for the Gimel Foundation

GiFo RFC 0090 Legal Provisions Related to Gimel Foundation Documents

GiFo RCC 0100 Rights Contributors Provide to the Gimel Foundation
