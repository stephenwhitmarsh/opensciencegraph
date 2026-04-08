---
{"dg-publish":true,"permalink":"/02-standards/neuro-ml/","dg-note-properties":{"name":"Neural Open Markup Language","aliases":["NeuroML","NeuroML2"],"website":"https://neuroml.org","type":"standard","scope":"international","domain":["computational","electrophysiology"],"status":"active","founded":2001,"parent_org":"INCF"}}
---


# NeuroML - Neural Open Markup Language

## Overview
NeuroML is a community standard for describing biologically detailed computational
models of neurons and neural networks in an XML-based, simulator-independent format.
It covers neuronal morphology, ion channel dynamics, synaptic mechanisms, and full
network connectivity. Endorsed by [[01_Actors/INCF\|INCF]] and now in its mature NeuroML2 version,
it underpins a broad ecosystem of interoperable tools for model construction,
validation, and simulation across NEURON, NEST, MOOSE, and other simulators.

## Created / Governed By
- [[01_Actors/INCF\|INCF]] — endorsing organisation; NeuroML developed through INCF multiscale modeling program
- Open Source Brain community — active development and model sharing platform

## Key Features
- Simulator-independent XML description of neurons, channels, synapses, and networks
- LEMS (Low Entropy Model Specification) for formal, executable model descriptions
- pyNeuroML and jNeuroML libraries for programmatic model building and conversion
- NeuroML-DB — searchable database of NeuroML models
- Open Source Brain (OSB) — web platform for collaborative model development

## Key Outputs
- NeuroML2 specification (versioned, open)
- Conversion tools to/from NEURON, GENESIS, MOOSE, Brian, NEST
- Blue Brain Python Optimisation Library (BluePyOpt) NeuroML export
- NetPyNE — multiscale modelling environment using NeuroML

## Connections
- Endorsed by: [[01_Actors/INCF\|INCF]]
- Complements: [[02_Standards/NWB\|NWB]] (experimental data), [[02_Standards/BIDS\|BIDS]] (dataset organisation)
- Archived on: Open Source Brain, ModelDB
- Related standards: NineML (network-level modelling language)
- Relevant to: [[03_Platforms/EBRAINS\|EBRAINS]] (Blue Brain Project models)

## Resources
- https://neuroml.org
- https://github.com/NeuroML
- https://www.opensourcebrain.org
- https://neuroml-db.org
