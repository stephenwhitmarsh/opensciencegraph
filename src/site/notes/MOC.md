---
{"dg-publish":true,"permalink":"/moc/","tags":["MOC","gardenEntry"],"dg-note-properties":{"type":"MOC","aliases":["Open Science Hub","Open Science Neuroscience Index"],"tags":["MOC","gardenEntry"]}}
---

---

# Map of Content

This page maps the **open science** ecosystem for neuroscience: the frameworks, data standards, platforms, infrastructure and working groups that together make up the field. The aim is to make the landscape navigable by making explicit the dependencies and convergences between its many actors. The graph is anchored at the [[Actors/Paris Brain Institute\|Paris Brain Institute]] and its French and European research infrastructure context, but extends outward to cover the broader international open neuroscience ecosystem and is open to further expansion.

A few structural axes orient the graph: [[Actors/Paris Brain Institute\|Paris Brain Institute]] sits within a set of French national infrastructures ([[Governance/France Life Imaging\|France Life Imaging]], [[Governance/France BioImaging\|France BioImaging]], [[Governance/IFB\|IFB]], [[Governance/NeurATRIS\|NeurATRIS]]) that connect upward to their European counterparts ([[Governance/Euro-BioImaging\|Euro-BioImaging]], [[Governance/ELIXIR\|ELIXIR]], [[Governance/EATRIS\|EATRIS]], [[Governance/EOSC\|EOSC]]). On the standards side, [[Standards/BIDS\|BIDS]] and [[Standards/NWB\|NWB]] form the spine of open neuroimaging and neurophysiology data, implemented across repositories such as [[Platforms/OpenNeuro\|OpenNeuro]], [[Platforms/DANDI Archive\|DANDI Archive]] and [[Platforms/EBRAINS\|EBRAINS]]. In the clinical domain, [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/HL7 FHIR\|HL7 FHIR]] and [[Standards/SNOMED CT\|SNOMED CT]] are the interoperability standards connecting [[Governance/AP-HP\|AP-HP]], the [[Governance/Health Data Hub\|Health Data Hub]] and the [[Governance/EHDS\|EHDS]].


---

## Index

The graph is organised across four directories, each with a dedicated sub-MOC with a full alphabetical index of its nodes.

- [[Actors/_Actors\|_Actors]] — consortia, institutes, initiatives, biobanks and ICM core facilities
- [[Standards/_Standards\|_Standards]] — data format standards, terminologies, ontologies and metadata frameworks
- [[Platforms/_Platforms\|_Platforms]] — repositories, data platforms and clinical data capture systems
- [[Governance/_Governance\|_Governance]] — national and European infrastructures, policies, working groups and frameworks

---

## Frontmatter Schema

Every node uses a lean, non-redundant YAML frontmatter schema. The following fields and values are used:

| Field                    | Values                                                                                                                                                            |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                   | `standard` `terminology` `framework` `platform` `repository` `infrastructure` `facility` `institute` `consortium` `initiative` `working-group` `policy` `biobank` |
| `domain`                 | `neuroimaging` `electrophysiology` `clinical` `genomics` `multimodal` `bioimaging` `computational` `behavior` `health`                                            |
| `scope`                  | `french` `european` `international`                                                                                                                               |
| `tags: icm/uses`         | ICM operationally uses this standard, platform or tool                                                                                                            |
| `tags: icm/participates` | ICM is an active member or participant in this body                                                                                                               |

---
## Contributing

The graph is built as an [Obsidian](https://obsidian.md/) vault, published [here](https://publish.obsidian.md/openscience), and openly available in the [git repository](https://gitlab.com/icm-institute/dac/opensciencegraph). Contributions, corrections and suggestions are welcome — open an issue or pull request there, or [email me](mailto:stephen.whitmarsh@icm-institute.org) directly. In open science perhaps more than anywhere else, this quote by W.B. Yeats rings true:

> *There are no strangers here, just friends you haven't met yet*

