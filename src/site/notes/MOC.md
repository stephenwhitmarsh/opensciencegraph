---
{"dg-publish":true,"permalink":"/moc/","tags":["MOC","gardenEntry"],"dg-note-properties":{"type":"MOC","aliases":["Open Science Hub","Open Science Neuroscience Index"],"tags":["MOC","gardenEntry"]}}
---

# Map of Content

This map is a relational index of the **open science** ecosystem for neuroscience, including open science frameworks, data standards, platforms, infrastructure and working groups. The goal is the disambiguate the field by showing dependencies and convergences across actors, domains and research initiatives. While initially overwhelming, the graph can be explored with detailed descriptions in each node.

The original focus is on [[00_Core/Paris Brain Institute\|Paris Brain Institute]]'s operational context, explaining it's node centrality. However, the network can be extended beyond its direct connections, as the main limitation in my understanding and memory.

The graph is made with Obsidian, with the website published to Vercel from my public [github repository](https://github.com/stephenwhitmarsh/opensciencegraph) using the Digital Garden plugin. For now, to contribute please [email me](mailto:stephen.whitmarsh@icm-institute.org) directly rather than via pull-requests. The latter will be difficult to manage due to the interconnected nature of the graph. However, if you want to give it a shot, you can find the gitlab repository here.

Last updated: 2026-04-08

---

## Core

- [[00_Core/Paris Brain Institute\|Paris Brain Institute]]

---

## Actors — Consortia, Institutes and Projects

*All in `01_Actors`. Filter by `type: consortium / institute / initiative / biobank` and `scope`.*

### Neuroscience — International
- [[01_Actors/DZNE\|DZNE]] — German Centre for Neurodegenerative Diseases; CURE-ND founding partner; EBRAINS contributor; JPND participant
- [[01_Actors/UK DRI\|UK DRI]] — UK Dementia Research Institute; CURE-ND founding partner; JPND; FAIR data policy
- [[01_Actors/Mission Lucidity\|Mission Lucidity]] — imec/KU Leuven/VIB/UZ Leuven neurotechnology consortium (Belgium); CURE-ND founding partner
- [[01_Actors/The Florey\|The Florey]] — largest brain research institute in southern hemisphere (Melbourne); ENIGMA-Epilepsy; ARDC ecosystem
- [[01_Actors/Mount Sinai Neuroscience\|Mount Sinai Neuroscience]] — Friedman Brain Institute / Nash Family Dept; CommonMind + PsychENCODE lead site; ENIGMA
- [[01_Actors/INCF\|INCF]] — International Neuroinformatics Coordinating Facility; governs BIDS, endorses NWB/HED/NIDM
- [[01_Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]] — co-founded NWB; open-access brain atlases and electrophysiology datasets
- [[01_Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]] — primary US funder of open neuroscience data infrastructure (DANDI, NWB mandate)
- [[01_Actors/Human Connectome Project\|Human Connectome Project]] — landmark open MRI dataset; produced CIFTI format
- [[01_Actors/IBL\|IBL]] — International Brain Laboratory; fully open data/code model; Brain Wide Map on DANDI
- [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] — federated meta-analysis across 45+ working groups; ICM participates
- [[01_Actors/ADNI\|ADNI]] — Alzheimer's Disease Neuroimaging Initiative; multisite open clinical neuroimaging cohort
- [[01_Actors/Donders Institute\|Donders Institute]] — European open-data pioneer; FieldTrip toolbox; mandatory data sharing policy
- [[01_Actors/TOSI\|TOSI]] — Tanenbaum Open Science Institute (Montreal); first institute to adopt open science as core value
- [[01_Actors/CONP\|CONP]] — Canadian Open Neuroscience Platform; federated BIDS portal; DataLad backend
- [[01_Actors/OBI\|OBI]] — Ontario Brain Institute; FAIR neuroinformatics platform Brain-CODE; CONP founding sponsor
- [[01_Actors/ReproNim\|ReproNim]] — reproducibility tools (NIDM, ReproIn, DataLad); NIH-funded

### Bioimaging
- [[01_Actors/OME\|OME]] — Open Microscopy Environment; produces OME-TIFF, OME-NGFF, Bio-Formats, OMERO

### Paris Peer Institutions
- [[01_Actors/Institut Pasteur\|Institut Pasteur]] — founding France BioImaging node; Icy software; strong open science policy (90% OA)
- [[01_Actors/Institut Curie\|Institut Curie]] — PICT-IBiSA imaging platform; France BioImaging node; QUAREP-LiMi participation
- [[01_Actors/Sorbonne Universite\|Sorbonne Universite]] — founding governing member of ICM; Faculty of Medicine at Pitié-Salpêtrière; strong open science policy
- [[01_Actors/Institut de Myologie\|Institut de Myologie]] — international reference centre for neuromuscular diseases; co-located at Pitié-Salpêtrière; founding NeurATRIS node
- [[01_Actors/Banque ADN et Cellules\|Banque ADN et Cellules]] — ICM DNA and cell biobank; BBMRI-ERIC; HPO/ORDO phenotyping; links to iGENSEQ and CATI
- [[01_Actors/iGENSEQ\|iGENSEQ]] — ICM NGS platform; RNA-seq, scRNA-seq, WGS/WES; data → NCBI GEO / EGA / EVA
- [[01_Actors/CENIR\|CENIR]] — ICM neuroimaging centre; 3T MRI ×2, PET-MRI, MEG; FLI node; data via CATI
- [[01_Actors/DAC\|DAC]] — ICM Data Analysis Core; bioinformatics, statistics, FAIR workflows; IFB/OPIDoR interface
- [[01_Actors/EMBL\|EMBL]] — European Molecular Biology Laboratory; operates EMBL-EBI (EGA, EVA, IDR, ENA, Ensembl)

### Genomics
- [[01_Actors/GA4GH\|GA4GH]] — Global Alliance for Genomics and Health; governs VCF, Phenopackets, Beacon, DRS, DUO
- [[01_Actors/UK Biobank\|UK Biobank]] — 500,000 participants; 50,000+ brain MRI; genomics; RAP cloud platform
- [[01_Actors/BICAN\|BICAN]] — BRAIN Initiative Cell Atlas Network; comprehensive multi-resolution mammalian brain cell atlas
- [[01_Actors/OHDSI\|OHDSI]] — Observational Health Data Sciences and Informatics; maintains [[02_Standards/OMOP CDM\|OMOP CDM]]; ATLAS, ACHILLES, HADES tools; 700M+ patient records globally

---

## Standards, Terminologies and Ontologies

*All in `02_Standards`. Filter by `type` in Dataview: `standard` | `terminology` | `framework`.*

### Neuroimaging Formats
- [[02_Standards/DICOM\|DICOM]] — universal clinical imaging format; source format converted to NIfTI/BIDS
- [[02_Standards/NIfTI\|NIfTI]] — universal processed neuroimaging format (.nii/.nii.gz); pivot between DICOM and BIDS
- [[02_Standards/CIFTI\|CIFTI]] — surface+volume (greyordinate) format for cortical data; developed by HCP; complements NIfTI
- [[02_Standards/BIDS\|BIDS]] — Brain Imaging Data Structure; de facto community standard for neuroimaging datasets

### Neurophysiology
- [[02_Standards/NWB\|NWB]] — Neurodata Without Borders; community standard for electrophysiology and calcium imaging
- [[02_Standards/HED\|HED]] — Hierarchical Event Descriptors; structured event annotation integrated into BIDS/NWB
- [[02_Standards/SPARC SDS\|SPARC SDS]] — SPARC Data Structure; NIH SPARC programme standard for peripheral nervous system data

### Microscopy
- [[02_Standards/OME File Formats\|OME File Formats]] — OME file formats: archival (OME-TIFF) and cloud-native (OME-Zarr)
- [[02_Standards/REMBI\|REMBI]] — Recommended Metadata for Biological Images; community metadata framework for bioimaging

### Computational Neuroscience
- [[02_Standards/NeuroML\|NeuroML]] — simulator-independent XML format for computational neuron/network models

### Neuroimaging Annotation and Semantics
- [[02_Standards/NIDM\|NIDM]] — Neuroimaging Data Model; W3C PROV-based provenance for neuroimaging experiments
- [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] — ontology of cognitive processes and tasks; used by NeuroVault and BIDS
- [[02_Standards/UBERON\|UBERON]] — cross-species anatomy ontology; brain region annotation in EBRAINS, NWB, Allen Institute
- [[02_Standards/openMINDS\|openMINDS]] — EBRAINS metadata framework; required for EBRAINS data deposit

### Clinical Health Standards
- [[02_Standards/OMOP CDM\|OMOP CDM]] — OHDSI Common Data Model; federated observational health research
- [[02_Standards/HL7 FHIR\|HL7 FHIR]] — Fast Healthcare Interoperability Resources; mandated by EHDS for EHR exchange
- [[02_Standards/openEHR\|openEHR]] — semantic EHR specification using archetypes and templates
- [[02_Standards/CDISC\|CDISC]] — clinical trial data standards (SDTM, ADaM, CDASH); regulatory submissions

### Clinical Terminologies
- [[02_Standards/SNOMED CT\|SNOMED CT]] — comprehensive clinical terminology; core vocabulary in OMOP CDM and HL7 FHIR
- [[02_Standards/ICD-10\|ICD-10]] — WHO disease classification; CIM-10 is the French version used in SNDS and AP-HP billing
- [[02_Standards/ICD-11\|ICD-11]] — WHO updated classification (2022); France in transition; improved neuroscience coverage
- [[02_Standards/LOINC\|LOINC]] — standard for lab tests, biomarkers, clinical observations
- [[02_Standards/CCAM\|CCAM]] — French national procedure classification; present in SNDS and AP-HP PMSI billing
- [[02_Standards/MedDRA\|MedDRA]] — adverse event coding for clinical trial regulatory submissions (EMA, ANSM)
- [[02_Standards/MeSH\|MeSH]] — NLM controlled vocabulary for PubMed indexing and ClinicalTrials.gov; ~30,000 biomedical descriptors
- [[02_Standards/OMIM\|OMIM]] — Online Mendelian Inheritance in Man; gene-disease relationships; MIM numbers; rare neurological diseases

### Disease Ontologies
- [[02_Standards/MONDO\|MONDO]] — Monarch Disease Ontology; harmonises ICD-10, OMIM, ORDO into one hierarchy
- [[02_Standards/ORDO\|ORDO]] — Orphanet Rare Disease Ontology; European standard for rare neurological diseases
- [[02_Standards/HPO\|HPO]] — Human Phenotype Ontology; 18,000+ phenotypic abnormality terms for rare disease genomics
- [[02_Standards/ERN Vocabularies\|ERN Vocabularies]] — ERN-RND and ERN-EpiCARE patient registry terminologies; ORDO+HPO+OMOP CDM
- [[02_Standards/ADO\|ADO]] — Alzheimer’s Disease Ontology; biomarkers, staging, genetics for Alzheimer’s cohorts

### Genomics Standards
- [[02_Standards/VCF\|VCF]] — Variant Call Format; universal format for genomic variant data
- [[02_Standards/Phenopackets\|Phenopackets]] — GA4GH standard linking clinical phenotypes (HPO) to genomic data (ISO/TS 5435)
- [[02_Standards/ClinVar\|ClinVar]] — NCBI authoritative database of clinical variant interpretations; pathogenicity classifications
- [[02_Standards/GO\|GO]] — Gene Ontology; biological process, molecular function, cellular component; used in transcriptomics
- [[02_Standards/NBO\|NBO]] — Neurobehavior Ontology; behavioural phenotypes in humans and model organisms
- [[02_Standards/ChEBI\|ChEBI]] — Chemical Entities of Biological Interest; drugs, metabolites, neurotransmitters (EMBL-EBI)
- [[02_Standards/RxNorm\|RxNorm]] — NLM drug terminology; clinical drug names and identifiers; primary drug vocabulary in OMOP CDM
- [[02_Standards/NCIT\|NCIT]] — NCI Thesaurus; cancer and clinical research terminology; used in CDISC SDTM submissions
- [[02_Standards/Cell Ontology\|Cell Ontology]] — OBO Foundry ontology for cell types; required for single-cell data annotation (CELLxGENE, BICAN)
- [[02_Standards/AnnData\|AnnData]] — de facto standard format (h5ad) for single-cell genomics data; Scanpy/scverse ecosystem

### Research Data Management Standards
- [[02_Standards/PROV-O\|PROV-O]] — W3C Provenance Ontology; foundation for NIDM and DataLad provenance tracking
- [[01_Actors/OBI\|OBI]] — Ontology for Biomedical Investigations; formal study protocol description
- [[02_Standards/DCAT\|DCAT]] — W3C Data Catalog Vocabulary; powers EOSC and Recherche Data Gouv discoverability
- [[02_Standards/Dublin Core\|Dublin Core]] — 15-element base metadata standard; present in all repositories (Zenodo, HAL)

---

## Platforms and Repositories

### Neuroimaging
- [[03_Platforms/OpenNeuro\|OpenNeuro]] — leading open BIDS repository (MRI, EEG, MEG, iEEG, PET); CC0/PDDL; DataLad
- [[03_Platforms/NeuroVault\|NeuroVault]] — unthresholded statistical maps, parcellations, atlases; meta-analysis via Neurosynth
- [[03_Platforms/DANDI Archive\|DANDI Archive]] — NIH BRAIN Initiative archive for neurophysiology (NWB required)
- [[03_Platforms/BrainLife.io\|BrainLife.io]] — cloud platform for BIDS/NWB analysis with provenance tracking
- [[03_Platforms/EBRAINS\|EBRAINS]] — EU brain research infrastructure; BIDS + NWB + openMINDS; ICM is member
- [[03_Platforms/LORIS\|LORIS]] — open-source data management for multisite neuroimaging studies (ADNI, CONP, CATI)
- [[03_Platforms/XNAT\|XNAT]] — DICOM management and pipeline platform; used at EBRAINS member sites
- [[03_Platforms/Neurobagel\|Neurobagel]] — federated participant-level cohort search across BIDS datasets; DataLad backend

### Microscopy and Bioimaging
- [[03_Platforms/IDR\|IDR]] — EMBL-EBI reference image repository (OMERO-based); published microscopy datasets
- [[03_Platforms/OMERO\|OMERO]] — OME's institutional image management platform; deployed at Euro-BioImaging and France BioImaging nodes

### Genomics and Sequence Data
- [[03_Platforms/NCBI GEO\|NCBI GEO]] — primary open-access repository for gene expression and functional genomics data
- [[03_Platforms/EGA\|EGA]] — EMBL-EBI/CRG controlled-access repository for human genomics and phenotypic data
- [[03_Platforms/dbGaP\|dbGaP]] — NIH controlled-access repository for GWAS and human genotype-phenotype data
- [[03_Platforms/EVA\|EVA]] — EMBL-EBI open-access variant archive; short variants and structural variants
- [[03_Platforms/DDBJ\|DDBJ]] — Japanese national sequence database; INSDC partner (mirrors NCBI/ENA)
- [[03_Platforms/NeMO Archive\|NeMO Archive]] — primary BRAIN Initiative / BICAN multi-omics repository; single-cell brain atlas data

### Preprint Infrastructure
- [[03_Platforms/Preprint Servers\|Preprint Servers]] — bioRxiv (life sciences) and medRxiv (clinical research); open access by default; DOI; ORCID

### Clinical Trials
- [[03_Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]] — world's largest clinical trial registry and results database (NLM/NIH)
- [[03_Platforms/VIVLI\|VIVLI]] — global clinical trial individual patient data sharing platform; controlled access enclave
- [[03_Platforms/REDCap\|REDCap]] — secure web-based eCRF and clinical data capture platform; supported at ICM by [[01_Actors/DAC\|DAC]]

### Neuroscience Multiomics
- [[03_Platforms/Brain-CODE\|Brain-CODE]] — OBI neuroinformatics platform; 240+ researchers; LORIS/XNAT/CONP federation; FAIR; multimodal brain disorder data
- [[03_Platforms/Synapse AMP-AD\|Synapse AMP-AD]] — Sage Bionetworks; AMP-AD Knowledge Portal; CommonMind; PsychENCODE; open Alzheimer's + psychiatric brain multiomics

### General Research Data
- [[03_Platforms/OSF\|OSF]] — Open Science Framework / Center for Open Science; pre-registration, data/code sharing, preprints
- [[03_Platforms/Zenodo\|Zenodo]] — CERN/OpenAIRE general-purpose repository; DOIs; recommended for EU-funded projects

---

## Governance, Infrastructure and Frameworks

*All in `04_Governance` (56 nodes). Use `scope` and `type` to filter*

### French (scope: french)
- [[04_Governance/CATI\|CATI]] — Centre d’Acquisition et de Traitement des Images; hosted at ICM; FLI neuroimaging node
- [[04_Governance/France BioImaging\|France BioImaging]] — national cellular imaging infrastructure; French node of Euro-BioImaging; **ICM participates**
- [[04_Governance/France Life Imaging\|France Life Imaging]] — national in vivo imaging infrastructure; CATI is its neuroimaging data node; **ICM participates**
- [[04_Governance/INBS\|INBS]] — umbrella for all French national biology/health infrastructures (FBI, FLI, IFB, BIOBANQUES…)
- [[04_Governance/IFB\|IFB]] — Institut Français de Bioinformatique (ELIXIR-FR); FAIR-Checker; usegalaxy.fr; HPC
- [[04_Governance/OPIDoR\|OPIDoR]] — DMP OPIDoR, Cat OPIDoR, DORANum, JurisDoR; national RDM tools suite
- [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] — national multidisciplinary research data repository; recommended by ANR/CNRS/Inserm
- [[04_Governance/Health Data Hub\|Health Data Hub]] — French national health data platform; SNDS; OMOP CDM; EHDS national HDAB candidate
- [[04_Governance/data.gouv.fr\|data.gouv.fr]] — general French government open data portal; umbrella for Recherche Data Gouv and HDH
- [[04_Governance/AP-HP\|AP-HP]] — Assistance Publique Hôpitaux de Paris; EDS AP-HP (OMOP CDM); ICM partner via Pitié-Salpêtrière
- [[04_Governance/Ouvrir la Science\|Ouvrir la Science]] — French national open science plan (publications, data, software, skills)
- [[04_Governance/CoSO\|CoSO]] — Comité pour la Science Ouverte; coordinates Ouvrir la Science implementation; **ICM participates**
- [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]] — mandates DMP, open access, FAIR deposit for all ANR-funded projects
- [[04_Governance/CNRS Open Science\|CNRS Open Science]] — CNRS institutional open science policy; ICM parent org
- [[04_Governance/Inserm Open Science\|Inserm Open Science]] — Inserm institutional open science policy; ICM parent org
- [[01_Actors/Sorbonne Universite\|Sorbonne Universite]] — founding governing member of ICM; open science policy: mandatory HAL deposit, RDM via OPIDoR
- [[04_Governance/NeurATRIS\|NeurATRIS]] — French translational neuroscience infrastructure; French node of EATRIS; ICM is core member; **ICM participates**
- [[04_Governance/MUDIS4LS\|MUDIS4LS]] — IFB-coordinated FAIR digital infrastructure for French life sciences; multi-omics + imaging integration; **ICM participates**
- [[04_Governance/HAL\|HAL]] — French national open access publication archive; mandatory deposit under ANR/CNRS/Inserm mandates
- [[04_Governance/Software Heritage\|Software Heritage]] — universal software source code archive; French open science mandate for code deposit
- [[04_Governance/Barometre Science Ouverte\|Barometre Science Ouverte]] — French Open Science Monitor; tracks OA rates and FAIR data compliance
- [[04_Governance/ANS\|ANS]] — Agence du Numérique en Santé; French health IT standardisation; SNOMED CT NRC; HL7 FHIR French profiles
- [[04_Governance/Code de la Sante Publique\|Code de la Sante Publique]] — French public health law; governs health data access, biobanking, clinical research

