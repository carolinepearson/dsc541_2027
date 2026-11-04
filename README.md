# CDISC Pilot eTFL Repository

This repository contains a demonstration clinical study package based on the CDISC Pilot / eTFL Portal example. It is organized around a realistic ADaM analysis dataset, supporting metadata, study documents, and a finalized table shell/output for a demographic summary.

## Overview

The project includes:
- ADaM analysis data (`ADSL`) and metadata (`define.xml`)
- Analysis results metadata in JSON and Excel formats
- Study protocol, SAP, CRF, and shell documents
- Final table output in RTF format

This material is useful for learning and practicing CDISC standards, ADaM data structure, TLF generation, and clinical programming workflows.

## Repository structure

Folder structure for source datasets, table metadata, generated study artifacts, and output directory.
.
├── README.md
└── draft1/
    ├── adamdata/
    │   ├── adsl.sas7bdat
    │   ├── adsl.xpt
    │   ├── define.xml
    │   └── define2-1-0.xsl
    ├── arsdata/
    │   ├── fda-dm-t02-ars.json
    │   └── fda-dm-t02-ars.xlsx
    ├── docs/
    │   ├── Lzzt_protocol_redacted.pdf
    │   ├── blankcrf.pdf
    │   ├── cdiscpilot01.pdf
    │   ├── sap-cdisc-pilot-study.pdf
    │   ├── sdtmadampilotprojectreport.pdf
    │   └── shells/
    │       ├── fda-dm-t02-shell.pdf
    │       └── fda-dm-t02-shell.rtf
    ├── output/
    │   └── fda-dm-t02.rtf
    └── ...
```

## Key folders

### `draft1/adamdata/`
Contains the analysis data package for the study:
- `adsl.xpt` and `adsl.sas7bdat`: subject-level analysis dataset
- `define.xml`: CDISC Define-XML metadata describing the dataset and variables
- `define2-1-0.xsl`: stylesheet used to render the Define-XML metadata

### `draft1/arsdata/`
Contains analysis results support files:
- `fda-dm-t02-ars.json`: structured analysis-results metadata
- `fda-dm-t02-ars.xlsx`: spreadsheet version of the analysis results package

### `draft1/docs/`
Contains study and programming reference documents:
- protocol and SAP
- blank CRF
- project report and supporting materials
- table shells used to define the planned output

### `draft1/output/`
Contains generated deliverables, including the final RTF table output:
- `fda-dm-t02.rtf`: demographic and clinical characteristics table for the safety population

## Intended use

This repository is intended for:
- CDISC and ADaM learning exercises
- clinical data standards review
- table-shell and analysis-output development
- data-definition and metadata inspection
- practice with SAS, R, Python, or XML-based validation workflows

## Notes

- The content is based on the CDISC Pilot dataset and related eTFL examples.
- The package is organized as a study artifact repository rather than a software application.
- Files are provided for educational, validation, and demonstration purposes.

## Suggested next steps

- Review `define.xml` to understand the ADaM metadata and variable definitions.
- Open the protocol and SAP for study context.
- Compare the shell documents `draft1/docs/` with the final output in `draft1/output/`.
- Use the analysis results files to understand how the table was specified and structured.
