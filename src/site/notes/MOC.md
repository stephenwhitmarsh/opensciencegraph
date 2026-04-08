---
{"dg-publish":true,"permalink":"/moc/","tags":["MOC","gardenEntry"],"dg-note-properties":{"type":"MOC","aliases":["Open Science Hub","Open Science Neuroscience Index"],"tags":["MOC","gardenEntry"]}}
---

# Map of Content

This map is a relational index of the **open science** ecosystem for neuroscience, including open science frameworks, data standards, platforms, infrastructure and working groups. The goal is to disambiguate the field by showing dependencies and convergences across actors, domains and research initiatives. While initially overwhelming, the graph can be explored with detailed descriptions in each node. The original focus has been on [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]'s operational context (explaining it's node centrality). However, the network can be extended beyond its direct environment and include standards, policies and partners who engage in open neuroscience. In open science the saying certainly goes:

> *There are no strangers here, just friends you haven't met yet*. - W.B. Yeats

What you see is an [Obsidian](https://obsidian.md/) vault, with the website published to Vercel via my public [github repository](https://github.com/stephenwhitmarsh/opensciencegraph) using the [Digital Garden community plugin](https://docs.forestry.md/). If you want to contribute or make a correction or suggestion, please [email me](mailto:stephen.whitmarsh@icm-institute.org).

---

## Actors — Consortia, Institutes and Projects

*All in `01_Actors` (including [[01_Actors/Paris Brain Institute\|Paris Brain Institute]]). Filter by `type: consortium / institute / initiative / biobank` and `scope`.*

### ICM — Paris Brain Institute
- [[01_Actors/Paris Brain Institute\|Paris Brain Institute]] — ICM; the central node of this graph; hosts CENIR, CATI, iGENSEQ, DAC, Banque ADN et Cellules and 5 other platforms

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
- [[01_Actors/Brain-MINDS\|Brain-MINDS]] — Japan's AMED-funded brain mapping programme; open marmoset atlas; SRPBS dataset on OpenNeuro

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

### Neuroimaging
- [[02_Standards/DICOM\|DICOM]] — universal clinical imaging format; source format converted to NIfTI/BIDS
- [[02_Standards/NIfTI\|NIfTI]] — universal processed neuroimaging format (.nii/.nii.gz); pivot between DICOM and BIDS
- [[02_Standards/CIFTI\|CIFTI]] — surface+volume (greyordinate) format for cortical data; developed by HCP; complements NIfTI
- [[02_Standards/BIDS\|BIDS]] — Brain Imaging Data Structure; de facto community standard for neuroimaging datasets
- [[02_Standards/NIDM\|NIDM]] — Neuroimaging Data Model; W3C PROV-based provenance for neuroimaging experiments
- [[02_Standards/Cognitive Atlas\|Cognitive Atlas]] — ontology of cognitive processes and tasks; used by NeuroVault and BIDS
- [[02_Standards/UBERON\|UBERON]] — cross-species anatomy ontology; brain region annotation in EBRAINS, NWB, Allen Institute
- [[02_Standards/openMINDS\|openMINDS]] — EBRAINS metadata framework; required for EBRAINS data deposit
### Neurophysiology
- [[02_Standards/NWB\|NWB]] — Neurodata Without Borders; community standard for electrophysiology and calcium imaging
- [[02_Standards/HED\|HED]] — Hierarchical Event Descriptors; structured event annotation integrated into BIDS/NWB
- [[02_Standards/SPARC SDS\|SPARC SDS]] — SPARC Data Structure; NIH SPARC programme standard for peripheral nervous system data

### Microscopy
- [[02_Standards/OME File Formats\|OME File Formats]] — OME file formats: archival (OME-TIFF) and cloud-native (OME-Zarr)
- [[02_Standards/REMBI\|REMBI]] — Recommended Metadata for Biological Images; community metadata framework for bioimaging

### Computational Neuroscience
- [[02_Standards/NeuroML\|NeuroML]] — simulator-independent XML format for computational neuron/network models

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
- [[02_Standards/ATC\|ATC]] — WHO Anatomical Therapeutic Chemical classification; drug utilisation standard; OMOP CDM vocabulary
- [[02_Standards/OSIRIS\|OSIRIS]] — French national minimum data set for oncology clinical + genomic data sharing; HL7 FHIR-aligned; INCa-funded
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
- [[03_Platforms/CleanWEB\|CleanWEB]] — Telemedicine Technologies eClinical suite; AP-HP institutional eCRF platform since 2003; regulatory-grade clinical trials (not used by ICM)

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

### International Frameworks and Principles
- [[04_Governance/ARDC\|ARDC]] — Australian Research Data Commons; national FAIR/RDM infrastructure; EOSC counterpart; RDA partner
- [[04_Governance/HDR UK\|HDR UK]] — Health Data Research UK; UK national health data science institute; FAIR; OMOP CDM; HL7 FHIR; CURE-ND AI/ML workshop participant
- [[04_Governance/FAIR Principles\|FAIR Principles]] — 15 Findable/Accessible/Interoperable/Reusable principles (Wilkinson et al. 2016)
- [[04_Governance/GO FAIR\|GO FAIR]] — international initiative for FAIR implementation; Three-Point FAIRification Framework
- [[04_Governance/RDA\|RDA]] — Research Data Alliance; FAIR Data Maturity Model; 120+ working groups
- [[04_Governance/FORCE11\|FORCE11]] — co-authored FAIR Principles; scholarly communications reform
- [[04_Governance/UNESCO Open Science Recommendation\|UNESCO Open Science Recommendation]] — 2021 global framework for open science policy

### Clinical Research Infrastructure
- [[04_Governance/i2b2\|i2b2]] — clinical data warehousing platform; deployed at AP-HP alongside OMOP CDM
- [[04_Governance/YODA Project\|YODA Project]] — Yale Open Data Access; independent third-party clinical trial data sharing (499 trials); influenced NIH data sharing policy; co-founders created medRxiv
- [[04_Governance/TransCelerate\|TransCelerate]] — pharma industry consortium; CDISC standards; trial data sharing

### Working Groups
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
| `01_Actors` | Consortia, institutes, initiatives, projects, software orgs (incl. Paris Brain Institute) | 33 |
| `02_Standards` | All standards, formats, terminologies, ontologies | 47 |
| `03_Platforms` | Repositories, platforms, data infrastructure | 28 |
| `04_Governance` | Infrastructure, policies, frameworks, working groups (french + european + international) | 56 |
| **Total** | | **164** |

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

## TODO
Add link ICM - IFB (DAC as participating platform)