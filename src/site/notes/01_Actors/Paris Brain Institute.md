---
{"dg-publish":true,"permalink":"/01-actors/paris-brain-institute/","dg-note-properties":{"name":"Paris Brain Institute","aliases":["ICM","Institut du Cerveau","PBI"],"website":"https://institutducerveau-icm.org","type":"institute","scope":"french","domain":["neuroimaging","electrophysiology","clinical","multimodal"],"status":"active","founded":2010,"parent_org":["Sorbonne Universite","CNRS","Inserm","AP-HP"]}}
---


# Paris Brain Institute

## Overview
The Paris Brain Institute (Institut du Cerveau — ICM) is a world-leading neuroscience
research centre located at Pitié-Salpêtrière Hospital, Paris. It unites basic science,
clinical neurology, and translational research under one roof, co-governed by
[[04_Governance/CNRS Open Science\|CNRS Open Science]], [[04_Governance/Inserm Open Science\|Inserm Open Science]], [[04_Governance/AP-HP\|AP-HP]], and [[01_Actors/Sorbonne Universite\|Sorbonne Universite]].

ICM operates 10 core technological platforms and participates in the major French and
European open science infrastructures. It is a member node of [[04_Governance/NeurATRIS\|NeurATRIS]] (French
translational neuroscience infrastructure, French component of [[04_Governance/EATRIS\|EATRIS]]), a participant
in [[04_Governance/MUDIS4LS\|MUDIS4LS]] (IFB-led FAIR data infrastructure), and active in [[03_Platforms/EBRAINS\|EBRAINS]], [[ENIGMA
Consortium]], and [[04_Governance/France BioImaging\|France BioImaging]] through its platforms [[04_Governance/CATI\|CATI]] ([[France Life
Imaging]]) and ICM Quant. Data management and bioinformatics are centralised through
[[04_Governance/CATI\|CATI]] (neuroimaging) and [[01_Actors/DAC\|DAC]] (genomics and multi-omics), with computing resources
via [[04_Governance/IFB\|IFB]] and open science compliance implemented through [[04_Governance/OPIDoR\|OPIDoR]] and [[04_Governance/HAL\|HAL]].
 
## Core Facilities

ICM operates 10 technological platforms accessible to internal and external researchers via https://plateforme.institutducerveau.org.

### CENIR — Centre de NeuroImagerie de Recherche
https://cenir.institutducerveau.org — Human neuroimaging research centre. Equipment: 3T MRI (×2), simultaneous PET-MRI (Siemens Biograph mMR), MEG (Elekta Neuromag), EEG, TMS, eye-tracking. Supports structural, functional, diffusion, spectroscopy, and molecular imaging. Data managed via [[04_Governance/CATI\|CATI]] pipelines; primary site for MEMENTO, INSIGHT-preAD, and iShare cohorts.

### CATI — Centre d'Acquisition et de Traitement des Images
https://cati-neuroimaging.com — French national neuroimaging data management centre hosted at ICM. See [[04_Governance/CATI\|CATI]].

### ICM Quant — Quantitative Microscopy
https://quant.institutducerveau.org — Advanced light microscopy; [[04_Governance/France BioImaging\|France BioImaging]] node. Confocal, multiphoton, super-resolution (STED, STORM/PALM), light-sheet, FLIM. FAIR image data management via [[01_Actors/OME\|OME]] (OMERO); connected to [[04_Governance/Euro-BioImaging\|Euro-BioImaging]] open access programme.

### HISTOMICS — Histology and Neuropathology
https://histomics.institutducerveau.org — Tissue sectioning, immunohistochemistry, immunofluorescence, in situ hybridisation, digital slide scanning.

### iGENSEQ — Genomics and Sequencing
https://igenseq.institutducerveau.org — Next-generation sequencing: RNA-seq, whole-exome, whole-genome, targeted panels, single-cell RNA-seq, spatial transcriptomics. Data aligned with [[02_Standards/VCF\|VCF]] and [[01_Actors/GA4GH\|GA4GH]] standards.

### Banque ADN et Cellules — Biobank
https://banqueadn.institutducerveau.org — Neurological disease biobank: DNA, RNA, cells, CSF, plasma, iPSCs from neurological patient cohorts. Aligned with [[04_Governance/BBMRI-ERIC\|BBMRI-ERIC]] standards; phenotyping via [[02_Standards/HPO\|HPO]] and [[02_Standards/ORDO\|ORDO]].

