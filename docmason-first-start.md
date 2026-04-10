---
layout: page
title: "DocMason First Start"
permalink: /docmason-first-start/
description: "A first-run guide for DocMason on macOS. Download the clean bundle, drop in a few real files, prepare the environment, build the knowledge base, and start asking questions."
---

If you already have ChatGPT access, getting started with DocMason is much simpler than it looks.

This page is for the second question people ask after the demo: how do I actually get it running on my Mac?

<div style="margin: 1.25rem 0 1.5rem 0;">
  <a href="https://github.com/JetXu-LLM/DocMason/releases/latest/download/DocMason-clean.zip" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #0DAFC6; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">Download DocMason</a>
  <a href="https://youtu.be/jWRtr70Rvug?si=50-2yxbXzeidcaWy" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #1f2937; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">Watch Tutorial</a>
  <a href="https://openai.com/codex" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #4b5563; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">Get Codex for macOS</a>
</div>

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1.5rem 0;">
  <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://www.youtube.com/embed/jWRtr70Rvug?si=Xu0esBGQoLLdWwCy" title="DocMason Setup Guide: Turn your Office Files into AI Second Brain Knowledge Base" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

## What You Need

You only need four things for the first run:

1. A Mac.
2. A ChatGPT account you can use with Codex.
3. The DocMason clean bundle.
4. A few real files you want to analyze.

Start with a small batch of files instead of throwing in everything at once. DocMason supports incremental updates later, so the fastest way to trust the workflow is to get one clean first run.

## The First Run

### 1. Download and unzip the clean bundle

Download the latest clean bundle from GitHub and unzip it anywhere local on your Mac.

The folder you care about first is `original_doc/`. That is where your working files go.

### 2. Drop a few real files into `original_doc/`

For the first pass, drag in a small set of real work files:

- PowerPoint decks
- spreadsheets
- PDFs
- email files

The goal is not to build your entire knowledge base on minute one. The goal is to get to a real published workspace quickly.

### 3. Install Codex and open the DocMason folder

Install Codex for macOS, sign in with your ChatGPT account, and open the DocMason folder as the project workspace.

DocMason's operating model is simple:

- the repo is the app
- the agent is the runtime

You are not uploading your files to a separate web tool. You are opening a local workspace and letting the agent work inside it.

### 4. Ask Codex to prepare the environment

Send this message:

```text
Please prepare the DocMason environment.
```

On the first run, DocMason checks the workspace, builds the local runtime, and verifies what it needs.

If Codex asks for Full access, switch it here and click Continue. That is a normal part of the bootstrap path.

### 5. Build the knowledge base

When the environment is ready, send this:

```text
Please build the knowledge base.
```

DocMason will stage, compile, validate, and publish your files into a traceable local knowledge base.

The long middle stretch is real agent work. Only the waiting should feel slow.

### 6. Start asking questions

When you see that the knowledge base is built and published, the workspace is ready.

At that point, stop thinking about setup and start asking business questions.

Better first questions look like this:

- What risks appear across these documents, and which sources support them?
- Where do the deck and the spreadsheet disagree?
- Which file contains the strongest evidence against the official story?

## What To Expect On Your First Run

These things are normal:

- environment preparation takes a bit longer than you want
- Codex may ask for Full access
- the first knowledge-base build is slower than later incremental updates

Do not optimize for speed on the first run. Optimize for finishing one clean pass.

Once you have seen `built and published`, you have the part that matters.

## Where To Go Next

- [Read the launch post](/posts/docmason-llm-knowledge-base/)
- [Open the DocMason repository](https://github.com/JetXu-LLM/DocMason)
- [Download the clean bundle](https://github.com/JetXu-LLM/DocMason/releases/latest/download/DocMason-clean.zip)