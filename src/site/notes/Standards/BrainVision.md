---
{"dg-publish":true,"permalink":"/standards/brain-vision/","tags":["icm/uses"],"dg-note-properties":{"name":"BrainVision Data Format","aliases":["BrainVision","BrainVision Core Data Format",".vhdr",".vmrk",".eeg"],"website":"https://www.brainproducts.com/support-resources/brainvision-core-data-format-1-0/","type":"standard","scope":"international","domain":["electrophysiology"],"status":"active","founded":1996,"parent_org":"Brain Products GmbH","tags":["icm/uses"]}}
---


# BrainVision Data Format

## Overview
The BrainVision Core Data Format is the native file format of Brain Products GmbH EEG hardware and software, and one of the two dominant open research EEG formats (alongside [[Standards/EDF\|EDF]]). Where EDF is the clinical EEG standard — used by hospital systems worldwide — BrainVision is the de facto standard for high-density research EEG, widely adopted because of the ubiquity of Brain Products amplifiers (BrainAmp, actiCHamp, LiveAmp) in cognitive neuroscience and research labs globally. It is one of the three formats explicitly accepted by the [[Standards/BIDS\|BIDS]] EEG specification, alongside EDF and FIF.

At [[Actors/Paris Brain Institute\|Paris Brain Institute]] and [[Actors/CENIR\|CENIR]], BrainVision format is used for high-density EEG recordings acquired with Brain Products systems. It is also the native export format of many EEG labs contributing to [[Actors/ENIGMA Consortium\|ENIGMA Consortium]] working groups and [[Platforms/OpenNeuro\|OpenNeuro]] datasets.

## Format Structure
The BrainVision format is a three-file set — all three files must be present together:

| File | Extension | Content |
|---|---|---|
| Header file | `.vhdr` | Plain-text INI-style file; stores channel names, sampling rate, amplifier settings, data format, reference electrode, and pointers to the marker and data files |
| Marker file | `.vmrk` | Plain-text file; stores all event markers with type, description, position (in samples), and duration |
| Data file | `.eeg` | Binary file; stores the raw sample data as interleaved channel values (16-bit or 32-bit integer, or 32-bit float depending on recording settings) |

This separation of header, events, and data is the key structural difference from [[Standards/EDF\|EDF]], which stores everything in a single file. The plain-text `.vhdr` and `.vmrk` files make the metadata human-readable and easy to parse without specialist libraries.

## Key Properties
- **Open specification** — Brain Products publishes the Core Data Format specification openly; no licence required to read or write the format
- **High-density EEG support** — naturally handles 32–256+ channel systems with individual channel metadata
- **Flexible data precision** — supports 16-bit integer, 32-bit integer, and 32-bit float sample storage; float format avoids the quantisation precision limitations of [[Standards/EDF\|EDF]]'s fixed-range integer encoding
- **Rich event marking** — `.vmrk` stores stimulus and response codes, boundary markers (recording breaks), and custom annotations with type/description fields
- **Reference electrode metadata** — explicit reference channel information in the header, important for EEG re-referencing in analysis
- **No built-in compression** — `.eeg` files are uncompressed binary; large for high-density long recordings

## BrainVision in the Open Neuroscience Ecosystem

### BIDS integration
[[Standards/BIDS\|BIDS]] accepts BrainVision as one of three allowed EEG file formats (with [[Standards/EDF\|EDF]] and FIF). In a BIDS dataset the three files (`.vhdr`, `.vmrk`, `.eeg`) are stored together in the `eeg/` directory alongside the standard BIDS sidecar files (`.json` metadata, `channels.tsv`, `electrodes.tsv`, `events.tsv`). The BIDS EEG specification maps BrainVision header fields directly to BIDS metadata fields, making conversion straightforward. **MNE-BIDS** handles BrainVision-to-BIDS conversion natively.

### MNE-Python ecosystem
MNE-Python reads BrainVision format natively via `mne.io.read_raw_brainvision()`, making it directly usable in the dominant open-source EEG/MEG analysis pipeline. The MNE ecosystem connects BrainVision data to [[Standards/NWB\|NWB]] export (for [[Platforms/DANDI Archive\|DANDI Archive]] deposit), [[Standards/HED\|HED]] event annotation, and [[Platforms/OpenNeuro\|OpenNeuro]] upload via MNE-BIDS.

### OpenNeuro datasets
Many of the largest open EEG datasets on [[Platforms/OpenNeuro\|OpenNeuro]] are distributed in BrainVision format within BIDS structure — particularly datasets from cognitive neuroscience labs running Brain Products hardware, which represents a substantial fraction of research EEG globally.

## Relationship to EDF
BrainVision and [[Standards/EDF\|EDF]] are complementary rather than competing:

| Feature | BrainVision | EDF / EDF+ |
|---|---|---|
| Primary context | Research EEG | Clinical EEG |
| Hardware origin | Brain Products amplifiers | Clinical hospital systems |
| File structure | Three files (.vhdr / .vmrk / .eeg) | Single file |
| Data precision | 16/32-bit int or 32-bit float | 16-bit integer |
| Event storage | Separate .vmrk file | Annotations channel (EDF+) |
| BIDS support | Yes | Yes |
| Clinical use | Rare | Universal |

In practice, research labs often encounter both: Brain Products systems produce BrainVision files for high-density cognitive EEG, while clinical recordings from hospital EEG labs arrive in EDF. Both are converted to BIDS for open data sharing.

## Connections
- Produced by: Brain Products GmbH amplifiers and BrainVision Recorder software
- Used with: [[Standards/BIDS\|BIDS]] (one of three accepted EEG formats)
- Converts to: [[Standards/NWB\|NWB]] (via MNE-Python for [[Platforms/DANDI Archive\|DANDI Archive]] deposit)
- Event annotation: [[Standards/HED\|HED]] (HED tags applied to `.vmrk` events in BIDS)
- Analysis ecosystem: MNE-Python, EEGLAB, BrainVision Analyzer 2
- Related format: [[Standards/EDF\|EDF]] (clinical EEG counterpart; both BIDS-accepted)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (high-density research EEG at [[Actors/CENIR\|CENIR]]; BIDS EEG datasets on [[Platforms/OpenNeuro\|OpenNeuro]])

## Resources
- https://www.brainproducts.com/support-resources/brainvision-core-data-format-1-0/ (Core Data Format specification)
- https://mne.tools/stable/generated/mne.io.read_raw_brainvision.html (MNE-Python reader)
- https://bids-specification.readthedocs.io/en/stable/modality-specific-files/electroencephalography.html (BIDS EEG — BrainVision accepted format)
- https://www.brainproducts.com (Brain Products GmbH)