### European (scope: european)
- [[04_Governance/CURE-ND\|CURE-ND]] — DZNE / ICM / Mission Lucidity / UK DRI alliance for neurodegeneration; ICM founding member; **ICM participates**
- [[04_Governance/JPND\|JPND]] — Joint Programme Neurodegenerative Disease Research; transnational funding; links DZNE, UK DRI, ICM
- [[03_Platforms/EBRAINS\|EBRAINS]] — EU flagship brain research infrastructure; successor to Human Brain Project; **ICM participates**
- [[04_Governance/Human Brain Project\|Human Brain Project]] — EU Horizon Flagship (2013–2023); created EBRAINS
- [[04_Governance/EOSC\|EOSC]] — European Open Science Cloud; mandates FAIR for EU-funded research
- [[04_Governance/ELIXIR\|ELIXIR]] — European life science data infrastructure; 23 national nodes; French node = [[04_Governance/IFB\|IFB]]
- [[04_Governance/Euro-BioImaging\|Euro-BioImaging]] — European bioimaging infrastructure; French node = [[04_Governance/France BioImaging\|France BioImaging]]
- [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] — European biobanking infrastructure; OMOP CDM, VCF, Phenopackets
- [[04_Governance/EATRIS\|EATRIS]] — European translational medicine infrastructure; biomarker development; clinical trial support
- [[04_Governance/LifeTime Initiative\|LifeTime Initiative]] — single-cell technologies for disease interception; multi-omics + imaging
- [[04_Governance/ECRIN\|ECRIN]] — European Clinical Research Infrastructure Network; multinational trials; CDISC/OMOP/FHIR
- [[04_Governance/EHDS\|EHDS]] — European Health Data Space Regulation (EU 2025/327); HL7 FHIR mandated; in force March 2025
- [[04_Governance/OpenAIRE\|OpenAIRE]] — EU open science and open access infrastructure; hosts Zenodo
- [[04_Governance/EC Open Science Policy\|EC Open Science Policy]] — Horizon Europe OA mandates, Plan S, EOSC policy; drives all EU open science requirements

