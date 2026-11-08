# claude-citation-management-skill

A Claude Code skill for finding, validating, formatting, and maintaining accurate academic citations and bibliographies.

## Overview

Citation management is a data-quality task as much as a writing task. A correct reference needs accurate authorship, title, publication details, identifiers, and formatting. This skill helps organize the process from literature search through metadata extraction, validation, BibTeX generation, and bibliography cleanup.

## Main Capabilities

- Search for academic papers using supported scholarly databases.
- Retrieve metadata from identifiers such as DOI, PMID, and arXiv ID.
- Extract authors, title, journal, year, volume, issue, pages, and identifiers.
- Generate and format BibTeX entries.
- Validate existing references against publication records.
- Detect duplicate or incomplete citations.
- Normalize bibliography fields.
- Prepare references for manuscripts, theses, and research reports.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-citation-management-skill.git ~/.claude/skills/citation-management
```

Install the Python dependencies required by the scripts. Network-backed search and metadata retrieval require connectivity and may depend on service availability.

## Usage

Invoke the skill for citation and bibliography tasks:

```text
/citation-management
```

Provide the reference list, DOI or PMID identifiers, target citation style, and any constraints on database access.

## Typical Workflow

1. Search for the required paper or resolve its identifier.
2. Retrieve metadata from an appropriate record.
3. Compare the returned metadata with the actual publication details.
4. Generate or update the BibTeX entry.
5. Validate required fields and identifier consistency.
6. Detect duplicates and incomplete records.
7. Format the bibliography consistently.
8. Preserve the query and validation steps for reproducibility.

## Repository Structure

```text
claude-citation-management-skill/
├── SKILL.md
├── assets/
│   ├── bibtex_template.bib
│   └── citation_checklist.md
├── references/
│   ├── bibtex_formatting.md
│   ├── citation_validation.md
│   ├── google_scholar_search.md
│   ├── metadata_extraction.md
│   └── pubmed_search.md
└── scripts/
    ├── doi_to_bibtex.py
    ├── extract_metadata.py
    ├── format_bibtex.py
    ├── search_google_scholar.py
    ├── search_pubmed.py
    └── validate_citations.py
```

## Script Responsibilities

| Script | Purpose |
|---|---|
| `doi_to_bibtex.py` | Resolve DOI metadata into BibTeX |
| `extract_metadata.py` | Extract publication metadata |
| `format_bibtex.py` | Normalize BibTeX formatting |
| `search_google_scholar.py` | Search scholarly records |
| `search_pubmed.py` | Search biomedical literature |
| `validate_citations.py` | Check citation completeness and consistency |

Check command-line options in each script before use.

## Validation Checklist

- Author names and order are correct.
- Publication title matches the record.
- DOI or PMID resolves to the intended paper.
- Journal, year, volume, issue, and pages are checked where applicable.
- Citation style is applied consistently.
- Duplicate records are identified.
- Missing metadata is not silently invented.
- Bibliography output is reviewed before submission.

## Repository Contents

- `SKILL.md`: Main citation-management workflow.
- `assets/`: BibTeX template and validation checklist.
- `references/`: Search, metadata, formatting, and validation guidance.
- `scripts/`: Citation retrieval and processing utilities.
- `README.md`: Setup and usage documentation.

## Research Integrity

Never fill missing citation fields by guessing. If metadata sources disagree, preserve the discrepancy and verify the publication record. A formatted citation is not necessarily an accurate citation until its underlying metadata has been checked.
