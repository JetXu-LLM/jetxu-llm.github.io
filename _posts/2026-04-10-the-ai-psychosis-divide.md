---
title: 'The "AI Psychosis" Divide: Why Coders are Terrified and Everyone Else is Bored'
date: 2026-04-10 21:40:00 +0800
categories: [AI, Knowledge Work]
tags: [andrej-karpathy, ai-capability-gap, llm-knowledge-bases, docmason, codex, office-files, knowledge-work]
description: "Andrej Karpathy is right: the biggest AI capability gap is not between people who write better prompts. It is between workflows with durable context and workflows that still force models to start from zero."
image:
  path: /assets/img/posts/2026-04-10-ai-psychosis-divide/cover.png
  alt: "A split illustration showing messy office files on one side and a structured knowledge system on the other"
pin: true
---

> *Andrej Karpathy is right: the most important AI gap in 2026 is not between people who "get AI" and people who do not. It is between workflows that give frontier agents a working memory, and workflows that still make them start from scratch.*

Two intelligent people can use "AI" every day and walk away with opposite conclusions.

One sees ChatGPT miss obvious questions, stumble on simple voice tasks, and produce polished nonsense on demand. From that angle, the hype looks inflated. 

Another watches Codex or Claude Code spend an hour inside a repository, trace dependencies across dozens of files, run tests, fix failures, and come back with a coherent patch. From that angle, the complacency looks absurd.

Both impressions are real.

That is why Andrej Karpathy's phrase "AI Psychosis" landed so hard this month. It named a social fact that many technical people had been feeling but had not explained cleanly: the people who are closest to frontier agentic workflows are not living in the same AI reality as everyone else.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-gap.png" alt="Karpathy tweet on AI capability gap" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

The lazy version of this story is that programmers simply know how to prompt better.

I do not think that is the right explanation.

The real gap is structural. Coders are giving AI a full working surface. Most white-collar workers are not.

## The strange part is that both sides feel justified

In his thread, Karpathy made two crucial claims that fit together perfectly.

The first is about recency and tier of use. A large number of people still anchor their view of AI to older, weaker, or free-tier experiences. If that is the product one has actually used, skepticism is entirely rational. The model fumbles basic queries, and people laugh it off as a glorified autocomplete.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-psychosis.png" alt="Karpathy tweet defining AI Psychosis" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

But the second claim is the one that matters. The biggest recent gains in AI have been unusually concentrated in technical domains. Why? Because domains like coding, math, and research offer explicit feedback loops. Code compiles or it does not. Tests pass or they fail. A patch breaks the build or survives contact with reality.

Frontier models have improved fastest where the environment supplies both rich context and hard checks.

This is why technical users sound overheated when they talk about AI. They are not reacting to marketing videos. They are reacting to repeated, daily exposure to systems that can already perform real work inside bounded, inspectable environments.

The non-technical crowd is reacting to a different product surface. In their experience, AI still feels like a clever assistant that forgets too much, guesses too often, and rarely earns full trust.

That disagreement will keep sounding irrational until more people notice that the two groups are not arguing from the same workflow.

## Code provides an engine. Office work provides a swamp.

When a programmer hands a frontier agent a codebase, the agent gets more than text.

It gets a working environment. The repository contains assembled intent: source files, tests, config, docs, examples, commit history, naming conventions, scripts, and maintainer policy. The agent can inspect, modify, run, verify, and revise. Every action leaves evidence.

In other words, code has become unusually legible to AI because software teams already store their work in a structured, machine-readable form.

Most office work does not look like that.

A strategist, operator, analyst, consultant, lawyer, or finance lead may spend the week inside decks, spreadsheets, PDFs, meeting notes, exports, appendices, and email threads. The relevant context exists, but it is scattered across file formats and folder boundaries. Much of the most important information lives in speaker notes, hidden tabs, comments, side calculations, naming quirks, and the relationship between one document and another.

None of that survives the standard copy-paste workflow into a chat window.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/context-gap.svg" alt="Diagram comparing codebase context to fragmented office files" style="max-width: 100%;">
</div>

This is the failure point many product discussions miss.

Office work *has* a codebase too. It is the folder tree full of messy business files. The problem is that this codebase is rarely compiled into anything durable, searchable, or self-maintaining. Each new chat session starts close to zero.

That makes ordinary knowledge work look weaker than it should. The model is being asked to synthesize from fragments, then forget the result when the conversation ends. It is not building an engine; it is wading through a swamp.