### International Frameworks and Principles (scope: international, type: framework/initiative/policy)
- [[04_Governance/ARDC\|ARDC]] — Australian Research Data Commons; national FAIR/RDM infrastructure; EOSC counterpart; RDA partner
- [[04_Governance/HDR UK\|HDR UK]] — Health Data Research UK; UK national health data science institute; FAIR; OMOP CDM; HL7 FHIR; CURE-ND AI/ML workshop participant
- [[04_Governance/FAIR Principles\|FAIR Principles]] — 15 Findable/Accessible/Interoperable/Reusable principles (Wilkinson et al. 2016)
- [[04_Governance/GO FAIR\|GO FAIR]] — international initiative for FAIR implementation; Three-Point FAIRification Framework
- [[04_Governance/RDA\|RDA]] — Research Data Alliance; FAIR Data Maturity Model; 120+ working groups
- [[04_Governance/FORCE11\|FORCE11]] — co-authored FAIR Principles; scholarly communications reform
- [[04_Governance/UNESCO Open Science Recommendation\|UNESCO Open Science Recommendation]] — 2021 global framework for open science policy

### Clinical Research Infrastructure (domain: clinical)
- [[04_Governance/i2b2\|i2b2]] — clinical data warehousing platform; deployed at AP-HP alongside OMOP CDM
- [[04_Governance/YODA Project\|YODA Project]] — Yale Open Data Access; independent third-party clinical trial data sharing (499 trials); influenced NIH data sharing policy; co-founders created medRxiv
- [[04_Governance/TransCelerate\|TransCelerate]] — pharma industry consortium; CDISC standards; trial data sharing

