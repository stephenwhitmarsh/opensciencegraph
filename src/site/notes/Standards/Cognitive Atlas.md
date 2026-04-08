---
{"dg-publish":true,"permalink":"/standards/cognitive-atlas/","tags":["icm/uses"],"dg-note-properties":{"name":"Cognitive Atlas","aliases":["Cognitive Atlas ontology"],"website":"https://www.cognitiveatlas.org","type":"terminology","scope":"international","domain":["neuroimaging","behavior"],"status":"active","founded":2011,"parent_org":"Poldrack Lab / Stanford University","tags":["icm/uses"]}}
---


# Cognitive Atlas

## Overview
The Cognitive Atlas is a collaborative ontology of cognitive processes and psychological tasks used in neuroimaging research, developed by the Poldrack Lab at Stanford University. It provides a controlled vocabulary of mental processes (e.g. working memory, cognitive control, episodic memory) and the experimental tasks that measure them (e.g. N-back task, Stroop task, word recognition). Its primary function in the open neuroscience ecosystem is to enable **semantic cross-study comparison** of fMRI datasets: when datasets from different labs annotate their tasks using Cognitive Atlas terms, automated meta-analysis tools like Neurosynth can query which brain regions activate across studies measuring "working memory" regardless of task implementation.

## Role in the Neuroimaging Ecosystem
- **[[Standards/BIDS\|BIDS]]** — the `task` metadata field in BIDS datasets can reference Cognitive Atlas task identifiers, enabling formal semantic task description
- **[[Platforms/NeuroVault\|NeuroVault]]** — requires Cognitive Atlas task annotation for all uploaded statistical maps; powers the Neurosynth integration
- **[[Platforms/OpenNeuro\|OpenNeuro]]** — encourages Cognitive Atlas annotation for fMRI datasets
- **Neurosynth** — uses Cognitive Atlas term co-occurrence for large-scale automated meta-analysis of brain-behaviour relationships

## Key Concepts
The ontology has two main branches:
- **Cognitive concepts** — mental processes with formal definitions and hierarchical relationships (e.g. memory → episodic memory → autobiographical memory)
- **Tasks** — specific experimental paradigms linked to the concepts they measure (e.g. digit span task → measures short-term memory)

## Connections
- Used with: [[Standards/BIDS\|BIDS]] (task annotation), [[Platforms/NeuroVault\|NeuroVault]] (required annotation), [[Platforms/OpenNeuro\|OpenNeuro]] (fMRI datasets)
- Complements: [[Standards/HED\|HED]] (event-level annotation), [[Standards/UBERON\|UBERON]] (brain region annotation)
- Relevant to: [[Actors/Paris Brain Institute\|Paris Brain Institute]] (fMRI studies, cognitive neuroscience)

## Resources
- https://www.cognitiveatlas.org
- https://www.cognitiveatlas.org/api (REST API for programmatic access)