## Stop chatting. Start compiling.

This is why Karpathy's most important post this month may not have been the one about "AI Psychosis" at all. It may have been a quieter post a week earlier on the concept of "LLM knowledge bases."

The key shift is profound: stop treating documents as static inputs to retrieve from at query time, and start treating them as raw material for a persistent, interlinked knowledge artifact.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-llm-kb.png" alt="Karpathy tweet on LLM Knowledge Bases" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

His phrasing in the idea gist is unusually clear: *"The knowledge is compiled once and then kept current, not re-derived on every query."*

That one sentence reframes the problem from better retrieval (RAG) to better accumulation. Instead of uploading files and hoping the model rediscovers the right fragments on demand, the model incrementally reads, summarizes, cross-references, updates, flags contradictions, and maintains a wiki that grows richer with every source and every question.

In this architecture, raw sources remain the immutable ground truth. The human curates sources and asks good questions. The model does the bookkeeping.

That last part is the breakthrough. Humans do not abandon personal knowledge bases because knowledge is worthless. They abandon them because maintenance is tedious. Cross-links drift. Summaries go stale. Contradictions pile up. New evidence arrives faster than anyone wants to index by hand. LLMs are built to swallow that exact maintenance burden.

The center of gravity is moving from *"can AI read my docs?"* to *"how should an AI-maintained memory system stay reliable over time?"*

## The gap is no longer intelligence. It is operational context.

The next meaningful AI product for white-collar work is unlikely to be another prettier chat window.

It will look more like a local compiler for messy knowledge.

It will ingest the ugly reality of real work: board decks with speaker notes, spreadsheets with hidden sheets, PDFs with layout-dependent meaning, meeting transcripts, and folders with no naming discipline. It will preserve structure instead of flattening everything into anonymous text chunks. It will maintain memory instead of pretending every query is the first one. And it will show its work, because persistent systems need provenance, contradiction handling, and health checks if they are going to earn professional trust.

That is also why local-first matters heavily for this workflow. Serious knowledge work often happens in private files that should not bounce around cloud APIs by default. The workflow has to be comfortable with that constraint natively.

This, I think, is the office worker's version of AI psychosis. 

It will not begin when someone gets a slightly better answer in a chat tab. It will begin when a non-technical user drops forty ugly files into a workspace, lets an agent build maintained context around them, and then watches the system surface the hidden contradiction that their entire finance team has been missing for a week.

## Getting to the "Aha" Moment

Karpathy wrote that there is room here for "an incredible new product."

I think he is exactly right. The missing bridge is not from GPT-4 to GPT-5. It is from isolated chat to maintained context. 

That is the reason the category around local, evidence-first knowledge bases matters so much right now. It is also the reason I have been building around this exact workflow for office-heavy files—treating AI as an engine for structuring private context, instead of a generic writing tool.

If this argument resonates, I recently wrote a practical follow-up on what this looks like with real Mac workflows, Codex, and messy office documents. The example stages a realistic corporate scenario: a board-deck narrative that starts to fall apart once the system reads the underlying spreadsheet model, memos, and approvals together and compiles the real truth.

<div style="text-align: center; margin: 3rem 0; padding: 2rem; background: #fafafa; border-radius: 8px; border: 1px solid #eaeaea;">
  <h3 style="margin-top: 0;">Ready to try the compilation workflow?</h3>
  <p style="color: #666; margin-bottom: 1.5rem;">See how DocMason turns idle ChatGPT Plus capacity into a local knowledge compiler for your office files.</p>
  <a href="/posts/docmason-llm-knowledge-base/" style="display: inline-block; padding: 12px 24px; background-color: #111827; color: white; text-decoration: none; border-radius: 6px; font-weight: 600; font-size: 1.1rem; transition: background-color 0.2s;">Read the DocMason Walkthrough</a>
</div>

The argument over whether AI is a miracle or a disappointment will keep going in circles for a while.

That is fine. The two sides are often describing different systems, different workflows, and different memory conditions. But one conclusion is already visible: frontier agents look dramatically stronger in environments that give them structure, durable context, and feedback loops. 

Coding got there first because the repository was ready. The bigger opportunity now is to bring the same conditions to the rest of knowledge work.

## References

- Andrej Karpathy, April 2026 posts on X about the AI capability gap and "AI Psychosis": https://x.com/karpathy
- Andrej Karpathy, "LLM Wiki" idea file, April 5, 2026: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
