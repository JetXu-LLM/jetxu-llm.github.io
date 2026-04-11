---
title: 'The "AI Psychosis" Divide: Why Coders are Terrified and Everyone Else is Bored'
date: 2026-04-10 21:40:00 +0800
categories: [AI, Knowledge Work]
tags: [andrej-karpathy, ai-capability-gap, llm-knowledge-bases, docmason, codex, office-files, knowledge-work]
description: "Andrej Karpathy is right: the biggest AI capability gap is not between people who write better prompts. It is between workflows with durable context and workflows that still force models to start from zero."
image:
  path: /assets/img/posts/2026-04-10-ai-psychosis-divide/cover.svg
  alt: "A split illustration showing messy office files on one side and a structured knowledge system on the other"
pin: true
---

> *Andrej Karpathy is right: the most important AI gap in 2026 is not between people who "get AI" and people who do not. It is between workflows that give frontier agents a working memory and workflows that still make them start from scratch.*

Two intelligent people can use "AI" every day and walk away with opposite conclusions.

One sees ChatGPT miss obvious questions, stumble on simple voice tasks, and produce polished nonsense on demand. From that angle, the hype looks inflated.

Another watches Codex or Claude Code spend an hour inside a repository, trace dependencies across dozens of files, run tests, fix failures, and come back with a coherent patch. From that angle, the complacency looks absurd.

Both impressions are real.

That is why Andrej Karpathy's phrase "AI Psychosis" landed so hard. It named a social fact that many technical people had been feeling but had not explained cleanly: the people who are closest to frontier agentic workflows are not living in the same AI reality as everyone else.

