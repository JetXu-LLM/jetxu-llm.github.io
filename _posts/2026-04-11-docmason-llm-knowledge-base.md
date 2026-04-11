---
title: "The Hidden ChatGPT Plus Feature for Messy Office Files on Mac"
date: 2026-04-11 00:15:00 +0800
categories: [AI, Knowledge Work]
tags: [docmason, chatgpt-plus, codex, notebooklm-alternative, macos, office-files, knowledge-base]
description: "Most ChatGPT Plus users never touch Codex. DocMason turns that unused capacity into a local, evidence-first knowledge base for decks, spreadsheets, PDFs, and emails on Mac."
image:
  path: https://img.youtube.com/vi/Sq3a5qxsLwM/maxresdefault.jpg
  alt: "DocMason hero video thumbnail"
---

Most ChatGPT Plus users never open Codex.

That makes sense. Codex looks like a tool for programmers, and most white-collar work does not happen in a code editor. It happens in decks, spreadsheets, PDFs, and long email threads. So the extra capacity sitting behind Codex often stays idle.

That is the opening behind DocMason.

Andrej Karpathy recently described the missing layer in AI as the need for a real knowledge base before agents can do serious work. On a Mac, that gap usually looks less like a research paper and more like a shared drive full of half-finished board decks, finance models, legal PDFs, and buried notes.

DocMason is built for that exact mess.

## What The First Video Actually Shows

The first video is not a generic "chat with your docs" demo.

It stages a realistic office scenario around Project NOVA inside a listed hospitality group. The official board deck presents a polished success story. The underlying evidence does not.

- The board deck frames Project NOVA as a clean GBP 380M story.
- The PowerPoint speaker notes soften a compliance problem.
- A hidden sheet in the CFO model drops the valuation to GBP 94M.
- The legal memo flags a material omission.
- The final sign-off emails show leadership already knew.

That is the whole point. The job is not to summarize four files. The job is to pull signal out of contradictory office material and turn it into something a serious user can act on.

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1.5rem 0;">
  <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://www.youtube.com/embed/Sq3a5qxsLwM?si=ifGy-Iqo10VWKHfu" title="The Hidden ChatGPT Plus Feature You're Paying For (But Not Using)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

DocMason does not flatten that case into anonymous text chunks. It keeps the structure that matters, cross-references the evidence, and produces a consulting-grade memo with exact citations back to the underlying files.

That is also where the NotebookLM comparison becomes real. NotebookLM is useful for quick cloud-native research. But when the hard part of the work is hiding in speaker notes, hidden sheets, layout-heavy decks, and local file boundaries, you need a different operating model.

## Why This Matters To White-Collar Users

If you work in strategy, finance, operations, legal, product, or consulting, your bottleneck is rarely writing the final paragraph. It is finding the buried contradiction fast enough to trust the answer.

DocMason is built around three practical ideas:

- Keep the workspace local.
- Preserve Office-native structure instead of flattening everything into plain text.
- Return evidence-backed output you can inspect instead of a polished guess.

That is why the product is better described as a local, evidence-first knowledge base for serious file-heavy work, not as another document chatbot.

## The Second Video Answers The Next Question

After the first video, most people ask a simpler question: can I actually run this without turning my evening into a developer project?

That is exactly what the second video is for.

It is a first-start walkthrough for Mac users. The flow is deliberately simple:

1. Download the clean bundle from GitHub.
2. Unzip it on your Mac.
3. Drop a few real files into `original_doc/`.
4. Install Codex for macOS and open the DocMason folder as the workspace.
5. Tell Codex: `Please prepare the DocMason environment.`
6. If it asks for Full access, switch it and continue.
7. Tell Codex: `Please build the knowledge base.`
8. Wait until the knowledge base is built and published.
9. Start asking questions.

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1.5rem 0;">
  <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://www.youtube.com/embed/jWRtr70Rvug?si=Xu0esBGQoLLdWwCy" title="DocMason Setup Guide: Turn your Office Files into AI Second Brain Knowledge Base" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

The important detail is that the tutorial does not fake the hard part. The middle stretch is real agent work. Only the waiting is sped up. That matters, because trust starts before the first answer. Users need to see that the environment is being prepared, the knowledge base is being built, and the workspace is ending in a reusable state.

## Stop Leaving Codex Idle

OpenAI lists expanded Codex usage on the Plus plan, and Codex follows its own plan-based limits rather than the usual caps people run into in ChatGPT. In practice, that means many Plus subscribers are sitting on capacity they rarely use simply because they do not write code all day.

DocMason turns that neglected surface into something much more useful for office work: a local knowledge base over the files you already have, with answers you can trace back to the source.

<div style="text-align: center; margin: 2rem 0;">
  <a href="https://github.com/JetXu-LLM/DocMason/releases/latest/download/DocMason-clean.zip" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #0DAFC6; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">Download DocMason</a>
  <a href="/docmason-first-start/" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #1f2937; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">First-Start Guide</a>
  <a href="https://github.com/JetXu-LLM/DocMason" style="display: inline-block; padding: 10px 18px; margin: 0 8px 12px 0; background-color: #4b5563; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">View on GitHub</a>
</div>

If NotebookLM already handles your workload, keep using it. But if your real work lives in messy decks, spreadsheets, PDFs, and email threads on a Mac, and you want an answer that points back to exact files instead of asking you to trust the summary, this is the better fit.

If you try it, I would be curious about one thing: which office file type breaks your current AI workflow first?
