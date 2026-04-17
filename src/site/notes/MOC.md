---
{"dg-publish":true,"permalink":"/moc/","tags":["MOC","gardenEntry"],"dg-note-properties":{"type":"MOC","aliases":["Open Science Hub","Open Science Neuroscience Index"],"tags":["MOC","gardenEntry"]}}
---


# Map of Content

This page maps the **open science** ecosystem for neuroscience: the frameworks, data standards, platforms, infrastructure, initiatives and working groups that together make up the field. The aim is to make the landscape navigable by making explicit the dependencies and convergences between its many nodes. The graph is anchored at the [[Actors/Paris Brain Institute\|Paris Brain Institute]] and its French and European research infrastructure context, but extends outward to cover the broader international open neuroscience ecosystem and is open to further expansion.

A few structural axes orient the graph:

**French-to-European infrastructure.** [[Actors/Paris Brain Institute\|Paris Brain Institute]] sits within a set of French national infrastructures ([[Governance/France Life Imaging\|France Life Imaging]], [[Governance/France BioImaging\|France BioImaging]], [[Governance/IFB\|IFB]], [[Governance/NeurATRIS\|NeurATRIS]]) that connect upward to their European counterparts ([[Governance/Euro-BioImaging\|Euro-BioImaging]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/EATRIS\|EATRIS]], [[Governance/EOSC\|EOSC]]). The labelling and quality framework for [[Actors/Paris Brain Institute\|ICM]]'s own platforms ([[Actors/CENIR\|CENIR]], [[Actors/iGENSEQ\|iGENSEQ]], [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]]) runs through [[Governance/IBiSA\|IBiSA]], which feeds into the [[Governance/INBS\|INBS]] umbrella.

**Neuroimaging and neurophysiology standards.** [[Standards/BIDS\|BIDS]] and [[Standards/NWB\|NWB]] form the spine of open neuroimaging and neurophysiology data, governed by [[Actors/INCF\|INCF]] and implemented across repositories such as [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/DANDI Archive\|DANDI Archive]], and [[Platforms/EBRAINS\|EBRAINS]]. [[Actors/CATI\|CATI]] handles multisite MRI harmonisation for [[Actors/Paris Brain Institute\|ICM]]-associated cohorts such as MEMENTO, INSIGHT-preAD and iShare, with [[Actors/CENIR\|CENIR]] as [[Actors/Paris Brain Institute\|ICM]]'s acquisition platform.

**Clinical data and health interoperability.** [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]], and [[Standards/SNOMED CT\|SNOMED CT]] are the interoperability standards connecting [[Governance/AP-HP\|AP-HP]] and the [[Platforms/EDS AP-HP\|EDS AP-HP]], the [[Platforms/Health Data Hub\|Health Data Hub]], the [[Platforms/SNDS\|SNDS]], and the [[Governance/EHDS\|EHDS]]. The OMOP vocabulary draws on [[Standards/ICD-10\|ICD-10]], [[Standards/LOINC\|LOINC]], [[Standards/RxNorm\|RxNorm]], and [[Standards/CCAM\|CCAM]] as source terminologies.

**Genomics and single-cell data.** [[Actors/iGENSEQ\|iGENSEQ]] produces sequencing data deposited in [[Platforms/NCBI GEO\|NCBI GEO]] (open) or [[Platforms/EGA\|EGA]]/[[Platforms/dbGaP\|dbGaP]] (controlled access), governed by [[Actors/GA4GH\|GA4GH]] standards for data access and interoperability. Single-cell data aligns with [[Standards/AnnData\|AnnData]] and [[Standards/Cell Ontology\|Cell Ontology]], with [[Actors/BICAN\|BICAN]] providing the international cell atlas reference.

**Open science policy.** [[Governance/Ouvrir la Science\|Ouvrir la Science]] drives French open science mandates, implemented through [[Governance/ANR Open Science Policy\|ANR Open Science Policy]], [[Governance/CNRS Open Science\|CNRS Open Science]], and [[Governance/Inserm Open Science\|Inserm Open Science]], directing deposits to [[Platforms/HAL\|HAL]] (publications), [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] (data), and [[Platforms/Software Heritage\|Software Heritage]] (code), with [[Platforms/OPIDoR\|OPIDoR]] providing the DMP infrastructure. These align upward to [[Governance/EOSC\|EOSC]] and [[Platforms/OpenAIRE\|OpenAIRE]] at the European level.