![A quote card summarizing Karpathy's AI capability gap argument](/assets/img/posts/2026-04-10-ai-psychosis-divide/karpathy-gap-card.svg)
_Karpathy's April 10 observation matters because it explains the disagreement without pretending one side is hallucinating._

The lazy version of this story is that programmers simply know how to prompt better.

I do not think that is the right explanation.

The real gap is structural. Coders are giving AI a full working surface. Most white-collar workers are not.

## The strange part is that both sides are telling the truth

Karpathy's April 10 thread made two claims that fit together.

The first is about recency and tier of use. A large number of people still anchor their view of AI to older, weaker, or free-tier experiences. If that is the product one has actually used, skepticism is rational.

The second is more important. The biggest recent gains have been unusually concentrated in technical domains such as coding, math, and research. Those domains offer explicit feedback loops. Code compiles or it does not. Tests pass or they fail. A patch breaks the build or survives contact with the rest of the system.

That combination matters. Frontier models have improved fastest where the environment supplies both rich context and hard checks.

This is why technical users sound overheated when they talk about AI. They are not reacting to a marketing video. They are reacting to repeated exposure to systems that can already perform real work inside bounded, inspectable environments.

The non-technical crowd is reacting to a different product surface. In their experience, AI still feels like a clever assistant that forgets too much, guesses too often, and rarely earns full trust.

That disagreement will keep sounding irrational until more people notice that the two groups are not arguing from the same workflow.

## Code gives AI a complete working surface. Office work usually does not

When a programmer hands a frontier agent a repository, the agent gets more than text.

It gets a working environment.

The repository already contains accumulated intent: source files, tests, config, docs, examples, commit history, naming conventions, scripts, and usually some form of maintainer policy. The agent can inspect, modify, run, verify, and revise. Every action leaves evidence.

In other words, code has become unusually legible to AI because software teams already store their work in a structured, machine-readable form.

Most office work does not look like that.

A strategist, operator, analyst, consultant, lawyer, or finance lead may spend the week inside decks, spreadsheets, PDFs, meeting notes, exports, appendices, and email threads. The relevant context exists, but it is scattered across file formats and folder boundaries. Much of the most important information lives in speaker notes, hidden tabs, comments, side calculations, naming quirks, and the relationship between one document and another.

None of that survives the standard copy-paste workflow into a chat box.

![A diagram comparing codebase context with fragmented office-file context](/assets/img/posts/2026-04-10-ai-psychosis-divide/context-gap.svg)
_Programmers usually hand the model a living system. White-collar users often hand it a temporary excerpt._

This is the part many product discussions miss.

Office work has a codebase too. It is the folder tree full of messy business files. The problem is that this codebase is rarely compiled into anything durable, searchable, or self-maintaining. Each new chat session starts close to zero.

That makes ordinary knowledge work look weaker than it should. The model is being asked to synthesize from fragments, then forget the result when the conversation ends.

## Most white-collar AI use is still trapped in copy-paste mode

This is why so many otherwise smart people come away from everyday AI unimpressed.

The failure is not mainly about intelligence. It is about missing infrastructure.

Today, most non-technical AI use still follows the same pattern: upload a few files, ask a question, get a one-off answer, move on. The answer may be decent, but nothing compounds. The system does not maintain a stable map of the territory. It rediscovers knowledge from scratch every time.

That is tolerable for lightweight queries. It falls apart as soon as the real task spans multiple documents, conflicting claims, private files, or evolving context.

Take a normal corporate workflow. The public story sits in the board deck. The real tension sits in the spreadsheet model, the legal memo, the speaker notes, and the last three email approvals. A generic chat upload can summarize each file. It usually cannot maintain a disciplined memory of how those files reinforce or contradict one another over time.

This is why the best coding demos feel like a different species of product. They are not only using a stronger model. They are operating against a better memory substrate.

## Karpathy's bigger idea is about compilation, not chat

Karpathy's most important post this month may not have been the one about "AI Psychosis." It may have been the earlier post on LLM knowledge bases, and the April 5 gist that turned the tweet into an idea file.

The key shift is simple: stop treating documents as static inputs to retrieve from at query time, and start treating them as raw material for a persistent, interlinked knowledge artifact.

His phrasing in the gist is unusually clear: "The knowledge is compiled once and then kept current, not re-derived on every query."

That one sentence is doing a lot of work.

It reframes the problem from better retrieval to better accumulation. Instead of uploading files and hoping the model rediscovers the right fragments on demand, the model incrementally reads, summarizes, cross-references, updates, flags contradictions, and maintains a wiki that grows richer with every source and every question.

![A quote card on knowledge compilation from Karpathy's LLM Wiki gist](/assets/img/posts/2026-04-10-ai-psychosis-divide/karpathy-knowledge-base-card.svg)
_The important shift is from one-shot retrieval to maintained synthesis._

In Karpathy's formulation, raw sources remain the source of truth. The wiki becomes the maintained knowledge layer. A schema file tells the agent how to behave. The human curates sources and asks good questions. The model does the bookkeeping.

That last part is the breakthrough.

Humans do not abandon knowledge bases because knowledge is worthless. They abandon them because maintenance is tedious. Cross-links drift. Summaries go stale. Contradictions pile up. New evidence arrives faster than anyone wants to re-index by hand. LLMs are unusually well suited to that maintenance burden.

Even the fast response to Karpathy's gist made the same point from different angles. People immediately asked about provenance, contradiction handling, stale memory, ambient integration into agent workflows, and when to promote discoveries back into the knowledge layer. That is what infrastructure conversations sound like. The center of gravity moved from "can AI read my docs?" to "how should an AI-maintained memory system stay reliable over time?"

## The next breakout AI product will look less like chat and more like a knowledge compiler

Once that frame clicks, a lot of product positioning starts to look shallow.

The next meaningful AI product for white-collar work is unlikely to be another prettier chat window.

It will look more like a local compiler for messy knowledge.

It will ingest the ugly reality of real work: board decks with speaker notes, spreadsheets with hidden sheets, PDFs with layout-dependent meaning, meeting transcripts, drafts, side analyses, exports, and folders with no naming discipline. It will preserve structure instead of flattening everything into anonymous chunks. It will maintain memory instead of pretending every query is the first one. And it will show its work, because persistent systems need provenance, contradiction handling, and health checks if they are going to earn trust.

That is also why local-first matters more than the usual privacy slogan suggests. Serious knowledge work often happens in private files that should not leave the machine by default. The workflow has to be comfortable with that constraint. For many teams and individuals, it is not a preference. It is the table-stakes requirement that decides whether the product is usable at all.

This, I think, is the office worker's version of AI psychosis.

It will not begin when someone gets a slightly better answer in a chat tab.

It will begin when a non-technical user drops forty ugly files into a workspace, lets an agent build maintained context around them, and then watches the system surface the hidden contradiction that the team has been missing for a week.

## The gap is no longer model intelligence. It is operational context

Karpathy wrote that there is room here for "an incredible new product." I think he is right.

The missing bridge is not from GPT-4 to GPT-5. It is from isolated chat to maintained context.

That is the reason I think the category around local, evidence-first knowledge bases matters so much right now. It is also the reason I have been building around this exact workflow for office-heavy files instead of treating AI as a generic writing assistant.

If this argument resonates, I wrote a more practical follow-up on what this looks like with real Mac workflows, Codex, and messy office documents. The example is deliberately corporate: a board-deck narrative that starts to fall apart once the system reads the spreadsheet model, memo, notes, and approvals together.

<div style="text-align: center; margin: 2rem 0;">
  <a href="/posts/docmason-llm-knowledge-base/" style="display: inline-block; padding: 10px 18px; background-color: #111827; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">Read the practical DocMason walkthrough</a>
</div>

The argument over whether AI is amazing or disappointing will keep going in circles for a while.

That is fine. The two sides are often describing different systems, different workflows, and different memory conditions.

But one conclusion is already visible. Frontier agents look dramatically stronger in environments that give them structure, durable context, and feedback loops. Coding got there first because the repository was ready. The bigger opportunity now is to bring the same conditions to the rest of knowledge work.

## References

- Andrej Karpathy, April 2026 posts on X about the AI capability gap and "AI Psychosis": https://x.com/karpathy
- Andrej Karpathy, "LLM Wiki" idea file, April 5, 2026: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f