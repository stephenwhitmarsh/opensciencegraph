---
{"dg-publish":true,"permalink":"/standards/standards/","tags":["MOC"],"dg-note-properties":{"type":"MOC","tags":["MOC"]}}
---

# Standards, Terminologies and Ontologies

This index covers all data format standards, metadata frameworks, terminologies, and ontologies in the graph. The collection spans neuroimaging formats and structures (BIDS, NIfTI, CIFTI, DICOM), neurophysiology standards (NWB, HED, SPARC SDS), microscopy metadata (OME File Formats, REMBI), clinical interoperability standards (HL7 FHIR, OMOP CDM, CDISC, openEHR), disease classification systems (ICD-10, ICD-11, ORDO, MONDO), phenotypic and genomic ontologies (HPO, VCF, Phenopackets), and foundational research data management standards (PROV-O, DCAT, Dublin Core). 

Filter using `type: standard / terminology / framework` and `domain`. 
Return to [[MOC\|MOC]].

- [[Standards/ADO\|ADO]] — Alzheimer's Disease Ontology; biomarkers, staging, genetics for Alzheimer's cohorts
- [[Standards/AnnData\|AnnData]] — de facto standard format (h5ad) for single-cell genomics data; Scanpy/scverse ecosystem
- [[Standards/ATC\|ATC]] — WHO Anatomical Therapeutic Chemical classification; drug utilisation standard; OMOP CDM vocabulary
- [[Standards/BIDS\|BIDS]] — Brain Imaging Data Structure; de facto community standard for neuroimaging datasets
- [[Standards/CCAM\|CCAM]] — French national procedure classification; present in SNDS and AP-HP PMSI billing
- [[Standards/CDISC\|CDISC]] — clinical trial data standards (SDTM, ADaM, CDASH); regulatory submissions
- [[Standards/Cell Ontology\|Cell Ontology]] — OBO Foundry ontology for cell types; required for single-cell data annotation (CELLxGENE, BICAN)
- [[Standards/ChEBI\|ChEBI]] — Chemical Entities of Biological Interest; drugs, metabolites, neurotransmitters (EMBL-EBI)
- [[Standards/CIFTI\|CIFTI]] — surface+volume (greyordinate) format for cortical data; developed by HCP; complements NIfTI
- [[Standards/ClinVar\|ClinVar]] — NCBI authoritative database of clinical variant interpretations; pathogenicity classifications
- [[Standards/Cognitive Atlas\|Cognitive Atlas]] — ontology of cognitive processes and tasks; used by NeuroVault and BIDS
- [[Standards/DCAT\|DCAT]] — W3C Data Catalog Vocabulary; powers EOSC and Recherche Data Gouv discoverability
- [[Standards/DICOM\|DICOM]] — universal clinical imaging format; source format converted to NIfTI/BIDS
- [[Standards/Dublin Core\|Dublin Core]] — 15-element base metadata standard; present in all repositories (Zenodo, HAL)
- [[Standards/ERN Vocabularies\|ERN Vocabularies]] — ERN-RND and ERN-EpiCARE patient registry terminologies; ORDO+HPO+OMOP CDM
- [[Standards/GO\|GO]] — Gene Ontology; biological process, molecular function, cellular component; used in transcriptomics
- [[Standards/HED\|HED]] — Hierarchical Event Descriptors; structured event annotation integrated into BIDS/NWB
- [[Standards/HL7 FHIR\|HL7 FHIR]] — Fast Healthcare Interoperability Resources; mandated by EHDS for EHR exchange
- [[Standards/HPO\|HPO]] — Human Phenotype Ontology; 18,000+ phenotypic abnormality terms for rare disease genomics
- [[Standards/ICD-10\|ICD-10]] — WHO disease classification; CIM-10 is the French version used in SNDS and AP-HP billing
- [[Standards/ICD-11\|ICD-11]] — WHO updated classification (2022); France in transition; improved neuroscience coverage
- [[Standards/LOINC\|LOINC]] — standard for lab tests, biomarkers, clinical observations
- [[Standards/MedDRA\|MedDRA]] — adverse event coding for clinical trial regulatory submissions (EMA, ANSM)
- [[Standards/MeSH\|MeSH]] — NLM controlled vocabulary for PubMed indexing and ClinicalTrials.gov; ~30,000 biomedical descriptors
- [[Standards/MONDO\|MONDO]] — Monarch Disease Ontology; harmonises ICD-10, OMIM, ORDO into one hierarchy
- [[Standards/NBO\|NBO]] — Neurobehavior Ontology; behavioural phenotypes in humans and model organisms
- [[Standards/NCIT\|NCIT]] — NCI Thesaurus; cancer and clinical research terminology; used in CDISC SDTM submissions
- [[Standards/NeuroML\|NeuroML]] — simulator-independent XML format for computational neuron/network models
- [[Standards/NIDM\|NIDM]] — Neuroimaging Data Model; W3C PROV-based provenance for neuroimaging experiments
- [[Standards/NIfTI\|NIfTI]] — universal processed neuroimaging format (.nii/.nii.gz); pivot between DICOM and BIDS
- [[Standards/NWB\|NWB]] — Neurodata Without Borders; community standard for electrophysiology and calcium imaging
- [[Standards/OBI\|Standards/OBI]] — Ontology for Biomedical Investigations; formal study protocol description
- [[Standards/OME File Formats\|OME File Formats]] — OME file formats: archival (OME-TIFF) and cloud-native (OME-Zarr)
- [[Standards/OMIM\|OMIM]] — Online Mendelian Inheritance in Man; gene-disease relationships; MIM numbers; rare neurological diseases
- [[Standards/OMOP CDM\|OMOP CDM]] — OHDSI Common Data Model; federated observational health research
- [[Standards/openEHR\|openEHR]] — semantic EHR specification using archetypes and templates
- [[Standards/openMINDS\|openMINDS]] — EBRAINS metadata framework; required for EBRAINS data deposit
- [[Standards/ORDO\|ORDO]] — Orphanet Rare Disease Ontology; European standard for rare neurological diseases
- [[Standards/OSIRIS\|OSIRIS]] — French national minimum data set for oncology clinical + genomic data sharing; HL7 FHIR-aligned; INCa-funded
- [[Standards/Phenopackets\|Phenopackets]] — GA4GH standard linking clinical phenotypes (HPO) to genomic data (ISO/TS 5435)
- [[Standards/PROV-O\|PROV-O]] — W3C Provenance Ontology; foundation for NIDM and DataLad provenance tracking
- [[Standards/REMBI\|REMBI]] — Recommended Metadata for Biological Images; community metadata framework for bioimaging
- [[Standards/RxNorm\|RxNorm]] — NLM drug terminology; clinical drug names and identifiers; primary drug vocabulary in OMOP CDM
- [[Standards/SNOMED CT\|SNOMED CT]] — comprehensive clinical terminology; core vocabulary in OMOP CDM and HL7 FHIR
- [[Standards/SPARC SDS\|SPARC SDS]] — SPARC Data Structure; NIH SPARC programme standard for peripheral nervous system data
- [[Standards/UBERON\|UBERON]] — cross-species anatomy ontology; brain region annotation in EBRAINS, NWB, Allen Institute
- [[Standards/VCF\|VCF]] — Variant Call Format; universal format for genomic variant data