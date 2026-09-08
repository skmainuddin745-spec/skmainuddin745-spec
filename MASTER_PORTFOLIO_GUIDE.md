# GitHub Portfolio — Master Analysis & Organization Guide

> Created: September 2026 | By: In-depth drive analysis (C:\, E:\, F:\, G:\)

---

## What This Folder Is

`F:\Spain Universities Professor\github\` is your **curated GitHub portfolio** — organized from a rigorous analysis of all code and projects found across your four drives. Each sub-folder is a **standalone GitHub repository** with professional README, clean source files, and appropriate .gitignore.

---

## Repository Map

| # | Folder | Domain | Impressiveness | Source Drives |
|---|--------|--------|---------------|---------------|
| 00 | `00_AI-Closed-Loop-Dyeing-Bangladesh` | Industrial AI / Closed-Loop Control | 🌟🌟🌟🌟🌟 | F:\ |
| 01 | `01_Mpro-Acylation-TS` | Computational Chemistry / Drug Discovery | 🌟🌟🌟🌟🌟 | C:\ |
| 02 | `02_DES-Drug-Delivery-GROMACS` | Molecular Dynamics / Drug Delivery | 🌟🌟🌟🌟🌟 | C:\ |
| 03 | `03_PEG-Polymer-MD-Analysis` | Polymer Physics / MD | 🌟🌟🌟🌟 | C:\ |
| 04 | `04_Smart-Dyeing-Process-Analytics` | Data Science / Process Optimisation | 🌟🌟🌟🌟 | F:\ |
| 05 | `05_Odysseus-AI-Assistant` | AI Engineering / LLM / Full-stack | 🌟🌟🌟🌟🌟 | E:\ |
| 06 | `06_Data-Science-Portfolio` | Data Engineering / Python Algorithms | 🌟🌟🌟 | G:\ |
| 07 | `07_CADD-Drug-Discovery` | CADD / Molecular Docking | 🌟🌟🌟🌟 | G:\ |
| 08 | `08_CytMyo-Mobile-Proton-MD-Pesticides` | MS + Gas-Phase MD / Herbicide Binding | 🌟🌟🌟🌟🌟 | C:\ |
| 09 | `09_Hybrid-Quantum-Classical-CNN-Oral-Disease` | Quantum ML / Medical Imaging | 🌟🌟🌟🌟🌟 | Kaggle |

---

## What Was Found (Drive-by-Drive Analysis)

### C:\ Drive — Computational Chemistry Research

**Most impressive projects found:**

1. **`C:\Users\SK\Mpro_TS_FINAL\`** ⭐ *FLAGSHIP*
   - Full QM/MM pipeline for SARS-CoV-2 Main Protease acylation transition state
   - 4 stages: His41 approach scan → gate check → C–N cleavage scan → TS verification → high-accuracy energetics
   - Python scripts: `monitor.py` (live dashboard), `check_pose.py` (gate logic), `analyze_ts.py` (TS identification)
   - Bash orchestration: `run_stage0.sh`, `run_stage1.sh` (chained GROMACS+CP2K QM/MM runs)
   - Technology: GROMACS 2022, CP2K 9.1, PBE/DZVP, CHARMM36m

2. **`C:\Users\SK\DES-ACE-IBU-WA\`** and **`C:\Users\SK\second_solved\`**
   - Atomistic MD of Deep Eutectic Solvent (Menthol + Thymol) with Ibuprofen + Acetaminophen + water
   - Complete CHARMM36 topology: MEN.itp, THY.itp, IBU.itp, ACE.itp, topol.top, posre files
   - Energy minimisation + full production MD

3. **`C:\Users\SK\1\` and `C:\Users\SK\1\1_peg\`**
   - PEG-400, PEG-600, PEG-2000 comparative MD study (water + gas phase + urea)
   - VMD Tcl analysis scripts (`Density.tcl`) for frame-wise density
   - Radius of gyration analysis at frames 2, 500, 700, 1000

4. **`C:\Users\SK\myo\`, `C:\Users\SK\second_run\`, `C:\Users\SK\Solved\`, `C:\Users\SK\third_solved\`**
   - Additional GROMACS MD systems (likely myoglobin and related protein simulations)
   - `myo\charmm36-jul2022.ff` — CHARMM36 force-field installation

5. **`C:\Users\SK\PU\`**
   - TiO2 nanoparticle simulations (PDB files: TiO2_new.pdb, TiO2_replicated.pdb)
   - UNK.itp, UNL.itp — custom force-field parameter files

### E:\ Drive — AI Engineering Project

6. **`E:\odysseus-main\`** ⭐ *FLAGSHIP*
   - Production-grade self-hosted AI research assistant (~75,000 lines of Python)
   - Full-stack: Flask/WebSocket backend, services for STT/TTS/search/email/calendar/RAG/YouTube/shell
   - Key files: `ai_interaction.py` (74K lines), `builtin_actions.py` (107K), `deep_research.py` (36K)
   - Technology: Ollama, ChromaDB, FastEmbed, Whisper, Piper TTS, CalDAV, Docker

### F:\ Drive — Research Analysis & Web Projects

7. **`F:\Downloads\01_Projects_and_Research\2026-08-05_Analysis_Session\`**
   - Rigorous statistical analysis of real industrial dyeing batch data (660 batches)
   - Python: `generate_charts.py` (8 publication figures), `_verify_all_stats.py` (math verification)
   - Complete verification pipeline with JSON audit log

8. **`F:\build_doc.js`** — Documentation builder utility (JavaScript)

9. **`F:\Spain Universities Professor\website\`** — Academic website (HTML)

### G:\ Drive — CADD Research & Data Science

10. **`G:\01_Projects_and_Research\`**
    - PEG-400 in water 200 ns Desmond MD (8 RDF shell scripts)
    - CADD docking reports (HTML): 6LU7, 6MOJ, 4EY7/BOAT04000 (CYP3A4)
    - Ligand Plus interaction maps

11. **`G:\__duplicate_scanner\`**
    - Intelligent duplicate file scanner (`deep_scan.py` — 35K, `scan_duplicates.py`, `safe_cleanup.py`)
    - Generated analysis: `deep_scan_report.json` (3.2 MB), interactive `dashboard.html`

12. **`G:\07_Uncategorized_Folders\professional skill\`**
    - Udemy: Data Science Course 2021 (TensorFlow, scikit-learn Jupyter notebooks)
    - Udemy: Financial Analyst Course (Excel, financial modelling)
    - Udemy: Data Science with R

---

## How to Upload to GitHub

### Option 1: One repository per project (Recommended)

```bash
# Example for Project 01
cd "F:\Spain Universities Professor\github\01_Mpro-Acylation-TS"
git init
git add .
git commit -m "Initial commit: SARS-CoV-2 Mpro acylation TS QM/MM pipeline"
git remote add origin https://github.com/YOUR_USERNAME/Mpro-Acylation-TS.git
git push -u origin main
```

### Option 2: Monorepo

```bash
cd "F:\Spain Universities Professor\github"
git init
git add .
git commit -m "Portfolio: 10 computational chemistry + AI engineering projects"
git remote add origin https://github.com/YOUR_USERNAME/research-portfolio.git
git push -u origin main
```

### Option 3: GitHub Profile README

Copy the contents of `profile/README.md` to a repository named exactly `YOUR_USERNAME` on GitHub — this becomes your visible GitHub profile page.

---

## Files Needed for Each Repository

Each project folder should have:
- [x] `README.md` ✅ (created)
- [ ] `.gitignore` — exclude large binary files (.xtc, .trr, .tpr, .edr etc.)
- [ ] `requirements.txt` or `environment.yml` — Python dependencies
- [ ] `LICENSE` — MIT or CC-BY-4.0

---

## Suggested .gitignore for MD Projects

```gitignore
# GROMACS large binary trajectories
*.xtc
*.trr
*.edr
*.tpr
*.cpt
*.wfn
*.bak-*

