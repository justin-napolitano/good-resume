---
slug: github-good-resume-note-technical-overview
id: github-good-resume-note-technical-overview
title: Good Resume
repo: justin-napolitano/good-resume
githubUrl: https://github.com/justin-napolitano/good-resume
generatedAt: '2025-11-24T18:37:38.667Z'
source: github-auto
summary: >-
  This repo offers a LaTeX resume template tailored for data science and tech
  roles. It features a modular setup, making it easy to customize different
  sections. I’ve included a build pipeline using Python and Make for hassle-free
  PDF generation.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repo offers a LaTeX resume template tailored for data science and tech roles. It features a modular setup, making it easy to customize different sections. I’ve included a build pipeline using Python and Make for hassle-free PDF generation.

## Key Features

- Clean, professional LaTeX template
- Modular content in separate section files
- Custom styles via `TLCresume.sty`
- Automated build with Python script and Makefile

## Getting Started

### Prerequisites

- LaTeX distribution (TeX Live, MiKTeX)
- Python 3.x
- `make` utility

### Quick Run

1. Clone the repo:

   ```bash
   git clone https://github.com/justin-napolitano/good-resume.git
   cd good-resume
   ```

2. (Optional) Install Python dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Build the PDF:

   ```bash
   make clean
   make
   ```

Check `resume.pdf` for the output. Easy customization and automated builds make this a solid choice!
