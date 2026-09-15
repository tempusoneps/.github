# TempusOnePS Ecosystem README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a comprehensive, professional English README for the TempusOnePS ecosystem across both `profile/README.md` (GitHub Org profile) and `README.md` (repository root).

**Architecture:** The document incorporates organization hero banners, core pillars, an end-to-end Mermaid workflow diagram, categorized repository index tables with direct links to `tempusoneps/*` repos, an end-to-end quant strategy lifecycle guide, and contributor onboarding instructions.

**Tech Stack:** Markdown, GitHub Flavored Markdown (GFM), Mermaid.js diagrams.

## Global Constraints
- Must be written in English.
- Must accurately map all repositories in `/mnt/Shares/GIT/the-new-algo` to their respective GitHub remotes and functional roles.
- Must maintain identical, consistent content between `profile/README.md` and root `README.md`.
- File paths: `/mnt/Shares/GIT/the-new-algo/.github/profile/README.md` and `/mnt/Shares/GIT/the-new-algo/.github/README.md`.

---

### Task 1: Generate Organization Profile README (`profile/README.md`)

**Files:**
- Create: `/mnt/Shares/GIT/the-new-algo/.github/profile/README.md`

**Interfaces:**
- Consumes: Design spec at `docs/superpowers/specs/2026-09-15-tempusoneps-ecosystem-readme-design.md`
- Produces: GitHub Organization Profile page at `https://github.com/tempusoneps`

- [ ] **Step 1: Write `profile/README.md`**
Write complete documentation including:
- Header & Ecosystem overview
- Architecture flowchart in Mermaid
- Categorized component tables (Data, Feature Engineering & Profiling, Strategy & Signals, Simulation & Execution)
- End-to-end research to live execution lifecycle
- Developer and researcher setup guidelines

- [ ] **Step 2: Verify file existence and syntax formatting**
Check that `profile/README.md` is created and Mermaid blocks are syntactically valid.

- [ ] **Step 3: Commit `profile/README.md`**
```bash
git add profile/README.md
git commit -m "docs: add GitHub organization profile README"
```

---

### Task 2: Generate Root Repository README (`README.md`)

**Files:**
- Create: `/mnt/Shares/GIT/the-new-algo/.github/README.md`

**Interfaces:**
- Consumes: `profile/README.md`
- Produces: Root documentation for `tempusoneps/.github` repo

- [ ] **Step 1: Create root `README.md`**
Copy / mirror the validated content from `profile/README.md` to `README.md`.

- [ ] **Step 2: Verify content matching and links**
Ensure all relative and absolute links, badges, and Mermaid code blocks are identical and correctly formatted.

- [ ] **Step 3: Commit `README.md`**
```bash
git add README.md
git commit -m "docs: add root repository README"
```

---

### Task 3: Final Verification & Cleanliness

**Files:**
- Modify/Verify: `profile/README.md`, `README.md`

- [ ] **Step 1: Verify git status and file completeness**
Run `git status` and inspect line counts and markdown rendering.

- [ ] **Step 2: Verify all repository references against the local filesystem**
Confirm all 17 components are accounted for accurately.