### Working Groups (type: working-group)
- [[04_Governance/BIDS Steering Group\|BIDS Steering Group]] — governs BIDS specification and BEP extension process (under INCF)
- [[04_Governance/NWB Working Group\|NWB Working Group]] — governs NWB specification and NDX extensions (under INCF)
- [[04_Governance/INCF Working Groups\|INCF Working Groups]] — INCF task forces producing BIDS, NWB, HED, NIDM, NeuroML
- [[04_Governance/OHBM Open Science SIG\|OHBM Open Science SIG]] — promotes open science within OHBM; organises Brainhack
- [[04_Governance/RDA Neuroscience IG\|RDA Neuroscience IG]] — bridges RDA data management community with neuroscience standards
- [[04_Governance/QUAREP-LiMi\|QUAREP-LiMi]] — Quality Assessment and Reproducibility for light microscopy; 590+ members; ISO standards
- [[04_Governance/GT-GeDeM\|GT-GeDeM]] — RTmfm/CNRS working group on microscopy data management; **ICM participates**
- [[04_Governance/NIF\|NIF]] — Neuroscience Information Framework; RRID identifiers for research resources; repository registry
- [[04_Governance/GFRN\|GFRN]] — Global Federation of Reproducibility Networks; includes French RFRR network
- [[04_Governance/RDMkit\|RDMkit]] — ELIXIR research data management toolkit; life sciences FAIR guidance; French resources via IFB
- [[04_Governance/Huma-Num\|Huma-Num]] — French national digital humanities infrastructure; DARIAH and CLARIN French node

---

## Quick Reference: Ontologies and Terminologies

*All nodes are in `02_Standards`. Full descriptions in the Standards section above.*

### Which Ontology for Which Task
| Task | Use |
|---|---|
| Code diagnosis from Health Data Hub | [[02_Standards/ICD-10\|ICD-10]] / [[02_Standards/SNOMED CT\|SNOMED CT]] |
| Code AP-HP procedure | [[02_Standards/CCAM\|CCAM]] / [[02_Standards/SNOMED CT\|SNOMED CT]] |
| Code lab result or biomarker | [[02_Standards/LOINC\|LOINC]] |
| Annotate fMRI task events | [[02_Standards/HED\|HED]] + [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] |
| Describe brain regions cross-species | [[02_Standards/UBERON\|UBERON]] |
| Code rare neurological disease | [[02_Standards/ORDO\|ORDO]] + [[02_Standards/HPO\|HPO]] |
| Build OMOP CDM cohort | [[02_Standards/SNOMED CT\|SNOMED CT]] + [[02_Standards/LOINC\|LOINC]] + [[02_Standards/ICD-10\|ICD-10]] |
| Deposit data on EBRAINS | [[02_Standards/openMINDS\|openMINDS]] |
| Deposit data on Recherche Data Gouv | [[02_Standards/Dublin Core\|Dublin Core]] + [[02_Standards/DCAT\|DCAT]] |
| Track analysis provenance | [[02_Standards/PROV-O\|PROV-O]] + [[02_Standards/NIDM\|NIDM]] |
| Code clinical trial adverse events | [[02_Standards/MedDRA\|MedDRA]] |
| Describe study protocol formally | [[01_Actors/OBI\|OBI]] |
| Harmonise disease terms across databases | [[02_Standards/MONDO\|MONDO]] |
| Harmonise rare disease codes | [[02_Standards/ORDO\|ORDO]] ↔ [[02_Standards/MONDO\|MONDO]] ↔ [[02_Standards/HPO\|HPO]] |
| Annotate gene expression / transcriptomics | [[02_Standards/GO\|GO]] |
| Annotate behavioural phenotypes | [[02_Standards/NBO\|NBO]] + [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] |
| Code drug / chemical compound | [[02_Standards/RxNorm\|RxNorm]] + [[02_Standards/ChEBI\|ChEBI]] |
| Code cancer or clinical trial concept | [[02_Standards/NCIT\|NCIT]] + [[02_Standards/MedDRA\|MedDRA]] |
| Code rare neurological disease (ERN registry) | [[02_Standards/ERN Vocabularies\|ERN Vocabularies]] + [[02_Standards/ORDO\|ORDO]] + [[02_Standards/HPO\|HPO]] |
| Annotate PNS / peripheral nerve data | [[02_Standards/SPARC SDS\|SPARC SDS]] |
| Annotate genomic variants | [[02_Standards/VCF\|VCF]] + [[02_Standards/OMIM\|OMIM]] + [[02_Standards/HPO\|HPO]] (via [[02_Standards/Phenopackets\|Phenopackets]]) |
| Search clinical literature | [[02_Standards/MeSH\|MeSH]] (PubMed) |

### Key Ontology Browsers
- OBO Foundry: https://obofoundry.org
- BioPortal: https://bioportal.bioontology.org
- EMBL-EBI OLS: https://www.ebi.ac.uk/ols
- SNOMED CT browser: https://browser.ihtsdotools.org
- LOINC search: https://loinc.org/search/
- Athena OMOP vocabularies: https://athena.ohdsi.org
- Orphanet (ORDO): https://www.orpha.net
- openMINDS docs: https://openminds.ebrains.eu

---

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

## Vault Statistics

| Folder | Contents | Count |
|---|---|---|
| `00_Core` | ICM anchor node | 1 |
| `01_Actors` | Consortia, institutes, initiatives, projects, software orgs | 31 |
| `02_Standards` | All standards, formats, terminologies, ontologies | 45 |
| `03_Platforms` | Repositories, platforms, data infrastructure | 26 |
| `04_Governance` | Infrastructure, policies, frameworks, working groups (french + european + international) | 56 |
| **Total** | | **158** |

*Use `scope: french / european / international` and `type: policy / infrastructure / working-group / framework` to filter within `04_Governance`.*

---

## Frontmatter Schema

Every node uses a lean, non-redundant YAML schema. Only two semantic tags exist, marking ICM's operational relationship to a node:

| Tag | Meaning |
|---|---|
| `icm/uses` | ICM operationally uses this standard, platform, or tool |
| `icm/participates` | ICM is an active member or participant in this body |

**Controlled vocabularies:**

`type:` — `standard` \| `terminology` \| `framework` \| `platform` \| `repository` \| `infrastructure` \| `facility` \| `institute` \| `consortium` \| `initiative` \| `working-group` \| `policy` \| `biobank`

**Graph view group queries** (Settings → Graph view → Groups → `+`):

