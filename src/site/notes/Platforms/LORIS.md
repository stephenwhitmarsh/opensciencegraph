---
{"dg-publish":true,"permalink":"/platforms/loris/","dg-note-properties":{"name":"Longitudinal Online Research and Imaging System","aliases":["LORIS"],"website":"https://loris.ca","type":"platform","scope":"international","domain":["neuroimaging","clinical"],"status":"active","founded":2002,"parent_org":"McGill University / MCIN"}}
---


# LORIS — Longitudinal Online Research and Imaging System

## Overview
LORIS (Longitudinal Online Research and Imaging System) is an open-source web-based data and project management platform for neuroimaging and clinical research, developed and maintained by the **McGill Centre for Integrative Neuroscience (MCIN)** at the Montreal Neurological Institute (MNI), McGill University. Originally built in 1999 for the NIH MRI Study of Normal Brain Development (NIHPD), LORIS has grown into a comprehensive framework for managing multimodal longitudinal and multisite datasets — integrating neuroimaging, clinical, behavioural, electrophysiology, biospecimen, and genetic data in a single secure web-accessible database.

LORIS is primarily a Canadian platform but has an international user community spanning 4 continents and 400+ research sites. Its deployment model is self-hosted: institutions download and operate their own LORIS instance, with the MCIN core team providing development, governance, and community support.

## Key Features
- DICOM ingestion, automated QC, and [[Standards/BIDS\|BIDS]] conversion pipelines
- Longitudinal and multisite study management with role-based access control
- RESTful API for integration with processing pipelines and external platforms
- Federated data sharing via [[Actors/CONP\|CONP]] portal integration
- [[Standards/CDISC\|CDISC]]-compatible data export for regulatory submissions
- Interfaces with [[Platforms/XNAT\|XNAT]] (imaging data exchange) and [[Platforms/Neurobagel\|Neurobagel]] (federated cohort search)

## Confirmed Institutional Users and Projects

### Canada (primary user base)
- **McGill University / MNI / MCIN** — origin and development hub; PreventAD, StoP-AD, C-BIG (TOSI open biobank), EEGNet
- **[[Actors/TOSI\|TOSI]]** — Tanenbaum Open Science Institute; C-BIG Repository runs on LORIS
- **[[Actors/Ontario Brain Institute\|Ontario Brain Institute]] / [[Platforms/Brain-CODE\|Brain-CODE]]** — Brain-CODE federates with LORIS at McGill for neuroimaging data exchange
- **[[Actors/CONP\|CONP]]** — Canadian Open Neuroscience Platform; LORIS is one of the primary backend platforms; all LORIS-hosted datasets registered on the CONP portal
- **CCNA** (Canadian Consortium on Neurodegeneration in Aging) — multisite dementia cohort
- **QPN / C-OPN** — Quebec Parkinson Network / Canadian Open Parkinson Network
- **IBIS Network** — Infant Brain Imaging Study (autism); multisite infant neuroimaging
- **HBCD** — Healthy Brain and Child Development study (addiction/neurodevelopment)
- **CAPTURE** — ALS multisite study

### International
- **[[Actors/ADNI\|ADNI]]** — Alzheimer's Disease Neuroimaging Initiative; one of LORIS's earliest large-scale multisite deployments
- **GUSTO** — birth cohort study, Singapore
- **Indian Dementia Network / National Brain Research Centre** — India
- **European Alzheimer's Network** — multisite European deployment

## Connections
- Developed by: McGill MCIN (Montreal Neurological Institute / McGill University)
- Used by: [[Actors/ADNI\|ADNI]], [[Actors/CONP\|CONP]], [[Actors/TOSI\|TOSI]], [[Actors/Ontario Brain Institute\|Ontario Brain Institute]] / [[Platforms/Brain-CODE\|Brain-CODE]]
- Interoperates with: [[Platforms/XNAT\|XNAT]] (imaging data), [[Platforms/Neurobagel\|Neurobagel]] (federated cohort search), [[Platforms/OpenNeuro\|OpenNeuro]] (public data release)
- Standards: [[Standards/BIDS\|BIDS]], [[Standards/DICOM\|DICOM]], [[Standards/CDISC\|CDISC]]
- Related platforms: [[Platforms/XNAT\|XNAT]] (comparable imaging management platform)

## Resources
- https://loris.ca
- https://github.com/aces/Loris (source code)
- https://demo.loris.ca (public demo instance)
- https://mcin.ca/technology/loris/ (MCIN overview)
