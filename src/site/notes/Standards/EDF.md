---
{"dg-publish":true,"permalink":"/standards/edf/","tags":["icm/uses"],"dg-note-properties":{"name":"European Data Format","aliases":["EDF","EDF+","European Data Format Plus"],"website":"https://www.edfplus.info","type":"standard","scope":"international","domain":["electrophysiology","clinical"],"status":"active","founded":1992,"parent_org":"EDF+ community (Bob Kemp / Josip Värri; no formal governance body)","tags":["icm/uses"]}}
---


# EDF / EDF+ — European Data Format

## Overview
EDF (European Data Format) is the long-established open file format for storing and exchanging multichannel biosignal recordings — most importantly clinical and research EEG, polysomnography (PSG/sleep studies), and other continuous physiological time-series. Proposed by Bob Kemp and Josip Värri in 1992 and published in *Electroencephalography and Clinical Neurophysiology*, EDF became the de facto standard for clinical neurophysiology long before NWB or BIDS existed, and remains the format in which virtually all clinical EEG systems export data worldwide. EDF+ (2003) extended the format to support annotations, discontinuous recordings, and a wider range of signal types.

At [[Actors/Paris Brain Institute\|Paris Brain Institute]] and [[Governance/AP-HP\|AP-HP]], EDF/EDF+ is the primary format for clinical EEG, long-term video-EEG monitoring, polysomnography, and stereo-EEG (SEEG) recordings produced at [[Actors/CENIR\|CENIR]] and the clinical neurology service at Pitié-Salpêtrière. It is the format that must be converted or wrapped when depositing electrophysiology data into open repositories in [[Standards/BIDS\|BIDS]] format.

## Format Structure
An EDF file consists of:
- **Header** — ASCII-encoded, fixed-length; stores patient ID, recording start time, number of signals, sampling rates, physical and digital min/max, transducer types, and signal labels
- **Data records** — fixed-duration blocks (typically 1–30 seconds) storing interleaved integer samples for each channel in sequence; each channel has its own sampling rate

EDF+ adds:
- **Annotations channel (EDF Annotations)** — a special signal channel storing time-stamped text annotations (seizure markers, sleep stage labels, stimulus events) as UTF-8 strings with onset and duration
- **Discontinuous recordings** — EDF+D allows recording gaps to be marked explicitly, enabling storage of non-continuous data
- **Reserved field usage** — clarifies header field interpretation for clinical applications

## Key Properties
- **Simplicity** — 256-byte header per signal, integer sample storage; readable by any language without a library
- **Universal support** — native export from every major clinical EEG system (Natus, Nicolet, Micromed, Brain Products, BioSemi, Compumedics, Nihon Kohden)
- **Clinical annotations** — EDF+ annotations channel carries IEC 60601-compliant event codes and free-text labels
- **Precision limitations** — integer storage with fixed physical range means precision is limited by resolution = (physical max − min) / 2^bits; 16-bit storage is standard; 24-bit extensions exist but are non-standard
- **No built-in metadata model** — EDF header fields are minimal; extended metadata (electrode coordinates, subject demographics, task structure) must be stored separately in sidecar files

## EDF in the Open Neuroscience Ecosystem

### BIDS integration
[[Standards/BIDS\|BIDS]] supports EDF/EDF+ as one of the accepted file formats for EEG, iEEG, and MEG data (alongside BrainVision .vhdr/.vmrk/.eeg and MEFD). In a BIDS dataset, the EDF file is stored unchanged; task metadata, channel information, electrode coordinates, and event descriptions are stored in companion `.tsv` and `.json` sidecar files. The BIDS EEG specification explicitly accommodates EDF's annotation channel for event information. Tools such as **MNE-BIDS** automate EDF-to-BIDS conversion.

### NWB relationship
[[Standards/NWB\|NWB]] stores EEG and iEEG data in HDF5 with rich metadata but is not used clinically. The typical pipeline for clinical-to-open data is: EDF (clinical acquisition) → [[Standards/BIDS\|BIDS]] (organisation and metadata) → optionally [[Standards/NWB\|NWB]] (if depositing on [[Platforms/DANDI Archive\|DANDI Archive]]). MNE-Python can read EDF directly and export to both BIDS and NWB.

### OpenNeuro and DANDI
[[Platforms/OpenNeuro\|OpenNeuro]] accepts BIDS-organised EDF datasets; [[Platforms/DANDI Archive\|DANDI Archive]] requires [[Standards/NWB\|NWB]] format, so EDF data must be converted before DANDI deposit. Several large open EEG datasets on OpenNeuro (e.g. the Temple University Hospital EEG Corpus, TUAB) are distributed in EDF format within BIDS structure.

## Clinical Relevance at ICM
- **[[Actors/CENIR\|CENIR]]** — EEG (scalp, high-density), MEG (Elekta Neuromag raw data converted to FIF, but EDF used for clinical EEG exports)
- **Clinical EEG service (Pitié-Salpêtrière / [[Governance/AP-HP\|AP-HP]])** — long-term video-EEG monitoring for epilepsy diagnosis; all clinical EEG recorded and stored in EDF/EDF+ by Natus/Nihon Kohden systems
- **SEEG (stereo-EEG)** — intracranial EEG for pre-surgical epilepsy evaluation; recordings exported from Micromed/Nihon Kohden in EDF; used by BIDS iEEG specification
- **Polysomnography** — sleep EEG studies for sleep disorders and neurodegenerative disease; EDF is the international standard export format

## Related / Successor Formats
- **MEF3** (Millisecond Extreme Format) — compressed, encrypted iEEG format from Mayo Clinic / MNI; used for long-term implanted device recordings; not widely adopted outside epilepsy monitoring centres
- **[[Standards/BrainVision\|BrainVision]] format** (.vhdr/.vmrk/.eeg) — widely used in research EEG (Brain Products hardware); also accepted by BIDS
- **FIF** (Functional Imaging File) — native format of Elekta/MEGIN MEG systems and MNE-Python; used at [[Actors/CENIR\|CENIR]] for MEG data

## Connections
- Used with: [[Standards/BIDS\|BIDS]] (EEG, iEEG, MEG modalities; EDF accepted alongside BrainVision and FIF)
- Converts to: [[Standards/NWB\|NWB]] (via MNE-Python for DANDI deposit)
- Event annotation: [[Standards/HED\|HED]] (HED tags can annotate EDF+ annotation channel events in BIDS)
- Clinical context: [[Governance/AP-HP\|AP-HP]] (clinical EEG recording and archiving), [[Actors/CENIR\|CENIR]] (research EEG)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (clinical EEG, SEEG, polysomnography; BIDS iEEG datasets)
- Related formats: [[Standards/NWB\|NWB]] (research electrophysiology archive format), [[Standards/DICOM\|DICOM]] (clinical imaging equivalent)

## Resources
- https://www.edfplus.info (EDF+ specification and tools)
- https://www.edfplus.info/specs/edf.html (EDF specification — Kemp et al. 1992)
- https://www.edfplus.info/specs/edfplus.html (EDF+ specification — Kemp & Värri 2003)
- https://mne.tools/stable/generated/mne.io.read_raw_edf.html (MNE-Python EDF reader)
- https://bids-specification.readthedocs.io/en/stable/modality-specific-files/electroencephalography.html (BIDS EEG — EDF accepted format)