| Group                     | Query                                     |
| ------------------------- | ----------------------------------------- |
| Institutes                | `[type:institute]`                        |
| Consortia & initiatives   | `[type:consortium] OR [type:initiative]`  |
| Standards & terminologies | `[type:standard] OR [type:terminology]`   |
| Frameworks & principles   | `[type:framework] OR [type:policy]`       |
| Repositories & platforms  | `[type:repository] OR [type:platform]`    |
| Core facilities | `[type:facility]` |
| Infrastructure & biobanks | `[type:infrastructure] OR [type:biobank]` |
| Working groups            | `[type:working-group]`                    |
| ICM uses                  | `[tags:icm/uses]`                         |
| ICM participates          | `[tags:icm/participates]`                 |
| French scope              | `[scope:french]`                          |
| European scope            | `[scope:european]`                        |

`domain:` — `neuroimaging` \| `electrophysiology` \| `clinical` \| `genomics` \| `multimodal` \| `bioimaging` \| `computational` \| `behavior` \| `health`

`scope:` — `french` \| `european` \| `international`

**To query all `icm/uses` nodes:**
```dataview
TABLE type, scope, domain, founded
FROM "Open_Science_Neuroscience"
WHERE contains(tags, "icm/uses")
SORT type ASC
```

**To query `icm/participates` nodes:**
```dataview
TABLE type, scope, founded
FROM "Open_Science_Neuroscience"
WHERE contains(tags, "icm/participates")
SORT type ASC
```

**To query all ontologies and terminologies:**
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/02_Standards"
WHERE type = "terminology" OR type = "framework"
SORT type ASC
```

**To query all format standards:**
```dataview
TABLE domain, founded
FROM "Open_Science_Neuroscience/02_Standards"
WHERE type = "standard"
SORT domain ASC
```

**To query French governance nodes:**
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/04_Governance"
WHERE scope = "french"
SORT type ASC
```

**To query European governance nodes:**
```dataview
TABLE type, domain, founded
FROM "Open_Science_Neuroscience/04_Governance"
WHERE scope = "european"
SORT type ASC
```

**To query working groups and frameworks:**
```dataview
TABLE scope, domain, founded
FROM "Open_Science_Neuroscience/04_Governance"
WHERE type = "working-group" OR type = "framework" OR type = "initiative"
SORT scope ASC
```

---

## Backlog — TODOs and Candidate Nodes

---

### Vault review — improvements identified 2026-04

#### 1. Thin nodes that need enrichment (body < 10 substantive lines)
- [x] [[02_Standards/SNOMED CT\|SNOMED CT]] — enriched with concept model, French release, AP-HP context ✅
- [x] [[02_Standards/HL7 FHIR\|HL7 FHIR]] — enriched with resource model, versioning, SMART, French ANS, FHIR/OMOP comparison ✅
- [x] [[02_Standards/DICOM\|DICOM]] — enriched with object model, SOP classes, dcm2niix pipeline, CENIR context ✅
- [x] [[02_Standards/NIDM\|NIDM]] — enriched with three components (Experiment/Results/Workflow), tools, adoption status ✅
- [x] [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] — enriched with national nodes, MIABIS, Directory, Negotiator, French BIOBANQUES node ✅
- [x] [[04_Governance/ELIXIR\|ELIXIR]] — enriched with Hub, five platforms, Communities, AAI, French node (IFB) ✅
- [x] [[04_Governance/FORCE11\|FORCE11]] — heading order fixed; Key Outputs added ✅
- [x] [[04_Governance/ECRIN\|ECRIN]] — enriched with national partner structure, F-CRIN, CTIS, REDCap network ✅
- [x] [[04_Governance/CoSO\|CoSO]] — enriched with four colleges, membership, key outputs (PNSO, FNSO) ✅
- [x] [[04_Governance/GO FAIR\|GO FAIR]] — heading order fixed; Key Outputs added ✅
- [x] [[04_Governance/OpenAIRE\|OpenAIRE]] — enriched with OpenAIRE Graph, Zenodo, Monitor, Amnesia, Scholix, Horizon compliance ✅
- [x] [[04_Governance/Human Brain Project\|Human Brain Project]] — enriched with full legacy map (EBRAINS, openMINDS, UBERON, Julich Atlas) ✅
- [x] [[04_Governance/LifeTime Initiative\|LifeTime Initiative]] — enriched with ESFRI roadmap, scientific vision, neuroscience focus, flagship paper ✅
- [x] [[04_Governance/RDA Neuroscience IG\|RDA Neuroscience IG]] — enriched with role, activities, standards connections ✅
- [x] [[03_Platforms/VIVLI\|VIVLI]] — enriched with access model, enclave, neurological datasets, contributors ✅
- [x] [[04_Governance/TransCelerate\|TransCelerate]] — enriched with key programmes (CPT, myTrials, digital pathology, DCT) ✅
- [x] [[04_Governance/UNESCO Open Science Recommendation\|UNESCO Open Science Recommendation]] — enriched with four pillars, definition, implementation ✅

#### 2. Schema inconsistencies to fix
- [x] **`parent_org: Paris Brain Institute ICM`** still appears in [[04_Governance/CATI\|CATI]] frontmatter — fixed ✅
- [x] **`FAIR Principles.md` is in `04_Governance`** but `type: framework` — noted in MOC; moving to `02_Standards` deferred (would change Dataview folder scope) — acceptable as-is for now
- [x] **`CDISC` is `type: consortium`** — changed to `type: initiative`; kept in `02_Standards` as standards-producing body ✅
- [x] **`HAL` is `type: platform` but is functionally a publication archive** — changed to `type: repository` ✅
- [x] **`OMERO` is in `01_Actors`** — moved to `03_Platforms` with `type: platform` ✅
- [x] **`VIVLI` is `type: repository` in `04_Governance`** — moved to `03_Platforms`, type changed to `platform` ✅
- [x] **`domain: health` vs `domain: clinical`** — rule established: `health` = administrative/EHR/public health; `clinical` = research/trial; applied across vault ✅
- [x] **`founded:` field missing on several nodes** — added to [[04_Governance/RDA Neuroscience IG\|RDA Neuroscience IG]] (2015), [[04_Governance/GT-GeDeM\|GT-GeDeM]] (2017); [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] and [[04_Governance/QUAREP-LiMi\|QUAREP-LiMi]] already had it ✅
- [x] **`INCF.md` has a `logo:` property** — renamed to `icon:` ✅
- [x] **Heading order inversion in [[04_Governance/FORCE11\|FORCE11]] and [[04_Governance/GO FAIR\|GO FAIR]]** — fixed; Overview now first, Key Outputs second ✅

