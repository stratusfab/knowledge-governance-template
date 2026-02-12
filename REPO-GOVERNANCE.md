# REPO-GOVERNANCE.md

## Purpose
This repository provides a structured, version-controlled system for constructing and maintaining truth within any domain. It replaces scattered, conflicting, or outdated materials with a clean, auditable knowledge base that supports consistent decision-making and AI-assisted content generation.

The repo is not a storage dump. It is a truth-construction engine.

## Scope
This governance applies to any project domain. Examples include marketing, technical documentation, aircraft configuration, proposal development, engineering, regulatory work, or internal process design.

The repo adapts to the domain defined during initialization.

## Canonical vs Raw
The repo is divided into two zones:

1. Canonical  
   These files represent the current, approved truth. They are written in Markdown and intentionally maintained. AI tools should rely only on canonical files when generating content.

2. Raw  
   This contains unverified, unstructured, or conflicting materials. PDFs, images, spreadsheets, diagrams, legacy documents, and other artifacts belong here. Raw assets are evidence, not truth.

## Truth Construction
Truth is synthesized from raw evidence. The process is:

1. Select a raw asset.  
2. Extract meaningful claims into a temporary Markdown file.  
3. Compare those claims with existing canonical files and other evidence.  
4. Decide what is accurate, current, and relevant.  
5. Update canonical files accordingly.  
6. Commit changes with a clear explanation of what changed and why.

Truth is defined by the canonical files at each commit.

## Directory Structure
Initial structure:

/canonical
/assets-raw
/assets-processed
/workflows

Additional directories may be added based on project intent.


Additional directories may be added based on project intent.

## Ingestion Workflow
1. Place new materials into /assets-raw.  
2. Do not treat raw assets as authoritative.  
3. Extract claims into a temporary Markdown file.  
4. Compare and synthesize.  
5. Update canonical files.  
6. Move processed raw assets into /assets-processed or a subfolder such as superseded, conflicting, or irrelevant.

## Conflict Handling
Conflicts between sources are expected. When they occur:

1. Identify the conflict.  
2. Determine which claim aligns with current reality.  
3. If neither is correct, rewrite the claim into a new, accurate version.  
4. Document the decision in the commit message.  
5. Move conflicting raw assets to an appropriate subfolder.

## Auditing
Auditing is externalized:

1. AI-based governance audits  
   AI tools review the repo against this governance file, checking for structural violations, inconsistencies, outdated claims, missing metadata, and drift.

2. Human-in-the-loop review  
   A human reviews audit findings and updates canonical files as needed.

3. Structural audits via MCP  
   MCP enforces directory structure, naming conventions, metadata presence, and detection of unprocessed raw assets.

## AI Usage
AI tools may:

- summarize raw assets  
- highlight contradictions  
- propose canonical updates  
- generate audit reports  
- assist with structuring new content  
- enforce governance rules during content creation

AI tools may not:

- treat raw assets as authoritative  
- update canonical files without human approval  
- override governance rules  
- infer truth without evidence

## Commit Standards
Commits that modify canonical files must include:

- what changed  
- why it changed  
- which raw assets informed the decision  
- whether conflicts were resolved  
- where raw assets were moved

## MCP Integration
MCP may:

- fetch files from approved directories  
- detect new raw assets  
- enforce directory structure  
- identify unprocessed materials  
- validate naming conventions  
- support ingestion workflows

MCP does not determine truth. It supports the workflow that leads to truth.

## Maturity Model
The repo becomes useful as soon as the first canonical file exists. Usefulness increases as more raw assets are processed and canonical truth stabilizes. The system compounds in value over time.
