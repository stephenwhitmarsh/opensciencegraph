---
{"dg-publish":true,"permalink":"/actors/paris-brain-institute/","dg-note-properties":{"name":"Paris Brain Institute","aliases":["ICM","Institut du Cerveau","PBI"],"website":"https://institutducerveau-icm.org","type":"institute","scope":"french","domain":["neuroimaging","electrophysiology","clinical","multimodal"],"status":"active","founded":2010,"parent_org":["Sorbonne Universite","CNRS","Inserm","AP-HP"]}}
---


# Paris Brain Institute

## Overview
The Paris Brain Institute (Institut du Cerveau — ICM) is a world-leading neuroscience research centre located at Pitié-Salpêtrière Hospital, Paris. It unites basic science, clinical neurology, and translational research under one roof, co-governed by [[Governance/CNRS Open Science\|CNRS Open Science]], [[Governance/Inserm Open Science\|Inserm Open Science]], [[Governance/AP-HP\|AP-HP]], and [[Actors/Sorbonne Universite\|Sorbonne Universite]].

[[Actors/Paris Brain Institute\|ICM]] operates 10 core [technological platforms](https://parisbraininstitute.org/presentation-technology-platforms) and participates in the major French and European open science infrastructures. It is a member node of [[Governance/NeurATRIS\|NeurATRIS]] (French translational neuroscience infrastructure, French component of [[Governance/EATRIS\|EATRIS]]), a participant in [[Governance/MUDIS4LS\|MUDIS4LS]] ([[Governance/IFB\|IFB]]-led FAIR data infrastructure via [[Actors/DAC\|DAC]]), and active in [[Platforms/EBRAINS\|EBRAINS]], [[Actors/ENIGMA Consortium\|ENIGMA Consortium]], and [[Governance/France BioImaging\|France BioImaging]] through its platforms [[Actors/CATI\|CATI]] ([[Governance/France Life Imaging\|France Life Imaging]]) and ICM.Quant. Data management and bioinformatics are centralised through [[Actors/DAC\|DAC]] (bioinformatics and data management) and [[Actors/CATI\|CATI]] (neuroimaging) and, with open science compliance implemented through [[Platforms/OPIDoR\|OPIDoR]] and [[Platforms/HAL\|HAL]].

## Core Facilities

### CENIR — Centre de NeuroImagerie de Recherche
https://cenir.institutducerveau.org — Human neuroimaging research centre. Equipment: 3T MRI (×2), simultaneous PET-MRI (Siemens Biograph mMR), MEG (Elekta Neuromag), EEG, TMS, eye-tracking. Supports structural, functional, diffusion, spectroscopy, and molecular imaging. Data managed via [[Actors/CATI\|CATI]] pipelines; primary site for MEMENTO, INSIGHT-preAD, and iShare cohorts.

### CATI — Centre d'Acquisition et de Traitement des Images
https://cati-neuroimaging.com — French national neuroimaging data management centre. HQ at [[Actors/CEA\|CEA]] NeuroSpin; also hosted at [[Actors/Paris Brain Institute\|ICM]]. Manages neuroimaging data for [[Actors/Paris Brain Institute\|ICM]]-associated multisite cohort studies. See [[Actors/CATI\|CATI]].

## ICM.Quant — Quantitative Microscopy
https://quant.institutducerveau.org — Advanced light microscopy; [[Governance/France BioImaging\|France BioImaging]] node. Confocal, multiphoton, super-resolution (STED, STORM/PALM), light-sheet, FLIM. FAIR image data management via [[Actors/OME\|OME]] (OMERO); connected to [[Governance/Euro-BioImaging\|Euro-BioImaging]] open access programme.

### HISTOMICS — Histology and Neuropathology
https://histomics.institutducerveau.org — Tissue sectioning, immunohistochemistry, immunofluorescence, in situ hybridisation, digital slide scanning, spatial transcriptomics (10x Visium, 10x Xenium, Slide-seq).

### iGENSEQ — Genomics and Sequencing
https://igenseq.institutducerveau.org — Next-generation sequencing: RNA-seq, whole-exome, whole-genome, targeted panels, single-cell RNA-seq. Data aligned with [[Standards/VCF\|VCF]] and [[Actors/GA4GH\|GA4GH]] standards.

### Banque ADN et Cellules — Biobank
https://banqueadn.institutducerveau.org — Neurological disease biobank: DNA, RNA, cells, CSF, and plasma from neurological patient cohorts. Aligned with [[Governance/BBMRI-ERIC\|BBMRI-ERIC]] standards.

### ICV — Ingénierie Cellulaire et Vectorologie
https://icv.institutducerveau.org — Two sub-units: **CELIS** (cell culture, iPSC generation and differentiation) and **Vectorology** (AAV, lentivirus, adenovirus production for gene therapy and circuit tracing).

### ePHYS — Electrophysiology
https://ephys.institutducerveau.org — Preclinical electrophysiology: in vitro and ex vivo patch-clamp, in vivo recording (Neuropixels, tetrodes), multi-electrode array (MEA), high-density MEA. Data output compatible with [[Standards/NWB\|NWB]].

### PRISME — Behavioural Phenotyping
https://prisme.institutducerveau.org — Human behavioural and cognitive laboratory.

### DAC — Data Analysis Core
https://dac.institutducerveau.org — Bioinformatics, data management and statistical analysis support: RNA-seq, genomics, imaging pipelines, training, consultation. Implements [[Governance/FAIR Principles\|FAIR Principles]], and interfaces with [[Governance/IFB\|IFB]] and [[Platforms/OPIDoR\|OPIDoR]] infrastructure.

### RnD Unit — F.P.Journe Charity Fund
https://rndunit.institutducerveau.org — Custom scientific instrumentation design and fabrication; open library of ICM-developed devices available to the research community.

## Institutional Affiliations
- [[Governance/CNRS Open Science\|CNRS Open Science]]
- [[Governance/Inserm Open Science\|Inserm Open Science]]
- [[Governance/AP-HP\|AP-HP]]
- [[Actors/Sorbonne Universite\|Sorbonne Universite]]

## Standards Used
- Neuroimaging: [[Standards/BIDS\|BIDS]], [[Standards/NIfTI\|NIfTI]], [[Standards/DICOM\|DICOM]]
- Clinical (via [[Governance/AP-HP\|AP-HP]] EDS): [[Standards/OMOP CDM\|OMOP CDM]], [[Standards/ICD-10\|ICD-10]], [[Standards/LOINC\|LOINC]], [[Standards/CCAM\|CCAM]]
- Genomics / rare disease: [[Standards/HPO\|HPO]], [[Standards/ORDO\|ORDO]], [[Standards/MONDO\|MONDO]]

## Platforms Used
- [[Platforms/OpenNeuro\|OpenNeuro]]
- [[Platforms/EBRAINS\|EBRAINS]]
- [[Platforms/Recherche Data Gouv\|Recherche Data Gouv]]
- [[Platforms/OPIDoR\|OPIDoR]]
- [[Platforms/OMERO\|OMERO]]

## Networks and Consortia
- [[Actors/INCF\|INCF]] - via [[Governance/CNRS Open Science\|CNRS Open Science]] French national node
- [[Actors/ENIGMA Consortium\|ENIGMA Consortium]] - ENIGMA-MDD, ENIGMA-STB, ENIGMA-TS working group participation (Baptiste Couvy-Duchesne; Worbe / Hartmann group)
- [[Governance/France Life Imaging\|France Life Imaging]] - via [[Actors/CATI\|CATI]]
- [[Platforms/EBRAINS\|EBRAINS]]
- [[Governance/ECRIN\|ECRIN]] - via [[Governance/AP-HP\|AP-HP]] / [[Actors/CIC Neurosciences\|CIC Neurosciences]]
- [[Governance/GT-GeDeM\|GT-GeDeM]] - RTmfm working group on microscopy data management (DAC participates)
- [[Governance/IFB\|IFB]] - via [[Actors/DAC\|DAC]]
- [[Governance/France BioImaging\|France BioImaging]] - via [[Actors/Paris Brain Institute\|ICM]] Quant microscopy platform
- [[Actors/CIC Neurosciences\|CIC Neurosciences]] - Inserm/AP-HP clinical investigation centre hosted at [[Actors/Paris Brain Institute\|ICM]]; Phase I–III neurological trials
- [[Actors/iCRIN\|iCRIN]] — [[Actors/Paris Brain Institute\|ICM]] translational clinical research programme; 13 disease-area projects bridging AP-HP clinical services and [[Actors/Paris Brain Institute\|ICM]] research teams

## French Policy Context
- [[Governance/Ouvrir la Science\|Ouvrir la Science]]
- [[Governance/CoSO\|CoSO]]
- [[Governance/ANR Open Science Policy\|ANR Open Science Policy]]

## Paris Open Science Peers
See the MOC Paris Peer Institutions section for a full list. Key co-located partners:
- [[Actors/Institut Pasteur\|Institut Pasteur]], [[Actors/Institut Curie\|Institut Curie]], [[Actors/Institut de Myologie\|Institut de Myologie]], [[Actors/Sorbonne Universite\|Sorbonne Universite]]

## Resources
- https://institutducerveau-icm.org
- https://parisbraininstitute.org/media/410/download (Data Policy)
- https://parisbraininstitute.org/media/2655/download (Ethics and Professional Conduct Charter)
- https://parisbraininstitute.org/our-commitments (commitments overview page)
- https://ror.org/050gn5214 (ROR ID — [[Standards/ROR\|ROR]])
- https://scicrunch.org/resolver/SCR_026379 (RRID:SCR_026379 — Institutional [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_026138 (RRID:SCR_026138 — DAC  [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_026393 (RRID:SCR_026393 — ICM.Quant [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_026412 (RRID:SCR_026412 — ePHYS [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_026394 (RRID:SCR_026394 — PRISME [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_028275 (RRID:SCR_028275 — HISTOMICS [[Standards/RRID\|RRID]])
- https://scicrunch.org/resolver/SCR_028048 (RRID:SCR_028048 — ICV [[Standards/RRID\|RRID]])
- https://cati-neuroimaging.com
