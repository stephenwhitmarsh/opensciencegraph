---
{"dg-publish":true,"permalink":"/governance/cnil/","dg-note-properties":{"name":"Commission Nationale de l'Informatique et des Libertés","aliases":["CNIL"],"website":"https://www.cnil.fr","type":"policy","scope":"french","domain":["clinical","health","genomics"],"status":"active","founded":1978,"parent_org":"French State (independent administrative authority)","tags":null}}
---


# CNIL — Commission Nationale de l'Informatique et des Libertés

## Overview

CNIL is France's independent data protection authority, established by the Loi Informatique et Libertés of 6 January 1978, one of the earliest national data protection laws in the world. It is responsible for ensuring that data processing activities in France comply with the GDPR (General Data Protection Regulation, EU 2016/679) and its French implementing legislation. CNIL has powers of investigation, sanction and guidance, and issues binding authorisations for certain categories of sensitive data processing, including health and genetic data.

CNIL occupies a central position in the French research data ecosystem: virtually any research project involving personal health data, biological samples or genomic data requires either a CNIL authorisation or a declaration of conformity to a CNIL reference methodology before data collection or processing can begin.

## Role in Health and Research Data

Health data is a special category under GDPR (Article 9) and requires explicit legal basis and, in France, specific CNIL oversight. CNIL has developed a set of reference methodologies (Méthodologies de Référence, MR) that define standard conditions under which research involving personal health data may proceed without individual authorisation, provided the study conforms strictly to the methodology. Studies that do not conform to a reference methodology require an individual CNIL authorisation, which involves a formal dossier and review process, and in some cases a prior opinion from the CESREES (Comité Ethique et Scientifique pour les Recherches, les Etudes et les Evaluations dans le domaine de la Santé).

## Relationship to Health Data Hub and SNDS

Access to the [[Platforms/SNDS\|SNDS]] via the [[Platforms/Health Data Hub\|Health Data Hub]] is conditional on CNIL authorisation or conformity to the relevant reference methodology for SNDS-based research. The [[Platforms/Health Data Hub\|Health Data Hub]] operates under a CNIL-approved framework and acts as a trusted intermediary, but individual research projects accessing [[Platforms/SNDS\|SNDS]] data through the platform must still obtain their own CNIL clearance. CNIL audits [[Platforms/Health Data Hub\|Health Data Hub]] operations and has previously issued formal notices regarding data hosting arrangements.

## Relationship to Biobanks and Genomics

[[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] and all French biobanks operating under the [[Governance/Code de la Sante Publique\|Code de la Sante Publique]] must comply with CNIL requirements for the collection, storage and reuse of biological samples and associated personal data. Genomic data, as a special subcategory of health data, is subject to specific reference methodology requirements or individual authorisation. Data transfers to international repositories such as [[Platforms/EGA\|EGA]] or [[Platforms/dbGaP\|dbGaP]] require additional CNIL consideration under GDPR Chapter V provisions on international data transfers.

## Relationship to GDPR and EHDS

CNIL is France's designated supervisory authority under GDPR and participates in the European Data Protection Board (EDPB), which coordinates enforcement across EU member states. In the context of the [[Governance/EHDS\|EHDS]] (European Health Data Space), CNIL will play a role in overseeing French compliance with the secondary use provisions of the regulation, working alongside the [[Platforms/Health Data Hub\|Health Data Hub]] in its role as the candidate French Health Data Access Body (HDAB).

## Relationship to ANS and Code de la Santé Publique

CNIL works in close coordination with [[Governance/ANS\|ANS]] on health IT standardisation and data security requirements. The [[Governance/Code de la Sante Publique\|Code de la Sante Publique]] provides the legislative framework within which CNIL operates for health research, defining the categories of research that require ethics committee approval (CPP or CESREES) alongside CNIL clearance.

## Connections

- Oversees: [[Platforms/Health Data Hub\|Health Data Hub]], [[Platforms/SNDS\|SNDS]], [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]], all French health research data processing
- GDPR supervisory authority relevant to: [[Platforms/EGA\|EGA]] data transfers, [[Platforms/dbGaP\|dbGaP]] data transfers, [[Standards/OMOP CDM\|OMOP CDM]] deployments at [[Governance/AP-HP\|AP-HP]]
- Coordinates with: [[Governance/ANS\|ANS]], [[Platforms/Health Data Hub\|Health Data Hub]], CESREES, CPP (Comités de Protection des Personnes)
- Legislative basis: [[Governance/Code de la Sante Publique\|Code de la Sante Publique]], Loi Informatique et Libertés, GDPR
- European coordination: European Data Protection Board (EDPB)
- Relevant to: [[Governance/EHDS\|EHDS]], [[Actors/iGENSEQ\|iGENSEQ]], [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]], [[Actors/DAC\|DAC]]

## Resources

- https://www.cnil.fr