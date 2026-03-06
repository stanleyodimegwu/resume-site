# Hosting a Resume Using Markdown, Git, and GitHub Pages

## Statement of Purpose

This document explains how to format and host a professional resume using modern technical documentation tools. The goal is to demonstrate the practical application of principles described in Andrew Etter’s book *Modern Technical Writing*. Etter emphasizes that modern documentation should prioritize simplicity, version control, and web-based publishing so that documentation is easy to maintain and update.

This README teaches the reader how to publish a resume as a static website using Markdown, Git, and GitHub Pages. It is written for readers with limited experience using distributed version control systems or static site generators, but who have basic familiarity with command-line tools and file management. By following these instructions, readers will learn how to produce a simple documentation workflow that reflects the practices recommended in *Modern Technical Writing*.

---

## Prerequisites

Before starting, the following tools and resources are required:

- A GitHub account
- Git installed on your computer
- Basic familiarity with Markdown
- A resume written in Markdown format

Andrew Etter argues that documentation should rely on tools that reduce complexity and make documentation easy to maintain. The tools used in this guide follow this principle:

- **Markdown** is a lightweight markup language that keeps documentation easy to read and edit.
- **Git** is a distributed version control system that tracks documentation changes.
- **GitHub** is a forge where repositories can be stored, shared, and hosted online.
- **Jekyll** is the static site generator used by GitHub Pages to convert Markdown files into web pages.

Together, these tools allow documentation to be managed similarly to software code.

---

## Instructions

### Step 1: Create a GitHub Repository

The first step is to create a repository on GitHub. A repository stores project files and tracks their changes through Git.

According to Etter, documentation should be treated as a version-controlled resource rather than a static document. Storing documentation in a Git repository allows updates to be tracked and managed efficiently.

To create the repository:

1. Log into GitHub.
2. Click **New Repository**.
3. Name the repository `resume-site`.
4. Create the repository.

Once created, the repository can be cloned locally.

---

### Step 2: Write the Resume Using Markdown

Etter recommends lightweight markup languages such as Markdown because they simplify documentation workflows and reduce formatting complexity.

Markdown allows writers to format text clearly without complicated HTML syntax. 

This formatting remains readable while also allowing the content to be converted into HTML automatically.

The resume should be stored in a file named `resume.md`.

---

### Step 3: Track Documentation Using Git

One of Etter’s key recommendations is that documentation should be version controlled.

Using Git allows documentation changes to be tracked and managed through a clear history.

To upload files to GitHub, run the following commands:
git add .
git commit -m "Added resume documentation"
git push

These commands stage the changes, record them in the repository history, and upload them to GitHub.

---

### Step 4: Generate the Static Website

Etter also emphasizes publishing documentation on the web rather than distributing static files like PDFs, which makes documentation easier to update and maintain.

Static site generators make this possible.

GitHub Pages uses **Jekyll** to automatically convert Markdown files into HTML pages.

To configure the site, create a `_config.yml` file:
title: Stanley Odimegwu Resume
theme: minima

An `index.md` file is also created to serve as the homepage of the website.

When GitHub Pages builds the repository, Jekyll converts the Markdown files into a functional website.

---

### Step 5: Enable GitHub Pages Hosting

The final step is to enable GitHub Pages.

1. Open the repository settings.
2. Click **Pages**.
3. Select **Deploy from a branch**.
4. Choose the `main` branch and the root directory.

Once deployed, the resume becomes accessible at:
https://username.github.io/resume-site/

Publishing documentation online reflects Etter’s recommendation that documentation should be accessible and easy to update.

---

## Further Resources

Markdown Guide  
https://www.markdownguide.org

Git Documentation  
https://git-scm.com/docs

Jekyll Documentation  
https://jekyllrb.com/docs

GitHub Pages Documentation  
https://docs.github.com/en/pages

---

## FAQ

### Why is Markdown better than HTML?

Markdown is simpler and easier to read than HTML. It allows writers to focus on the content instead of complex formatting syntax.

### Why are my website changes not appearing immediately?

GitHub Pages may take a few minutes to rebuild the site after changes are pushed to the repository.

### Why use a static site generator instead of building a website manually?

Static site generators automatically convert Markdown files into HTML pages. This allows writers to focus on writing documentation rather than designing webpages, which aligns with Etter’s principle of simplifying documentation workflows.

---

## Credits

Resume and documentation created by:

Stanley Odimegwu  
University of Manitoba

Theme used: Minima Jekyll Theme

Concepts based on Andrew Etter’s book *Modern Technical Writing*.
