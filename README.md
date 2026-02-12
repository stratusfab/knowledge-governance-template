# Knowledge Governance Template

This repository is a domain‑agnostic template for constructing and maintaining canonical truth from messy, multi‑format source material. It provides a structured workflow, governance rules, ingestion processes, and audit mechanisms that can be applied to any project where truth must be synthesized from raw evidence.

This repo is intended to be **forked** for each new project.  
The template itself should remain clean, stable, and domain‑neutral.

---

## When to Fork vs. When to Clone

### Fork this repo when:
- You are starting a new project
- You want to build a domain‑specific truth system (marketing, aircraft proposals, engineering documentation, etc.)
- You want to ingest raw assets and generate canonical files
- You want to customize workflows, directories, or canonical structures

### Clone this repo only when:
- You are contributing improvements to the template itself
- You are updating governance rules
- You are refining workflows or directory structures
- You are maintaining the template as the master reference

If you clone this repo for a new project by mistake, AI tools (including Copilot) should prompt you to fork it instead.

---

## AI Behavior Expectations

When this repo is opened in an AI‑assisted environment (VS Code with Copilot, Codespaces, etc.), the AI should:

1. Detect that this is the **template**, not a project repo.
2. Ask the user whether they intend to:
   - fork the template for a new project, or  
   - modify the template itself.
3. If the user intends to start a new project:
   - instruct them to fork the repo  
   - guide them through setting project intent  
   - scaffold domain‑specific canonical files  
   - prepare ingestion and audit workflows  
4. If the user intends to modify the template:
   - proceed normally  
   - maintain domain‑agnostic structure  
   - avoid adding project‑specific content  

This ensures the template remains clean and reusable.

---

## What This Template Provides

- A governance model for truth construction  
- Canonical vs. raw asset separation  
- Ingestion workflow  
- Audit workflow  
- AI model usage guidance  
- MCP integration guidance  
- Directory scaffolding  
- Canonical file templates  
- Project intent initializer  

These components work together to create a repeatable, auditable system for synthesizing truth from raw evidence.

---

## How to Start a New Project

1. **Fork this repository** into your GitHub account or organization.
2. Clone your fork locally or open it in Codespaces.
3. Fill out `PROJECT-INTENT.md` to define the domain and purpose.
4. Add raw materials to `/assets-raw`.
5. Begin the ingestion workflow:
   - extract claims  
   - compare  
   - synthesize  
   - update canonical files  
6. Run audits regularly to maintain consistency and governance compliance.

---

## Maintaining the Template

If you are improving the template itself:

- Keep all files domain‑neutral  
- Update governance rules only when they apply universally  
- Avoid adding project‑specific examples unless clearly marked  
- Maintain backward compatibility for existing forks when possible  

Changes to the template should improve clarity, structure, or workflow without locking it into a specific domain.

---

## License

This template is intended for internal use and adaptation.  
Use, fork, and modify as needed for your projects.
