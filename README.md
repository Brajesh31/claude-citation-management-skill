# Citation Management

Comprehensive citation management for academic research. Search Google Scholar and PubMed for papers, extract accurate metadata, validate citations, and generate properly formatted BibTeX entries. This skill should be used when you need to find papers, verify citation information, convert DOIs to BibTeX, or ensure reference accuracy in scientific writing.

## Overview

This repository preserves the original AITMPL skill definition, reference documentation, reusable assets, and scripts at their original relative paths.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-citation-management-skill.git ~/.claude/skills/citation-management
```

On Windows, use `%USERPROFILE%\.claude\skills\citation-management` as the destination.

## Usage

Claude Code can load this skill when a request matches its description. Invoke directly with `/citation-management` when appropriate.

## Repository structure

```text
citation-management/
├── SKILL.md
├── assets/bibtex_template.bib
├── assets/citation_checklist.md
├── references/bibtex_formatting.md
├── references/citation_validation.md
├── references/google_scholar_search.md
├── references/metadata_extraction.md
├── references/pubmed_search.md
├── scripts/doi_to_bibtex.py
├── scripts/extract_metadata.py
├── scripts/format_bibtex.py
├── scripts/search_google_scholar.py
├── scripts/search_pubmed.py
├── scripts/validate_citations.py
├── README.md
└── LICENSE
```

## Runtime requirements

- Python 3 for included Python scripts
- Check the scripts for package imports and API requirements before execution.
- Network-backed citation lookups may require external connectivity and service availability.
- No scripts or tests are claimed as executed.
