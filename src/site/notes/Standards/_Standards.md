---
{"dg-publish":true,"permalink":"/standards/standards/","tags":["MOC"],"dg-note-properties":{"type":"MOC","tags":["MOC"]}}
---

# Standards, Terminologies and Ontologies

*[[MOC\|MOC]]*

This index covers all data format standards, metadata frameworks, terminologies, and ontologies in the graph. Sections follow the data lifecycle from acquisition format through to research data management.

---

## Neuroimaging

- [[Standards/BIDS\|BIDS]] — Brain Imaging Data Structure; de facto community standard for neuroimaging datasets
- [[Standards/CIFTI\|CIFTI]] — surface+volume (greyordinate) format for cortical data; developed by [[Actors/Human Connectome Project\|Human Connectome Project]]; complements [[Standards/NIfTI\|NIfTI]]
- [[Standards/Cognitive Atlas\|Cognitive Atlas]] — ontology of cognitive processes and tasks; used by [[Platforms/NeuroVault\|NeuroVault]] and [[Standards/BIDS\|BIDS]]
- [[Standards/DICOM\|DICOM]] — universal clinical imaging format; source format converted to [[Standards/NIfTI\|NIfTI]]/[[Standards/BIDS\|BIDS]]
- [[Standards/NIfTI\|NIfTI]] — universal processed neuroimaging format (.nii/.nii.gz); pivot between [[Standards/DICOM\|DICOM]] and [[Standards/BIDS\|BIDS]]
- [[Standards/NIDM\|NIDM]] — Neuroimaging Data Model; W3C [[Standards/PROV-O\|PROV-O]]-based provenance for neuroimaging experiments
- [[Standards/openMINDS\|openMINDS]] — [[Platforms/EBRAINS\|EBRAINS]] metadata framework; required for [[Platforms/EBRAINS\|EBRAINS]] data deposit
- [[Standards/UBERON\|UBERON]] — cross-species anatomy ontology; brain region annotation in [[Platforms/EBRAINS\|EBRAINS]], [[Standards/NWB\|NWB]], [[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]]

## Neurophysiology

- [[Standards/BrainVision\|BrainVision]] — Brain Products three-file EEG format (.vhdr/.vmrk/.eeg); dominant research EEG format; BIDS-accepted
- [[Standards/EDF\|EDF]] — European Data Format; universal clinical EEG, iEEG, and polysomnography format; EDF+ adds annotations
- [[Standards/HED\|HED]] — Hierarchical Event Descriptors; structured event annotation integrated into [[Standards/BIDS\|BIDS]]/[[Standards/NWB\|NWB]]
- [[Standards/NWB\|NWB]] — Neurodata Without Borders; community standard for electrophysiology and calcium imaging
- [[Standards/SPARC SDS\|SPARC SDS]] — SPARC Data Structure; NIH SPARC programme standard for peripheral nervous system data

## Computational Neuroscience

- [[Standards/NeuroML\|NeuroML]] — simulator-independent XML format for computational neuron/network models

## Microscopy and Bioimaging

- [[Standards/OME File Formats\|OME File Formats]] — [[Actors/OME\|OME]] file formats: archival (OME-TIFF) and cloud-native (OME-Zarr)
- [[Standards/REMBI\|REMBI]] — Recommended Metadata for Biological Images; community metadata framework for bioimaging

## Genomics and Single-cell

- [[Standards/AnnData\|AnnData]] — de facto standard format (h5ad) for single-cell genomics data; Scanpy/scverse ecosystem
- [[Standards/Cell Ontology\|Cell Ontology]] — OBO Foundry ontology for cell types; required for single-cell data annotation (CELLxGENE, [[Actors/BICAN\|BICAN]])
- [[Standards/ClinVar\|ClinVar]] — NCBI authoritative database of clinical variant interpretations; pathogenicity classifications
- [[Standards/FASTQ\|FASTQ]] — universal raw sequencing read format; primary output of all NGS instruments
- [[Standards/GO\|GO]] — Gene Ontology; biological process, molecular function, cellular component; used in transcriptomics
- [[Standards/Phenopackets\|Phenopackets]] — [[Actors/GA4GH\|GA4GH]] standard linking clinical phenotypes ([[Standards/HPO\|HPO]]) to genomic data (ISO/TS 5435)
- [[Standards/SAM-BAM-CRAM\|SAM-BAM-CRAM]] — universal aligned sequencing read formats; pipeline backbone between FASTQ and [[Standards/VCF\|VCF]]/[[Standards/AnnData\|AnnData]]
- [[Standards/VCF\|VCF]] — Variant Call Format; universal format for genomic variant data

## Clinical Data Models and Interoperability

- [[Standards/CDISC\|CDISC]] — clinical trial data standards (SDTM, ADaM, CDASH); regulatory submissions
- [[Standards/HL7 FHIR\|HL7 FHIR]] — Fast Healthcare Interoperability Resources; mandated by [[Governance/EHDS\|EHDS]] for EHR exchange
- [[Standards/OMOP CDM\|OMOP CDM]] — [[Actors/OHDSI\|OHDSI]] Common Data Model; federated observational health research
- [[Standards/openEHR\|openEHR]] — semantic EHR specification using archetypes and templates