**Rare disease and phenotyping.** [[Standards/HPO\|HPO]] and [[Standards/ORDO\|ORDO]] are the primary phenotyping standards for rare neurological disease. [[Standards/HPO\|HPO]] is used for phenotype annotation in controlled-access genomic repositories ([[Platforms/EGA\|EGA]], [[Platforms/dbGaP\|dbGaP]]) and linked through [[Standards/Phenopackets\|Phenopackets]] for genotype-phenotype association. [[Standards/MONDO\|MONDO]] harmonises disease classifications across [[Standards/ICD-10\|ICD-10]], [[Standards/OMIM\|OMIM]], and [[Standards/ORDO\|ORDO]] into a single hierarchy. [[Governance/BBMRI-ERIC\|BBMRI-ERIC]] promotes [[Standards/Phenopackets\|Phenopackets]] and [[Standards/OMOP CDM\|OMOP CDM]] for cross-biobank discoverability, a network in which [[Actors/Paris Brain Institute\|ICM]]'s [[Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] participates as a CRB (Centre de Ressources Biologiques, biological resource centre).

**International neuroscience community.** [[Actors/INCF\|INCF]] coordinates standards governance across [[Governance/BIDS Steering Group\|BIDS Steering Group]], [[Governance/NWB Working Group\|NWB Working Group]], and [[Governance/INCF Working Groups\|INCF Working Groups]]. [[Actors/Paris Brain Institute\|ICM]] participates in [[Actors/ENIGMA Consortium\|ENIGMA Consortium]] for federated neuroimaging meta-analysis and in [[Governance/CURE-ND\|CURE-ND]] and [[Governance/JPND\|JPND]] for European neurodegeneration research alliances, with counterpart institutes including [[Actors/DZNE\|DZNE]], [[Actors/UK DRI\|UK DRI]], and [[Actors/Human Brain Project\|Human Brain Project]]/[[Platforms/EBRAINS\|EBRAINS]].


## Index

The graph is organised across four directories, each with a dedicated sub-MOC with a full alphabetical index of its nodes.

- [[Actors/_Actors\|_Actors]] — consortia, institutes, initiatives, biobanks and ICM core facilities
- [[Standards/_Standards\|_Standards]] — data format standards, terminologies, ontologies and metadata frameworks
- [[Platforms/_Platforms\|_Platforms]] — repositories, data platforms and clinical data capture systems
- [[Governance/_Governance\|_Governance]] — national and European infrastructures, policies, working groups and frameworks

## Frontmatter Schema

Every node uses a lean, non-redundant YAML frontmatter schema. The following fields and values are used:

| Field                    | Values                                                                                                                                                            |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                   | `standard` `terminology` `framework` `platform` `repository` `infrastructure` `facility` `institute` `consortium` `initiative` `working-group` `policy` `biobank` |
| `domain`                 | `neuroimaging` `electrophysiology` `clinical` `genomics` `multimodal` `bioimaging` `computational` `behavior` `health`                                            |
| `scope`                  | `french` `european` `international`                                                                                                                               |
| `tags: icm/uses`         | ICM operationally uses this standard, platform or tool                                                                                                            |
| `tags: icm/participates` | ICM is an active member or participant in this body                                                                                                               |

## Contributing

The graph is built as an [Obsidian](https://obsidian.md/) vault, published [here](https://publish.obsidian.md/openscience), and openly available in the [git repository](https://gitlab.com/icm-institute/dac/opensciencegraph). Contributions, corrections and suggestions are welcome. Just open an issue or pull request there, or [email me](mailto:stephen.whitmarsh@icm-institute.org) directly. In open science perhaps more than anywhere else, this quote by W.B. Yeats rings true:

> *There are no strangers here, just friends you haven't met yet*