# Python cache
__pycache__/
*.pyc
*.pyo
.ipynb_checkpoints/

# Virtual environments
venv/
.venv/
env/
conda-env/

# OS files
.DS_Store
Thumbs.db
```

---

## Priority Order for Professors

1. **`01_Mpro-Acylation-TS`** — Cutting-edge COVID research, shows deep mechanistic understanding
2. **`05_Odysseus-AI-Assistant`** — Shows advanced software engineering, AI/LLM competence
3. **`02_DES-Drug-Delivery-GROMACS`** — Shows MD expertise in biomedical application
4. **`00_AI-Closed-Loop-Dyeing-Bangladesh`** — Shows end-to-end industrial AI from data to deployment
5. **`04_Smart-Dyeing-Process-Analytics`** — Shows rigorous statistical/data science skills
6. **`08_CytMyo-Mobile-Proton-MD-Pesticides`** — Shows cross-disciplinary MS + MD expertise
7. **`09_Hybrid-Quantum-Classical-CNN-Oral-Disease`** — Shows quantum ML frontier research
8. **`07_CADD-Drug-Discovery`** — Shows breadth of computational drug discovery tools
9. **`03_PEG-Polymer-MD-Analysis`** — Polymer/biomaterials MD expertise
10. **`06_Data-Science-Portfolio`** — Software engineering + data pipeline skills

---

*Analysis completed: September 8, 2026 | All four drives scanned: C:\, E:\, F:\, G:\*