### ICV — Ingénierie Cellulaire et Vectorologie
https://icv.institutducerveau.org — Two sub-units: **CELIS** (cell culture, iPSC generation and differentiation) and **Vectorology** (AAV, lentivirus, adenovirus production for gene therapy and circuit tracing).

### ePHYS — Electrophysiology
https://ephys.institutducerveau.org — Preclinical electrophysiology: in vitro and ex vivo patch-clamp, in vivo recording (Neuropixels, tetrodes), multi-electrode array (MEA), high-density MEA. Data output compatible with [[02_Standards/NWB\|NWB]].

### PRISME — Behavioural Phenotyping
https://prisme.institutducerveau.org — Human behavioural and cognitive laboratory.

### DAC — Data Analysis Core
https://dac.institutducerveau.org — Bioinformatics and statistical analysis support: RNA-seq, genomics, imaging pipelines, training, consultation. Implements [[04_Governance/FAIR Principles\|FAIR Principles]]; interfaces with [[04_Governance/IFB\|IFB]] and [[04_Governance/OPIDoR\|OPIDoR]] infrastructure.

### RnD Unit — F.P.Journe Charity Fund
https://rndunit.institutducerveau.org — Custom scientific instrumentation design and fabrication; open library of ICM-developed devices available to the research community.

## Institutional Affiliations
- [[04_Governance/CNRS Open Science\|CNRS Open Science]]
- [[04_Governance/Inserm Open Science\|Inserm Open Science]]
- [[04_Governance/AP-HP\|AP-HP]]
- [[01_Actors/Sorbonne Universite\|Sorbonne Universite]]

## Standards Used
- Neuroimaging: [[02_Standards/BIDS\|BIDS]], [[02_Standards/NIfTI\|NIfTI]], [[02_Standards/CIFTI\|CIFTI]], [[02_Standards/DICOM\|DICOM]]
- Clinical: [[02_Standards/OMOP CDM\|OMOP CDM]], [[02_Standards/HL7 FHIR\|HL7 FHIR]], [[02_Standards/ICD-10\|ICD-10]], [[02_Standards/LOINC\|LOINC]], [[02_Standards/CCAM\|CCAM]]
- Genomics / rare disease: [[02_Standards/HPO\|HPO]], [[02_Standards/ORDO\|ORDO]], [[02_Standards/MONDO\|MONDO]], [[02_Standards/ADO\|ADO]] (Alzheimer's)

## Platforms Used
- [[03_Platforms/OpenNeuro\|OpenNeuro]]
- [[03_Platforms/EBRAINS\|EBRAINS]]
- [[03_Platforms/Recherche Data Gouv\|Recherche Data Gouv]]
- [[04_Governance/Health Data Hub\|Health Data Hub]]
- [[04_Governance/OPIDoR\|OPIDoR]]
- [[03_Platforms/OMERO\|OMERO]]

## Networks and Consortia
- [[01_Actors/INCF\|INCF]] - via [[04_Governance/CNRS Open Science\|CNRS Open Science]] French national node
- [[01_Actors/ENIGMA Consortium\|ENIGMA Consortium]]
- [[04_Governance/France Life Imaging\|France Life Imaging]] - via [[04_Governance/CATI\|CATI]]
- [[03_Platforms/EBRAINS\|EBRAINS]]
- [[04_Governance/ECRIN\|ECRIN]] - via [[04_Governance/AP-HP\|AP-HP]]
- [[04_Governance/GT-GeDeM\|GT-GeDeM]] - RTmfm working group on microscopy data management (DAC participates)
- [[04_Governance/IFB\|IFB]] - via DAC
- [[04_Governance/France BioImaging\|France BioImaging]] — via ICM Quant microscopy platform

## French Policy Context
- [[04_Governance/Ouvrir la Science\|Ouvrir la Science]]
- [[04_Governance/CoSO\|CoSO]]
- [[04_Governance/ANR Open Science Policy\|ANR Open Science Policy]]

## Paris Open Science Peers
See the MOC Paris Peer Institutions section for a full list. Key co-located partners:
- [[01_Actors/Institut Pasteur\|Institut Pasteur]], [[01_Actors/Institut Curie\|Institut Curie]], [[01_Actors/Institut de Myologie\|Institut de Myologie]], [[01_Actors/Sorbonne Universite\|Sorbonne Universite]], [[01_Actors/EMBL\|EMBL]]

## Resources
- https://institutducerveau-icm.org
- https://cati-neuroimaging.com
