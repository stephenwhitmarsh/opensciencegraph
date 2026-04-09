---
{"dg-publish":true,"permalink":"/standards/nwb/","dg-note-properties":{"name":"Neurodata Without Borders","aliases":["NWB","NWB:N"],"website":"https://www.nwb.org","type":"standard","scope":"international","domain":["electrophysiology","multimodal"],"status":"active","founded":2015,"parent_org":"INCF","icon":"https://www.nwb.org/wp-content/uploads/2022/01/NWB-favicon.png"}}
---


# NWB — Neurodata Without Borders

## Overview
NWB (Neurodata Without Borders) is the community standard for neurophysiology
data, covering intracellular and extracellular electrophysiology, calcium imaging,
optogenetics, and behavioural data. Initiated in 2015 with funding from the
[[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]] and co-founded by the [[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]],
NWB addresses the same problem for neurophysiology that [[Standards/BIDS\|BIDS]] addresses for
neuroimaging: the absence of a shared data format had made cross-lab reuse and
meta-analysis of electrophysiology data essentially impossible.

NWB uses **HDF5** (and optionally Zarr) as its underlying container format,
with a rigorously defined schema for organising neural data and all associated
metadata — electrodes, stimulus parameters, trial structure, subject information,
and provenance — into a single, self-describing file. It is governed by [[Actors/INCF\|INCF]]
and the [[Governance/NWB Working Group\|NWB Working Group]], and is the mandatory format for the [[Platforms/DANDI Archive\|DANDI Archive]].

## Data Types Covered
NWB handles the full range of neurophysiology and systems neuroscience data:
- **Extracellular electrophysiology** — spike-sorted unit data, raw LFP,
  electrode geometry (Neuropixels, tetrodes, MEAs)
- **Intracellular electrophysiology** — patch-clamp recordings (current/voltage clamp)
- **Calcium imaging** — two-photon and wide-field fluorescence, ROI segmentations,
  ΔF/F traces
- **Optogenetics** — stimulus parameters, light delivery metadata
- **Behaviour** — positional tracking, task events, stimuli, reward delivery
- **Eye tracking** — pupil size, gaze position
- **Stimulus** — visual, auditory, and other stimulus metadata

## File Format and APIs
- **HDF5 container** — NWB files are HDF5 with a specific schema; any HDF5 library
  can read the raw data, but the NWB APIs provide semantic access
- **PyNWB** — Python API; primary interface for reading/writing NWB files
- **MatNWB** — MATLAB API; widely used in experimental neuroscience labs
- **NWB Explorer** — web-based visualisation tool for exploring NWB files interactively
  without coding (https://nwbexplorer.opensourcebrain.org)

## NWB Data Extensions (NDX)
The **NDX (NWB Data Extension)** mechanism allows community-developed extensions
to the core NWB schema for lab-specific or modality-specific data types:
- Extensions are versioned Python packages published on PyPI and catalogued
  at https://nwb-extensions.github.io
- Examples: `ndx-miniscope` (miniscope calcium imaging), `ndx-events` (flexible
  event types), `ndx-photometry` (fibre photometry)
- Extensions maintain backwards compatibility with the core NWB schema

## Relationship to BIDS
NWB and [[Standards/BIDS\|BIDS]] serve complementary roles and are designed to interoperate:
- **BIDS** organises datasets at the file/directory level across modalities
- **NWB** is a rich single-file format for neurophysiology recording sessions
- BIDS has a BEP (BEP032 — NWB BIDS) for organising NWB files within BIDS structure
- The [[Platforms/DANDI Archive\|DANDI Archive]] supports both NWB files and BIDS-organised NWB datasets

## Key Users and Datasets
- **[[Actors/IBL\|IBL]]** (International Brain Laboratory) — Brain Wide Map; the largest NWB
  dataset to date; Neuropixels recordings from 547 brain regions; fully public on DANDI
- **[[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]]** — Visual Coding and Allen Brain Observatory
  datasets distributed in NWB format
- **[[Actors/BICAN\|BICAN]]** — electrophysiology data from brain atlas projects
- **[[Platforms/DANDI Archive\|DANDI Archive]]** — 400+ public NWB datasets as of 2025

## Connections
- Primary archive: [[Platforms/DANDI Archive\|DANDI Archive]]
- Endorsed by: [[Actors/INCF\|INCF]], [[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]]
- Funded by: [[Actors/NIH BRAIN Initiative\|NIH BRAIN Initiative]] (original development and DANDI partnership)
- Compatible with: [[Standards/BIDS\|BIDS]] (BEP032), [[Standards/HED\|HED]] (event annotation)
- Governed by: [[Governance/NWB Working Group\|NWB Working Group]]
- Adopted by: [[Platforms/EBRAINS\|EBRAINS]], [[Actors/IBL\|IBL]], [[Actors/Allen Institute for Brain Science\|Allen Institute for Brain Science]], [[Actors/BICAN\|BICAN]]
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (ePHYS platform electrophysiology data;
  DANDI deposit for open neurophysiology datasets)

## Resources
- https://www.nwb.org
- https://pynwb.readthedocs.io (PyNWB documentation)
- https://github.com/NeurodataWithoutBorders (GitHub organisation)
- https://dandiarchive.org (DANDI Archive — primary NWB repository)
- https://nwb-extensions.github.io (NDX extension catalogue)
- https://nwbexplorer.opensourcebrain.org (NWB Explorer web viewer)
