---
slug: github-good-resume-writing-overview
id: github-good-resume-writing-overview
title: 'Good Resume: A LaTeX Template for Technical Roles'
repo: justin-napolitano/good-resume
githubUrl: https://github.com/justin-napolitano/good-resume
generatedAt: '2025-11-24T17:28:57.816Z'
source: github-auto
summary: >-
  I built the "good-resume" repo to simplify the often daunting task of creating
  a resume for data science and technical roles. Using LaTeX, I wanted to
  provide a clean, customizable template that speaks to both aesthetic appeal
  and functionality. Let's dig into the project, its design choices, and where
  I'm headed next.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: writing
entryLayout: writing
showInProjects: false
showInNotes: false
showInWriting: true
showInLogs: false
---

I built the "good-resume" repo to simplify the often daunting task of creating a resume for data science and technical roles. Using LaTeX, I wanted to provide a clean, customizable template that speaks to both aesthetic appeal and functionality. Let's dig into the project, its design choices, and where I'm headed next.

## What is Good Resume?

At its core, good-resume is a LaTeX-based template that allows anyone to craft a professional resume quickly. The idea is to have a solid starting point, with modular content sections that you can easily customize. No more wrestling with formatting in Word or Google Docs! 

The repository includes everything you need to create polished PDF outputs right from your terminal. Want to tweak your experience or education? No problem. It’s all modular, making changes straightforward.

## Why I Built It

There's a huge demand for resumes in today's job market, especially in technical fields where clarity and precision are key. I've seen too many resumes that either look cluttered or, worse, fail to highlight relevant skills effectively. With good-resume, I aimed to bridge that gap.

- **Clean Design:** I wanted something professional that prioritizes readability.
- **Customization Flexibility:** Giving users the ability to modify sections based on their unique skills and experiences was crucial.
- **Efficiency:** The build pipeline reduces manual effort and keeps things organized.

## Key Design Decisions

I chose LaTeX mainly for its powerful typesetting capabilities. It offers precision that you don't get with typical word processors, especially for scientific or technical content. Here are my key design choices:

- **Modular Content:** Each section of the resume—like education, work experience, and skills—lives in its own file. This means you can edit or swap them out independently, which reduces headaches when updating.
- **Styling:** A dedicated `.sty` file handles all the custom styling. This keeps the main document clean and focuses on content rather than appearance.
- **Automation:** I wrote a Python script and used Make to automate dependency installation and the build process. The more I can automate, the better—pragmatism is my friend.

## Tech Stack

Here’s what powers good-resume:

- **LaTeX**: The primary language for formatting resumes, of course.
- **Python**: Used for the build automation script.
- **Make**: Facilitates smooth builds with commands that anyone can run.

Each component serves a specific purpose in streamlining the resume creation process.

## Getting Started

To get rolling with good-resume, you need a few prerequisites:

1. **Install a LaTeX distribution** (e.g., TeX Live, MiKTeX).
2. **Python 3.x** must be installed.
3. The `make` utility is essential for running builds.

### Quick Installation Steps

1. Clone the repo:
   ```bash
   git clone https://github.com/justin-napolitano/good-resume.git
   cd good-resume
   ```

2. If you need to install Python dependencies later:
   ```bash
   pip install -r requirements.txt
   ```

3. Compile your resume:
   ```bash
   make clean
   make
   ```
   
4. Your generated PDF will be in the directory as `resume.pdf`.

## Project Structure

Here’s how the repository is organized:

```
/_header.tex           # Common headers for all resumes
/deployz/             # Deployment scripts
/python-build.py      # The build automation script
/README.md            # Overview and instructions
/resume.pdf           # Compiled output
/resume.tex           # Main source file
/sections/            # Modular content sections
/TLCresume.sty        # Custom style file
```

The `resume.tex` file is your main document. It imports styles from `TLCresume.sty` and pulls content dynamically from the `/sections/` folder, making editing seamless.

## Tradeoffs

While I love the modular approach, there are tradeoffs to consider. For instance:

- **Learning Curve**: If you’re unfamiliar with LaTeX, there’s a slight learning curve. But trust me, once you get the hang of it, you’ll love the control it gives you.
- **Installation Overhead**: The necessity of having a LaTeX distribution and setting up Python means it’s not as hassle-free as a simple Word template. However, for many, the additional control is worth it.

## Future Work / Roadmap

I’m far from done with good-resume. Here are a few things I’d like to tackle next:

- **Improved Documentation**: I want to detail how to customize sections and styles effectively. Nothing worse than a great tool with poor instructions.
- **Support for More Output Formats**: HTML or Markdown options would be nice for those who want to share their resumes on personal websites.
- **CI/CD Pipeline**: Automating resume generation on commits would keep the process even smoother.
- **Deployment Scripts**: Enhancing scripts to easily host your resume online would be a significant step forward.
- **Sample Data**: I want to include example scenarios to help newcomers get started quickly without needing to guess how to populate their resumes.

## Let's Stay Connected

If you’re interested in updates about good-resume or my other projects, I share news on social media. Find me on Mastodon, Bluesky, and Twitter/X. I’d love to connect and hear your thoughts!

In summary, good-resume is my personal take on simplifying the resume creation process for tech-minded folks. I believe it combines cleanliness with flexibility, allowing users to present themselves in the best light possible. Try it out, and let’s make resume writing less painful, one LaTeX file at a time!
