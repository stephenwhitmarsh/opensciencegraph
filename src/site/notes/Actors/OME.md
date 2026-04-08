---
{"dg-publish":true,"permalink":"/actors/ome/","dg-note-properties":{"name":"Open Microscopy Environment","aliases":["OME","OME Consortium"],"website":"https://www.openmicroscopy.org","type":"consortium","scope":"international","domain":["bioimaging"],"status":"active","founded":2001,"parent_org":"University of Dundee / German BioImaging (coordinating)"}}
---


# OME - Open Microscopy Environment

## Overview
The Open Microscopy Environment is a consortium of universities, research laboratories, industry partners, and developers producing open-source software and data format standards for biological microscopy. Founded in 2001 by Jason Swedlow, Ilya Goldberg, and Peter Sorger, OME is to microscopy what [[Actors/INCF\|INCF]] is to neuroscience informatics — the central community body that defines how imaging data is formatted, stored, and shared. Its products underpin the data infrastructure of [[Governance/Euro-BioImaging\|Euro-BioImaging]], [[Governance/France BioImaging\|France BioImaging]], and all major bioimaging repositories. Core development is led by the University of Dundee and German BioImaging.

## Standards Produced
- [[Standards/OME File Formats\|OME File Formats]] — the OME file format family: OME-TIFF (metadata-rich TIFF) and OME-Zarr (cloud-native next-generation format)
- OME-XML — the underlying metadata model embedded in OME-TIFF
- Bio-Formats — Java library reading 150+ proprietary microscopy formats and converting them to OME-TIFF; the dcm2niix equivalent for microscopy
- OMERO — client-server platform for managing, visualising, and sharing microscopy images and metadata; deployed at Euro-BioImaging nodes worldwide

## Key Products
- **Bio-Formats** — reads Zeiss .czi, Leica .lif, Nikon .nd2, and 150+ other proprietary formats; converts to OME-TIFF for interoperability
- **OMERO** — institutional image data management server; used at core facilities, national nodes (France BioImaging), and Euro-BioImaging nodes
- **OME-TIFF** — metadata-embedded TIFF standard; stable format for archiving and publication
- **OME-Zarr (OME-NGFF)** — cloud-optimised chunked format for large multidimensional datasets; the future-facing successor to OME-TIFF
- **IDR (Image Data Resource)** — public reference image repository hosted at EMBL-EBI using OMERO; complements the BioImage Archive

## Connections
- Standards produced: [[Standards/OME File Formats\|OME File Formats]]
- Platform produced: [[Platforms/OMERO\|OMERO]] (institutional image management server)
- Deployed by: [[Governance/Euro-BioImaging\|Euro-BioImaging]] (OMERO at all nodes), [[Governance/France BioImaging\|France BioImaging]] (OMERO instances)
- Endorsed by: [[Governance/ELIXIR\|ELIXIR]], [[Governance/EOSC\|EOSC]]
- Integrates with: [[Governance/QUAREP-LiMi\|QUAREP-LiMi]] (metadata and QC standards), [[Standards/REMBI\|REMBI]] (metadata framework), BioImage Archive (EMBL-EBI)
- Related: [[Actors/INCF\|INCF]] (equivalent body for neuroscience data standards), [[Standards/NIfTI\|NIfTI]] (analogous role for MRI data)

## Resources
- https://www.openmicroscopy.org
- https://www.openmicroscopy.org/bio-formats/
- https://www.openmicroscopy.org/omero/
- https://ngff.openmicroscopy.org (OME-NGFF specification)
