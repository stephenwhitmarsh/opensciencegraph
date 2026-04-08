---
{"dg-publish":true,"permalink":"/moc/","tags":["MOC","gardenEntry"],"dg-note-properties":{"type":"MOC","aliases":["Open Science Hub","Open Science Neuroscience Index"],"tags":["MOC","gardenEntry"]}}
---


---

# Map of Content

This map is a relational index of the **open science** ecosystem for neuroscience, including open science frameworks, data standards, platforms, infrastructure and working groups. The goal is to disambiguate the field by showing dependencies and convergences across actors, domains and research initiatives. While initially overwhelming, the graph can be explored with detailed descriptions in each node. The original focus has been on [[Actors/Paris Brain Institute\|Paris Brain Institute]]'s operational context (explaining its node centrality). However, the network can be extended beyond its direct environment and include standards, policies and partners who engage in open neuroscience. In open science the saying certainly goes:

> *There are no strangers here, just friends you haven't met yet*. - W.B. Yeats

What you see is an [Obsidian](https://obsidian.md/) vault, with the website published to Vercel via my public [github repository](https://github.com/stephenwhitmarsh/opensciencegraph) using the [Digital Garden community plugin](https://docs.forestry.md/). If you want to contribute or make a correction or suggestion, please [email me](mailto:stephen.whitmarsh@icm-institute.org).

---

## Index

The graph is organised across four directories, each with a dedicated sub-MOC with a full alphabetical index of its nodes.

- [[Actors/_Actors\|_Actors]] — consortia, institutes, initiatives, biobanks and ICM core facilities (33 nodes)
- [[Standards/_Standards\|_Standards]] — data format standards, terminologies, ontologies and metadata frameworks (47 nodes)
- [[Platforms/_Platforms\|_Platforms]] — repositories, data platforms and clinical data capture systems (27 nodes)
- [[Governance/_Governance\|_Governance]] — national and European infrastructures, policies, working groups and frameworks (55 nodes)

---
## Frontmatter Schema

Every node uses a lean, non-redundant YAML schema. Only two semantic tags exist, marking ICM's operational relationship to a node:

| Tag | Meaning |
|---|---|
| `icm/uses` | ICM operationally uses this standard, platform, or tool |
| `icm/participates` | ICM is an active member or participant in this body |

**Controlled vocabularies:**

`type:` — `standard` \| `terminology` \| `framework` \| `platform` \| `repository` \| `infrastructure` \| `facility` \| `institute` \| `consortium` \| `initiative` \| `working-group` \| `policy` \| `biobank`

`domain:` — `neuroimaging` \| `electrophysiology` \| `clinical` \| `genomics` \| `multimodal` \| `bioimaging` \| `computational` \| `behavior` \| `health`

`scope:` — `french` \| `european` \| `international`

**Graph view group queries** (Settings → Graph view → Groups → `+`):

| Group | Query |
|---|---|
| Institutes | `[type:institute]` |
| Consortia & initiatives | `[type:consortium] OR [type:initiative]` |
| Standards & terminologies | `[type:standard] OR [type:terminology]` |
| Frameworks & principles | `[type:framework] OR [type:policy]` |
| Repositories & platforms | `[type:repository] OR [type:platform]` |
| Core facilities | `[type:facility]` |
| Infrastructure & biobanks | `[type:infrastructure] OR [type:biobank]` |
| Working groups | `[type:working-group]` |
| ICM uses | `[tags:icm/uses]` |
| ICM participates | `[tags:icm/participates]` |
| French scope | `[scope:french]` |
| European scope | `[scope:european]` |

## Key Structural Relationships

```
ICM ──hosts──────────► CATI ──part of──► France Life Imaging
ICM ──hosts──────────► CENIR ──part of──► France Life Imaging
ICM ──hosts──────────► iGENSEQ ──deposits──► NCBI GEO (open) / EGA (controlled)
ICM ──hosts──────────► DAC ──uses──► IFB (NNCR); DAC part of MUDIS4LS initiative
ICM ──hosts──────────► Banque ADN et Cellules ──connects──► BBMRI-ERIC
ICM ──affiliated────► CNRS, Inserm, AP-HP, Sorbonne
ICM ──member of──────► EBRAINS, ENIGMA, GT-GeDeM
ICM ──member of──────► NeurATRIS ──French node of──► EATRIS
ICM ──founding member─► CURE-ND ──partners───► DZNE, UK DRI, Mission Lucidity
CURE-ND ──framework───► JPND ──participants──► ICM, DZNE, UK DRI
ICM ──participant in─► MUDIS4LS ──managed by──► IFB
ICM ──peer Paris────► Institut Pasteur, Institut Curie, Institut de Myologie

BIDS ──governed──────► INCF ──endorses──► NWB, HED, NIDM, NeuroML
BIDS ──requires──────► NIfTI (MRI/PET image format)
NIfTI ──companion───► CIFTI (surface+volume cortical data)
BIDS ──required by──► OpenNeuro, EBRAINS, DANDI, CONP, BrainLife.io, CATI

NWB ──archived on───► DANDI Archive ──funded by──► NIH BRAIN Initiative
DANDI ──depositors──► IBL (Brain Wide Map), Allen Institute

OME-TIFF/NGFF ──governed──► OME ──deploys──► OMERO
OMERO ──metadata────► REMBI, QUAREP-LiMi
France BioImaging ──nodes──► Institut Pasteur, Institut Curie
GT-GeDeM ──counterpart──► QUAREP-LiMi (international equivalent)

EBRAINS ──successor─► Human Brain Project ──part of──► EOSC
EOSC ──integrates───► ELIXIR, OpenAIRE, EBRAINS

Health Data Hub ──uses──► OMOP CDM, HL7 FHIR, SNOMED CT
Health Data Hub ──EHDS candidate HDAB──► EHDS (EU 2025/327)
AP-HP ──EDS──────────► OMOP CDM ──maps to──► HL7 FHIR, SNOMED CT

VCF ──governed──────► GA4GH ──produces──► Phenopackets ──uses──► HPO
Phenopackets ──links────► clinical phenotype ↔ genomic variant data
MONDO ──harmonises──► ICD-10, ICD-11, ORDO, OMIM
Cognitive Atlas ──annotates──► BIDS task metadata, NeuroVault maps
UBERON ──annotates──► NWB (brain regions), EBRAINS openMINDS
openMINDS ──required for──► EBRAINS data deposit
PROV-O ──extended by──► NIDM ──built on──► BIDS
DCAT ──powers──► Recherche Data Gouv, EOSC catalogue, data.gouv.fr
Dublin Core ──base layer of──► Zenodo, HAL, Recherche Data Gouv metadata

OPIDoR ──implements──► Ouvrir la Science ──mandated by──► ANR, CNRS, Inserm
IFB ──French node──► ELIXIR (ELIXIR-FR)
France BioImaging ──French node──► Euro-BioImaging
INBS ──umbrella────► France BioImaging, France Life Imaging, IFB

FAIR Principles ──promoted by──► GO FAIR, RDA, EOSC, INCF, IFB, ANR
FAIR Principles ──implemented via──► BIDS (neuroimaging), NWB (electrophysiology),
                                     OME File Formats (microscopy), OMOP CDM (clinical),
                                     Recherche Data Gouv (French research data)
```


---

## Dataview queries

Copy the following dataview code blocks in Obsidian:

All `icm/uses` nodes:
```dataview
TABLE type, scope, domain, founded
FROM "Open_Science_Neuroscience"
WHERE contains(tags, "icm/uses")
SORT type ASC
```

All `icm/participates` nodes:
```dataview
TABLE type, scope, founded
FROM "Open_Science_Neuroscience"
WHERE contains(tags, "icm/participates")
SORT type ASC
```

All ontologies and terminologies:
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/Standards"
WHERE type = "terminology" OR type = "framework"
SORT type ASC
```

All format standards:
```dataview
TABLE domain, founded
FROM "Open_Science_Neuroscience/Standards"
WHERE type = "standard"
SORT domain ASC
```

French governance nodes:
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/Governance"
WHERE scope = "french"
SORT type ASC
```

European governance nodes:
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/Governance"
WHERE scope = "european"
SORT type ASC
```

Working groups and frameworks:
```dataview
TABLE scope, domain, founded
FROM "Open_Science_Neuroscience/Governance"
WHERE type = "working-group" OR type = "framework" OR type = "initiative"
SORT scope ASC
```

---

## Vault Statistics

| Folder       | Contents                                                    | Count   |
| ------------ | ----------------------------------------------------------- | ------- |
| `Actors`     | Consortia, institutes, initiatives, projects, software orgs | 33      |
| `Standards`  | All standards, formats, terminologies, ontologies           | 47      |
| `Platforms`  | Repositories, platforms, data infrastructure                | 27      |
| `Governance` | Infrastructure, policies, frameworks, working groups        | 55      |
| **Total**    |                                                             | **162** |

## TODO

- Add link ICM - IFB (DAC as participating platform)
- Resolve OBI name collision: `Actors/OBI.md` (Ontario Brain Institute) and `Standards/OBI.md` (Ontology for Biomedical Investigations) will produce ambiguous links in Obsidian; consider renaming one