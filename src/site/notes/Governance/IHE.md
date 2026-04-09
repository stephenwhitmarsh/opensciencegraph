---
{"dg-publish":true,"permalink":"/governance/ihe/","tags":["icm/uses"],"dg-note-properties":{"name":"Integrating the Healthcare Enterprise","aliases":["IHE"],"website":"https://www.ihe.net","type":"working-group","scope":"international","domain":["clinical","health"],"status":"active","founded":1998,"parent_org":"HIMSS / RSNA (founding sponsors; now independent)","tags":["icm/uses"]}}
---


# IHE — Integrating the Healthcare Enterprise

## Overview

IHE is an international initiative that produces implementation specifications — called integration profiles — that define precisely how health IT standards such as [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/DICOM\|DICOM]], and [[Standards/SNOMED CT\|SNOMED CT]] should be applied together to solve specific clinical interoperability problems. Where standards bodies define the vocabulary and syntax, IHE defines the choreography: which transactions occur in which order, which actors send and receive them, and which options are required versus voluntary.

Founded in 1998 as a collaboration between HIMSS and the Radiological Society of North America (RSNA), IHE has since expanded far beyond radiology into laboratory, pathology, pharmacy, patient identity, document sharing, and IT infrastructure. It is now governed as an independent international organisation with national deployment initiatives active across Europe, North America, Asia and Australia.

## Integration Profiles

IHE profiles are grouped into domain-specific technical frameworks. Key frameworks relevant to this graph include:

- **IHE ITI (IT Infrastructure)** — foundational profiles for patient identity management (PIX/PDQ), cross-enterprise document sharing (XDS, XDR, XDM), audit logging (ATNA), and the FHIR-based Mobile access to Health Documents (MHD) profile used in [[Governance/EHDS\|EHDS]] implementation contexts
- **IHE RAD (Radiology)** — profiles governing [[Standards/DICOM\|DICOM]] workflow, scheduled imaging, results distribution and structured reporting; foundational to PACS and RIS integration at [[Actors/CENIR\|CENIR]] and [[Governance/AP-HP\|AP-HP]]
- **IHE LAB (Laboratory)** — profiles for laboratory order and result exchange; relevant to [[Standards/LOINC\|LOINC]]-coded result reporting
- **IHE PCC (Patient Care Coordination)** — clinical document profiles including the International Patient Summary (IPS), which is mandated under [[Governance/EHDS\|EHDS]]
- **IHE QRPH (Quality, Research and Public Health)** — profiles supporting clinical research, registries and public health reporting; relevant to [[Standards/CDISC\|CDISC]] and [[Standards/OMOP CDM\|OMOP CDM]] integration contexts

## Relationship to HL7 FHIR and DICOM

IHE does not compete with [[Standards/HL7 FHIR\|HL7 FHIR]] or [[Standards/DICOM\|DICOM]] but sits on top of them, specifying how implementations must use these standards to achieve confirmed interoperability. The Connectathon testing events — held annually in Europe and North America — allow vendors and institutions to validate implementations against IHE profiles in a structured environment. Software that passes Connectathon testing receives an IHE Integration Statement, which is increasingly required in public procurement.

## IHE Europe and IHE France

IHE Europe coordinates national deployment activities across the continent and contributes European requirements into the global profile development process. IHE France operates under [[Governance/ANS\|ANS]] oversight and is the primary vehicle through which [[Standards/HL7 FHIR\|HL7 FHIR]] French profiles and [[Standards/SNOMED CT\|SNOMED CT]] national release adaptations are aligned with IHE integration profiles in the French health IT ecosystem. [[Governance/AP-HP\|AP-HP]] deployments of document sharing and patient identity infrastructure are IHE-profiled.

## Relevance to EHDS

The [[Governance/EHDS\|EHDS]] regulation (EU 2025/327) mandates [[Standards/HL7 FHIR\|HL7 FHIR]] for EHR exchange but does not specify which IHE profiles to use. The European Commission's eHealth Network and [[Governance/ANS\|ANS]] are actively working with IHE Europe to identify the required profile set, making IHE the de facto implementation specification layer for EHDS technical compliance.

## Connections

- Builds on: [[Standards/HL7 FHIR\|HL7 FHIR]], [[Standards/DICOM\|DICOM]], [[Standards/SNOMED CT\|SNOMED CT]], [[Standards/LOINC\|LOINC]]
- Relevant to: [[Governance/EHDS\|EHDS]], [[Governance/ANS\|ANS]], [[Governance/AP-HP\|AP-HP]], [[Governance/ECRIN\|ECRIN]], [[Governance/Health Data Hub\|Health Data Hub]]
- Complements: [[Standards/CDISC\|CDISC]] (research data), [[Standards/OMOP CDM\|OMOP CDM]] (observational research)
- Testing mechanism: IHE Connectathon (Europe, North America)
- National node: IHE France (coordinated via [[Governance/ANS\|ANS]])

## Resources

- https://www.ihe.net
- https://www.ihe-europe.net
- IHE Technical Frameworks: https://www.ihe.net/resources/technical_frameworks/