#### 3. Missing `icm/uses` and `icm/participates` tags on eligible nodes
- [x] [[03_Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]] — already tagged `icm/uses` ✅
- [x] [[03_Platforms/EGA\|EGA]] — already tagged `icm/uses` ✅
- [x] [[03_Platforms/NCBI GEO\|NCBI GEO]] — already tagged `icm/uses` ✅
- [x] [[04_Governance/HAL\|HAL]] — already tagged `icm/uses` ✅
- [x] [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] — already tagged `icm/uses` ✅
- [x] [[04_Governance/OPIDoR\|OPIDoR]] — already tagged `icm/uses` ✅
- [x] [[02_Standards/CDISC\|CDISC]] — already tagged `icm/uses` ✅
- [x] [[02_Standards/OMOP CDM\|OMOP CDM]] — already tagged `icm/uses` ✅
- [x] [[04_Governance/EATRIS\|EATRIS]] — already tagged `icm/participates` ✅
- [x] [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] — added `icm/participates` (Banque ADN et Cellules is ICM's BBMRI-ERIC node) ✅
- [x] [[04_Governance/RDA\|RDA]] — ICM participates indirectly via CNRS; not tagged (institutional membership not confirmed)

#### 4. `Paris Brain Institute.md` anchor node needs updating
- [x] **Overview paragraph** — rewritten to reflect NeurATRIS, MUDIS4LS, full ecosystem ✅
- [x] **`parent_org` wikilinks** — YAML stays plain text (wikilinks break YAML parsing); body Institutional Affiliations now uses `[[Sorbonne Universite]]` ✅
- [x] **`tags:` empty field** — removed ✅
- [x] **`icon:` broken URL** — removed ✅
- [x] **`[[France BioImaging|FBI]]` alias** — fixed to `[[France BioImaging]]` ✅
- [x] **Paris Open Science Peers section** — simplified to MOC pointer ✅

#### 5. Body text quality issues found across nodes
- [x] **`BIDS.md`** — enriched with modalities, BEP process, BIDS Apps ecosystem, raw vs derivatives distinction ✅
- [x] **`NWB.md`** — enriched with data types, HDF5/APIs, NDX extensions, IBL/Allen datasets, BIDS interop ✅
- [x] **`OMOP CDM.md`** — enriched with domain tables, OHDSI tools, federated network model, French context ✅
- [x] **`HL7 FHIR.md`** — enriched (done in section 1) ✅
- [x] **`SNOMED CT.md`** — enriched (done in section 1) ✅
- [x] **Duplicate `## Open Science Connections` / `## Connections` in [[01_Actors/CENIR\|CENIR]]** — merged into single Connections section ✅

#### 6. Structural and navigation improvements
- [x] **MOC Governance section header** — updated to `(51 nodes)` ✅
- [x] **`last updated`** — updated to 2026-04-07 ✅
- [x] **Key Structural Relationships — ICM facility chains** — CENIR, iGENSEQ, DAC, Banque ADN chains added ✅
- [x] **Key Structural Relationships — NeurATRIS and MUDIS4LS** — added; MUDIS4LS relationship corrected to “managed by IFB” (not “part of” IFB) ✅
- [x] **Which Ontology for Which Task table** — genomic variants and MeSH rows added ✅
- [x] **`[[Sorbonne Universite]]` in French governance section** — already present ✅

#### 8. New actors — open science linkages to ICM ✅ COMPLETE

**Nodes created:** CURE-ND, DZNE, UK DRI, Mission Lucidity, JPND, HDR UK, The Florey, ARDC, Mount Sinai Neuroscience, Synapse/AMP-AD, Preprint Servers (bioRxiv + medRxiv)
**Nodes rejected (with reasoning below):** HMC, Helmholtz Open Science, DELCODE/LICA, DPUK, COEN, AEP, CommonMind (context in Mount Sinai), PsychENCODE (context in Mount Sinai), Yale/Wu Tsai (YODA already in vault), Stanford/CORES (all outputs already in vault)

#### 9. Additional nodes identified during session 2026-04-08
- [x] **OBI** — [[01_Actors/OBI\|OBI]] added to `01_Actors` ✅
- [x] **Brain-CODE** — [[03_Platforms/Brain-CODE\|Brain-CODE]] added to `03_Platforms` ✅

---

For each institution below: investigate open science initiatives, data sharing
policies, relevant consortia, and linkages back to ICM. Create nodes where
connections are substantive. Check whether existing vault nodes already capture
the relationship (e.g. [[03_Platforms/EBRAINS\|EBRAINS]], [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]], [[04_Governance/JPND\|JPND]]).

##### DZNE — Deutsches Zentrum für Neurodegenerative Erkrankungen
- Website: https://www.dzne.de
- German national centre for neurodegenerative disease research; Helmholtz Association member
- **Open access**: Follows Helmholtz Association Open Access policy; mandatory OA
  for publicly funded research; publishes in Nature Communications, eLife, PLOS
- **Open data cohorts**:
  - DELCODE — longitudinal cognitive impairment & dementia study; structured access
  - LICA — Longitudinal Imaging of DZNE network; internal + collaborative
  - NAKO — participates in German National Cohort; application-based access
  - DESCRIBE — dementia registry; collaborative
- **EBRAINS / HBP**: DZNE researchers active contributors to EBRAINS infrastructure;
  share neuroimaging data, models, workflows; connects to EOSC
