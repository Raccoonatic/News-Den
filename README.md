
<p align="center">
 <img src=".assets/README_img/newsden_banner.png" alt="CoverArt" width="800">
</p>

<p align="center"><i>This project has been created as the central repository for the NewsDen infrastructure</i></p>

<h1 align="center">📰🌍 News Den - The Backend 🌍📰</h1>
<p align="center"><b><em>Designed to empower independent journalism.</em></b></p>

---

## 📰 Description
The end product is the entire infrastructure for an Online Newspaper. The system features a modular architecture designed with a default directive: posting the incoming article. There is a panel where every step of the article's lifetime can be toggled; if all steps are shut off, all incoming work must be published directly. The infrastructure supports three types of visitors: "None" (readers who only view news), "Editors" (staff making publishing decisions), and "Reporters" (contributors authorized to submit news, video, and research).

## ⚙️ Instructions

### 🛠️ Compilation
TBD

##  Users

The infrastructure heavily relies on a modular priority and badge system that controls access and permissions without needing to modify the source code. Below is a breakdown of the specific roles and pipeline stages:

 #### 🖥️ Editor Badges

 - **`Admin`** : The Mapache badge for developers; manages badges, priority scales, and editorial meets
 - **`Agent`** : Edits article priority, allocates resources, and sends items to development
 - **`Writer`** : Edits articles, accesses archives, and synthesizes reporting into final written pieces
 - **`Director`** : Accesses the composing bay, selects the final view of articles, and publishes them
 - **`Coordinator`** : Support role for the Director with all permissions except final publication
 - **`Mod`** : Schedules meets and manages registrants and badges
 - **`Designer`** : Accesses the weekly finalized article queue to build newsletters

 #### 📸 Reporter Badges

 - **`Viewer`** : A valid user without an ID check; can view news and submit feedback
 - **`Field`** : Completed ID check; can submit news requests and receive credits
 - **`Specialists`** : Roles like Photographer, Videographer, Redacter, Interviewer, and Inspector, who can be allocated as specific resources for an article

 ## 🗺️ Workflow Stages

 - **`[1] Content Ingestion`** : Submissions pass through an automated AI quality check
 - **`[2] Editorial Evaluation`** : Editors review for thematic alignment and assign priority scores
 - **`[3] Newsroom Review`** : Asset audit to resolve missing media via archives or field reporters
 - **`[4] Drafting`** : Final copywriting and resource verification
 - **`[5] Director Review`** : Executive quality control and web publication
 - **`[6] Newsletter Layout`** : Curation of published stories into a weekly layout
 - **`[7] Revision Loop`** : Rework protocols if benchmarks are unmet at any stage
<br></br>
---

### API Endpoints
TBD

<br></br>
---

## 🧠 Technical Overview

- Public Website: **Next.js or Hugo (Cloudflare/GitHub Pages)**
- Newsroom Application: **Strapi or Ghost**
- Back End API: **Python (FastAPI) or Node.js (Express)**
- Database: **PostgreSQL (or MariaDB)**
- AI Processing Layer: **Whisper, Llama 3, Groq, or Gemini**
- AI Orchestration: **LangChain, LlamaIndex, CrewAI, or custom (Odysseus)**
- File Archive: **100 TB Google Drive via Service Account**
- Submission System: **Tally.so or SecureDrop/React form**
- Editorial Workflow State Machine: **Managed via PostgreSQL Enums and timestamps**

---

## 📚 Resources
TBD

## 🤖 AI Usage
TBD

---

## 🚨 Other Makefile Utilities
TBD

---

## ⚖️ License

**Copyright (c) 2026 Luis "Mapache" Torcate & HUELLATINA coop. All Rights Reserved.**

This repository and its contents are proprietary and confidential. No part of this software may be copied, modified, distributed, or used without explicit written permission from the copyright holders.

---

## 🧾 Final Notes 🦝

If you made it this far…

Merry Christmas.
Take a break. Drink water. Maybe eat an arepa.

The future of journalism, is [here](https://github.com/Raccoonatic/News-Den).

📰✨💜