## Clinical Classification and Coding

- [[Standards/CCAM\|CCAM]] — French national procedure classification; present in [[Platforms/SNDS\|SNDS]] and [[Governance/AP-HP\|AP-HP]] PMSI billing
- [[Standards/ICD-10\|ICD-10]] — WHO disease classification; CIM-10 is the French version used in [[Platforms/SNDS\|SNDS]] and [[Governance/AP-HP\|AP-HP]] billing
- [[Standards/ICD-11\|ICD-11]] — WHO updated classification (2022); France in transition; improved neuroscience coverage
- [[Standards/LOINC\|LOINC]] — standard for lab tests, biomarkers, clinical observations
- [[Standards/MeSH\|MeSH]] — NLM controlled vocabulary for PubMed indexing and [[Platforms/ClinicalTrials.gov\|ClinicalTrials.gov]]; ~30,000 biomedical descriptors
- [[Standards/OSIRIS\|OSIRIS]] — French national minimum data set for oncology clinical + genomic data sharing; [[Standards/HL7 FHIR\|HL7 FHIR]]-aligned; INCa-funded
- [[Standards/SNOMED CT\|SNOMED CT]] — comprehensive clinical terminology; core vocabulary in [[Standards/OMOP CDM\|OMOP CDM]] and [[Standards/HL7 FHIR\|HL7 FHIR]]

## Drug and Chemical Terminologies

- [[Standards/ATC\|ATC]] — WHO Anatomical Therapeutic Chemical classification; drug utilisation standard; [[Standards/OMOP CDM\|OMOP CDM]] vocabulary
- [[Standards/ChEBI\|ChEBI]] — Chemical Entities of Biological Interest; drugs, metabolites, neurotransmitters ([[Actors/EMBL\|EMBL]]-EBI)
- [[Standards/MedDRA\|MedDRA]] — adverse event coding for clinical trial regulatory submissions (EMA, ANSM)
- [[Standards/NCIT\|NCIT]] — NCI Thesaurus; cancer and clinical research terminology; used in [[Standards/CDISC\|CDISC]] SDTM submissions
- [[Standards/RxNorm\|RxNorm]] — NLM drug terminology; clinical drug names and identifiers; primary drug vocabulary in [[Standards/OMOP CDM\|OMOP CDM]]

## Disease and Phenotype Ontologies

- [[Standards/ADO\|ADO]] — Alzheimer's Disease Ontology; biomarkers, staging, genetics for Alzheimer's cohorts
- [[Standards/ERN Vocabularies\|ERN Vocabularies]] — ERN-RND and ERN-EpiCARE patient registry terminologies; [[Standards/ORDO\|ORDO]]+[[Standards/HPO\|HPO]]+[[Standards/OMOP CDM\|OMOP CDM]]
- [[Standards/HPO\|HPO]] — Human Phenotype Ontology; 18,000+ phenotypic abnormality terms for rare disease genomics
- [[Standards/MONDO\|MONDO]] — Monarch Disease Ontology; harmonises [[Standards/ICD-10\|ICD-10]], [[Standards/OMIM\|OMIM]], [[Standards/ORDO\|ORDO]] into one hierarchy
- [[Standards/NBO\|NBO]] — Neurobehavior Ontology; behavioural phenotypes in humans and model organisms
- [[Standards/OMIM\|OMIM]] — Online Mendelian Inheritance in Man; gene-disease relationships; MIM numbers; rare neurological diseases
- [[Standards/ORDO\|ORDO]] — Orphanet Rare Disease Ontology; European standard for rare neurological diseases

## Research Data Management

- [[Standards/DCAT\|DCAT]] — W3C Data Catalog Vocabulary; powers [[Governance/EOSC\|EOSC]] and [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]] discoverability
- [[Standards/Dublin Core\|Dublin Core]] — 15-element base metadata standard; present in all repositories ([[Platforms/Zenodo\|Zenodo]], [[Governance/HAL\|HAL]])
- [[Standards/OBI\|OBI]] — Ontology for Biomedical Investigations; formal study protocol description
- [[Standards/PROV-O\|PROV-O]] — W3C Provenance Ontology; foundation for [[Standards/NIDM\|NIDM]] and DataLad provenance tracking
- [[Standards/RRID\|RRID]] — Research Resource Identifiers; persistent IDs for reagents, software, and core facilities; governed by [[Governance/NIF\|NIF]]
- [[Standards/ROR\|ROR]] — Research Organization Registry; persistent identifiers for research institutions

---

## Filtering

`type:` — `standard` | `terminology` | `framework`

`domain:` — `neuroimaging` | `electrophysiology` | `clinical` | `genomics` | `bioimaging` | `computational` | `health`