- **Helmholtz Open Science**: member of Helmholtz Open Science Office; follows
  Helmholtz Research Data Guidelines; participates in Helmholtz Metadata
  Collaboration (HMC, https://helmholtz-metadaten.de)
- **JPND**: active participant in Joint Programme Neurodegenerative Disease Research
  (https://www.jpnd.eu) — already partially covered via [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] linkage
- ICM linkage: ENIGMA Consortium overlap; EBRAINS membership; JPND shared programmes;
  Alzheimer's / neurodegeneration research alignment
- Potential new nodes:
  - **DZNE** — ✅ create (major actor; EBRAINS, JPND, ENIGMA connections)
  - **JPND** — ✅ create (governance initiative linking DZNE, UK DRI, and ICM)
  - **HMC** — ❌ skip (German-internal; no direct ICM connection; covered by RDA/FAIR Principles)
  - **Helmholtz Open Science** — ❌ skip (German policy; context handled within DZNE node)
  - **DELCODE / LICA** — ❌ skip (DZNE-specific cohorts; not open platforms ICM uses)

*(Further actors to be added here once full list is provided)*

##### CURE-ND — Catalysing a United Response in Europe to Neurodegenerative Diseases
- Website: https://www.ukdri.ac.uk/partners/cure-nd (hosted on UK DRI site)
- **ICM is a founding member** (launched 2020); four-way alliance: DZNE, ICM (Paris Brain
  Institute), Mission Lucidity (Belgium), UK DRI (UK)
- 2,000+ researchers across the four institutes
- Activities: annual ECR workshops (2022 London, 2023 Leuven, 2024 Bonn), clinical
  symposia (Paris 2023 workshop on clinical trials/digital biomarkers), AI/ML workshop
  (2026, with UK DRI, DZNE, ICM, HDR UK, Mission Lucidity directors)
- Mandate: share expertise, raise global awareness, advocate for European brain research
  funding, train next generation of neurodegeneration researchers
- **This is the structural link between DZNE, UK DRI, and Mission Lucidity** —
  all three should be documented primarily as CURE-ND partners, not independent actors
- Potential new nodes:
  - **CURE-ND** — ✅ create (ICM founding member; direct alliance; umbrella for DZNE, UK DRI,
    Mission Lucidity connections; `icm/participates` tag)
  - **DZNE** — ✅ create (CURE-ND partner; EBRAINS contributor; JPND participant)
  - **UK DRI** — ✅ create (CURE-ND partner; JPND participant; strong open science policy)
  - **Mission Lucidity** — ✅ create (CURE-ND partner; imec/KU Leuven/VIB/UZ Leuven
    consortium; neurotechnology focus)
  - **JPND** — ✅ create (shared governance framework for DZNE, UK DRI, ICM
    transnational research; not yet in vault)
  - **HDR UK** — ✅ create (UK health data science; participant in CURE-ND AI/ML workshop;
    UK equivalent of Health Data Hub; FAIR health data ecosystem)

##### The Florey — Florey Institute of Neuroscience and Mental Health (Australia)
- Website: https://florey.edu.au
- Australia's largest brain research institute (~600 staff); University of Melbourne;
  Melbourne Biomedical Precinct; affiliated hospitals: Austin Health, Royal Melbourne
- Research domains: Alzheimer's, Parkinson's, MND, epilepsy, MS, stroke, mental health
- **Open science initiatives found on deeper investigation:**
  - **ENIGMA-Epilepsy** — Florey is a confirmed participant in ENIGMA-Epilepsy working
    group (multiple authors from Florey Department in ENIGMA-Epilepsy publications);
    this connects to [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] already in vault
  - **Australian Epilepsy Project (AEP)** — $30M national cohort; MRI, genetics,
    neuropsychology, AI; builds FAIR-aligned data platform; presented at ARDC
    eResearch Australasia conference as example of FAIR data infrastructure;
    connects neuroimaging + genomics + clinical data at national scale
  - **ARDC (Australian Research Data Commons)** — Australia's national FAIR data
    infrastructure (Australian analogue of EOSC / Recherche Data Gouv); NCRIS-funded;
    RDA partner; alignment with EOSC confirmed; runs FAIR Data 101, PID strategy,
    Biological Psychiatry Data Commons (Gen3/FAIR-aligned psychiatric omics platform);
    AEP data platform presented at ARDC eResearch forum
- **ICM linkage (revised assessment):**
  - [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] — direct overlap (Florey in ENIGMA-Epilepsy; ICM in ENIGMA)
  - ARDC → EOSC alignment: ARDC explicitly named alongside EOSC in international
    data commons convergence discussions; Australian counterpart to
    [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] / [[04_Governance/EOSC\|EOSC]]
  - AEP neuroimaging platform: uses similar multisite MRI + BIDS-compatible data
    structures to CATI/ICM workflows; potential collaboration avenue
- **Verdict (revised):**
  - **The Florey as actor** — ✅ create (ENIGMA-Epilepsy confirmed; AEP as major
    Australian open neuroscience infrastructure; represents southern hemisphere
    open science ecosystem; 01_Actors)
  - **ARDC** — ✅ create (Australia's national FAIR/RDM infrastructure; RDA partner;
    EOSC counterpart; broader picture of global FAIR ecosystem; 04_Governance;
    `scope: international`)
  - **AEP** — ❌ skip (Australian-specific cohort; context handled within Florey node;
    no vault-level open infrastructure connection beyond ARDC/ENIGMA)

##### Mount Sinai — Nash Family Department of Neuroscience / Icahn School of Medicine
- Website: https://icahn.mssm.edu/about/departments-offices/neuroscience
- **Open science initiatives found on deeper investigation:**
  - **CommonMind Consortium (CMC)** — Mount Sinai is lead site; multimodal brain
    genomics data (RNA-seq, epigenomics, chromatin architecture) from schizophrenia,
    bipolar, ALS postmortem brain tissue; data deposited to **Synapse** (Sage
    Bionetworks open platform) and **AMP-AD Knowledge Portal**; uses [[03_Platforms/NCBI GEO\|NCBI GEO]],
    [[03_Platforms/dbGaP\|dbGaP]], and [[02_Standards/AnnData\|AnnData]] formats; open access under controlled access model;
    directly relevant to [[01_Actors/iGENSEQ\|iGENSEQ]] / [[01_Actors/DAC\|DAC]] workflows at ICM
  - **PsychENCODE Consortium** — Mount Sinai is a lead site; NIMH-funded multi-omics
    brain genomics across autism, schizophrenia, bipolar; data shared via Synapse;
    15 US institutions; published in *Science* (2018); directly relevant to ICM
    psychiatric genomics and neurogenomics research
  - **Center for Disease Neurogenomics** — uses UK Biobank, BioMe, psychEMERGE;
    large-scale multi-ethnic GWAS; open GWAS summary statistics
  - **ENIGMA Consortium** — confirmed participant (multiple working groups including
    psychosis); already in vault
  - **Synapse / AMP-AD Knowledge Portal** — not yet in vault; major open platform
    for Alzheimer's and psychiatric multiomics data
- **ICM linkage (revised assessment):**
  - CommonMind / PsychENCODE data on Synapse/AMP-AD are directly accessible to
    ICM's [[01_Actors/iGENSEQ\|iGENSEQ]] and [[01_Actors/DAC\|DAC]] for transcriptomics / multiomics research
  - [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] overlap confirmed
  - Shared use of [[03_Platforms/dbGaP\|dbGaP]], [[03_Platforms/NCBI GEO\|NCBI GEO]], [[03_Platforms/EGA\|EGA]] for controlled-access data
- **Verdict (revised):**
  - **Mount Sinai as actor** — ✅ create (CommonMind + PsychENCODE lead site;
    major open brain genomics data producer; 01_Actors)
  - **Synapse / AMP-AD Knowledge Portal** — ✅ create (open platform hosting
    CommonMind, PsychENCODE, AMP-AD Alzheimer's multiomics; Sage Bionetworks;
    03_Platforms; directly usable by DAC/iGENSEQ)
  - **CommonMind Consortium** — ❌ skip (covered adequately within Mount Sinai
    and Synapse nodes; not a standalone infrastructure)
  - **PsychENCODE** — ❌ skip (same reasoning; context within Mount Sinai node)

##### Yale — Wu Tsai Institute / YODA Project
- Website: https://wti.yale.edu / https://yoda.yale.edu
- **Open science initiatives found on deeper investigation:**
  - **YODA Project** — already in vault ([[04_Governance/YODA Project\|YODA Project]]); confirmed as the key
    Yale open science contribution; 499 clinical trials available; independent
    third-party data access model; influenced NIH data sharing policy; co-founders
    also created **medRxiv** (preprint server for clinical science)
  - **medRxiv** — Yale co-founders (Ross + Krumholz) created medRxiv alongside YODA;
    medRxiv is now the primary preprint server for clinical research; complements
    bioRxiv; directly relevant as preprint infrastructure for ICM clinical research
  - **Wu Tsai Institute** — neurocomputation center explicitly mentions curation
    and sharing of neuroscience data with the broader community; OPM-MEG (first
    in North America); interdisciplinary data science; no distinctive open
    infrastructure beyond YODA/medRxiv
- **ICM linkage (revised assessment):**
  - YODA already in vault — covers clinical trial data sharing
  - medRxiv: directly relevant as preprint server for ICM clinical neuroscience
    publications; complements [[04_Governance/HAL\|HAL]] (French mandate) and general open access
    infrastructure; not yet in vault
- **Verdict (revised):**
  - **Yale / Wu Tsai as actor** — ❌ skip (YODA already in vault; Wu Tsai has no
    additional open infrastructure connection; Yale itself does not warrant a node)
  - **medRxiv** — ✅ create (major preprint infrastructure for clinical neuroscience;
    Yale co-founded; relevant to ICM clinical research outputs alongside bioRxiv;
    03_Platforms or 04_Governance; not yet in vault)
  - Note: **bioRxiv** also not in vault — consider adding alongside medRxiv as
    preprint infrastructure pair

##### Stanford — Wu Tsai Neurosciences / CORES / Center for Reproducible Neuroscience
- Website: https://neuroscience.stanford.edu / https://reproducibility.stanford.edu
- **Open science initiatives found on deeper investigation:**
  - **CORES (Center for Open and REproducible Science)** — Stanford Data Science
    initiative; Poldrack as Faculty Director; cross-disciplinary open science
    training, pre-registration support, data/code sharing advocacy; aims to be
    'gold standard' for open science; not just neuroscience — spans all fields
  - **Center for Reproducible Neuroscience (CRN)** — produces fMRIPrep, NiPreps
    (NiLearn, dMRIPrep, ASLPrep etc.); these are BIDS Apps already effectively
    captured by the [[02_Standards/BIDS\|BIDS]] node; also produced fMRIPrep LTS, maintained by
    CRIUGM Montreal (connecting to [[01_Actors/CONP\|CONP]])
  - **OpenNeuro, BIDS, NeuroVault, Cognitive Atlas, NIDM** — all already in vault;
    Stanford is the institutional home of these but they are documented as
    independent infrastructure nodes
  - **fMRIPrep / NiPreps** — not yet explicitly in vault as a node; however these
    are BIDS Apps and could be captured as a note within [[02_Standards/BIDS\|BIDS]] rather than a
    standalone node
- **ICM linkage (revised assessment):**
  - Stanford's open science contribution is entirely captured by existing nodes;
    CORES is a general reproducibility initiative with no neuroscience-specific
    infrastructure beyond what is already documented
  - fMRIPrep is used at CENIR/ICM for MRI preprocessing; could add a brief mention
    in [[02_Standards/BIDS\|BIDS]] node rather than a new node
- **Verdict (revised):**
  - **Stanford / CORES as actor** — ❌ skip (all open science outputs already in
    vault; CORES is a general initiative not specific to the vault's scope)
  - **fMRIPrep / NiPreps** — ❌ skip (captured within [[02_Standards/BIDS\|BIDS]] Apps ecosystem;
    mention to add to BIDS node body rather than a new node)
  - **medRxiv / bioRxiv** — note: these preprint servers are not Stanford-specific
    but are relevant context identified through the Yale investigation above;
    consider adding as a preprint infrastructure pair node

##### UK DRI — UK Dementia Research Institute
- Website: https://www.ukdri.ac.uk
- Established 2017; UK's leading dementia research institute; principally funded by MRC,
  Alzheimer's Society, and Alzheimer's Research UK; 750+ researchers
- Hub at UCL; Centres at Cambridge, Cardiff, Edinburgh, Imperial, King's, Surrey
- **Open science / data sharing policy**:
  - Formal FAIR-aligned Data Sharing Policy (published 2025):
    https://www.ukdri.ac.uk/sites/default/files/2025-03/UK-DRI-Data-Sharing-Policy.pdf
  - Mandates data release no later than publication or 24 months after generation
  - Requires deposit in established public repositories (re3data listed)
  - Dedicated Data Science and Informatics Team + Informatics Steering Committee
  - UK DRI Computational Reproducibility Prize (annual)
- **Open code**: Active GitHub organisation (https://github.com/UKDRI);
  open-source pipelines (GWAS/QTL standardisation, fine-mapping, single-cell);
  2026 EMBL course materials on spatial transcriptomics / dementia data science
- **JPND**: Active participant in EU Joint Programme for Neurodegenerative Disease Research
  (resources page lists JPND); connects to COEN initiative
- **HDR UK**: Member of UK Health Data Research Alliance; collaboration with HDR UK +
  GSK on population-scale dementia health data study using NHS records
- **COEN**: Participant in Network of Centres of Excellence in Neurodegeneration
  (aligned with JPND broader framework)
- **Dementias Platform UK (DPUK)**: MRC-funded; UK DRI researchers access 2M+ individuals
  from 40+ cohort studies via DPUK; overlaps with [[01_Actors/UK Biobank\|UK Biobank]]
- **ICM linkage**:
  - [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]] — overlapping Alzheimer's/neurodegeneration working groups
  - [[01_Actors/ADNI\|ADNI]] — shared use of multisite neuroimaging cohort
  - JPND joint programmes (shared with ICM via CNRS/Inserm participation)
  - Research domain alignment: Alzheimer's, Parkinson's, FTD, tau pathology,
    neuroinflammation — directly overlapping with ICM programmes
  - [[01_Actors/UK Biobank\|UK Biobank]] — UK DRI researchers major users; ICM researchers also access UKB
  - Potential direct collaboration: NeurATRIS / EATRIS network (translational neuroscience)
- **Potential new nodes**:
  - **UK DRI** — ✅ create (major actor; JPND, ENIGMA, EATRIS connections)
  - **JPND** — ✅ create (shared with DZNE; single node serves both)
  - **HDR UK** — ✅ create (UK health data science institute; FAIR health data; UK Biobank / EGA / OMOP CDM ecosystem)
  - **DPUK** — ❌ skip (UK-internal platform; UK Biobank node already covers main ICM-relevant UK cohort)
  - **COEN** — ❌ skip (JPND-aligned network; covered within JPND node context)

#### 7. Candidate new nodes (completed)
- [x] **ClinVar** — [[02_Standards/ClinVar\|ClinVar]] added to `02_Standards` ✅
- [x] **Software Heritage** — [[04_Governance/Software Heritage\|Software Heritage]] added to `04_Governance` ✅
- [x] **Cell Ontology (CL)** — [[02_Standards/Cell Ontology\|Cell Ontology]] added to `02_Standards` ✅
- [x] **AnnData / h5ad** — [[02_Standards/AnnData\|AnnData]] added to `02_Standards` ✅
- [x] **NeMO Archive** — [[03_Platforms/NeMO Archive\|NeMO Archive]] added to `03_Platforms` ✅
- [x] **Recherche Data Gouv enrichment** — [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]] fully enriched with disciplinary nodes, DOI/FAIR features, OPIDoR integration, EOSC harvesting, ICM deposit guidance ✅
- [x] **ANS (Agence du Numérique en Santé)** — [[04_Governance/ANS\|ANS]] added to `04_Governance` ✅
- [x] **OHDSI** — [[01_Actors/OHDSI\|OHDSI]] added to `01_Actors` ✅

# Open Science Initiatives in Neuroscience in Japan

## Major National Programs

### Brain/MINDS (Brain Mapping by Integrated Neurotechnologies for Disease Studies)

- Launched ~2014, funded by **AMED** (Japan Agency for Medical Research and Development)
- Focuses on marmoset brain mapping using advanced neurotechnologies
- Has an associated **data sharing portal** providing open access to marmoset neuroimaging and connectome data
- Aims to bridge animal models and human neurological/psychiatric disease

### Brain/MINDS Beyond

- Extension toward **human brain imaging data**
- Multi-site neuroimaging studies with data-sharing components
- Connects Japanese data to international brain mapping efforts

---

## Open Datasets

### SRPBS Multi-Disorder Neuroimaging Dataset

- Multi-site resting-state fMRI dataset from Japanese institutions
- Covers schizophrenia, depression, ASD, OCD, and healthy controls
- Deposited on **OpenNeuro**, making it internationally accessible
- A significant contribution to psychiatric neuroimaging open data

---

## Institutional Contributions

|Institution|Notable Open Science Activity|
|---|---|
|**RIKEN Center for Brain Science (CBS)**|Data sharing, open tools, international collaborations|
|**ATR (Advanced Telecommunications Research)**|Brain decoding datasets, open code|
|**Kamitani Lab (Kyoto Univ./ATR)**|Shared data/code from visual imagery & dream decoding studies|
|**NICT/CiNet**|Neural imaging data, open access outputs|

---

## Infrastructure & Policy

- **INCF Japan Node** – Japanese participation in the International Neuroinformatics Coordinating Facility, supporting data standards and sharing
- **MEXT & JST open science policies** – Government mandates pushing toward open access publishing and data sharing for publicly funded research (formalized around 2015–2017)
- **BIDS adoption** – Japanese labs increasingly using Brain Imaging Data Structure for standardized data sharing

---

## International Connections

- Japanese groups contributing to **OpenNeuro**, **OSF**, and **figshare**
- Participation in global initiatives like **ABIDE**, **ADHD-200**
- Collaborations with **Human Connectome Project** style efforts

---

## Caveats

- This is a fast-moving area, and some initiatives may have evolved or ended since my knowledge cutoff (early 2025)
- Specific data portal URLs and access conditions change — checking **AMED's website** or **OpenNeuro** directly is recommended for current status

Would you like more detail on any specific initiative or institution?