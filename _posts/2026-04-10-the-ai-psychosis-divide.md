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

> **TL;DR:** We are entering a "Folded" AI reality. In the upper layer, software engineers deploy AI agents that autonomously rewrite entire codebases while they sleep. In the lower layer, top-tier consultants and strategy leads are stuck copy-pasting PDFs into chat boxes, receiving slightly smarter autocomplete. The biggest lie in productivity right now is that you need better "prompt engineering." You don't. The gap is about autonomy. If you are still manually feeding text into a passive chat box and waiting for an answer, you are trapped in the lower fold. Here is why the white-collar world is being left behind, and the only way to break through.

Two intelligent people can use "AI" every day and walk away with opposite conclusions.

One sees ChatGPT miss obvious questions, stumble on simple voice tasks, and produce polished nonsense on demand. From that angle, the hype looks inflated. 

Another watches Codex or Claude Code spend an hour inside a repository, trace dependencies across dozens of files, run tests, fix failures, and come back with a coherent strategic patch. From that angle, the complacency looks absurd.

Both impressions are completely real. They just happen in different spaces.

That is why Andrej Karpathy's phrase "AI Psychosis" landed so hard this month. It named a social fact many technical people had been feeling: the people who are closest to frontier agentic workflows are no longer living in the same digital reality as everyone else.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-gap.png" alt="Karpathy tweet on AI capability gap" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

The lazy explanation is that programmers simply know how to prompt better. The terrifying explanation is a concept from science fiction: the "Folded City."

## The Folded AI Reality

In Hao Jingfang's sci-fi novel *Folding Beijing*, the city is physically and temporally segregated into isolated layers. The elite First Space enjoys a 24-hour cycle of clean air, structure, and uninterrupted progress. The Third Space is forced into the darkness, processing the city's waste in compressed, fragmented time, completely blind to how the upper layer operates.

We are witnessing the exact same stratification in AI.

In the **First Space**, software engineers are handing AI agents entire codebases. A codebase is a pristine, deterministic environment. It has assembled intent: source files, tests, config, docs, and explicit pass/fail checks. The AI can inspect, modify, run, verify, and revise autonomously. Every action compounds. The AI exists in continuous, unbroken time. 

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-psychosis.png" alt="Karpathy tweet defining AI Psychosis" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

In the **Third Space**, analysts, strategists, and $800-an-hour consultants are operating in fragmented time. Their "codebase" is a dark, sprawling swamp of business files: decks, spreadsheets with hidden tabs, poorly formatted legal PDFs, half-finished memos, and long email chains. 

Because AI cannot naturally breathe in this swamp, consultants are forced to act as digital waste management. They manually excerpt 10 pages of a PDF, paste it into a stateless chat window, get a one-off summary, copy the text to a PowerPoint, and close the tab. 

When the tab closes, the AI dies. It learned nothing. It built nothing. 

The next day, they start entirely from zero.

This is the deep anxiety many top-tier knowledge workers silently feel. You pride yourself on structural, MECE (Mutually Exclusive, Collectively Exhaustive) thinking. Yet your intellectual relationship with AI is pure chaos. You are not wielding an engine; you are constantly fighting against amnesia.

## The Cognitive Trap in Office Work 

This is the failure point many product and feature discussions miss.

Most white-collar AI use is trapped in a copy-paste chat paradigm. You ask a question, you get an answer, you move on. The system never maintains a stable, compounding map of your territory. It rediscovers knowledge from scratch every single time.

That is tolerable for drafting a quick email. It becomes a fatal liability when the real task spans a quarterly board deck, a conflicting CFO spreadsheet model, and three legal memos. A generic chat window cannot maintain a disciplined memory of how those files reinforce or contradict one another over a three-month engagement. 

If your AI forgets everything when you close the tab, you are structurally trapped in the lower fold.

Meanwhile, First Space systems have improved fastest because their environment supplies both rich context and hard feedback loops. But non-technical crowds react to a different product surface. In their experience, AI feels like a clever, forgetful intern that guesses too often. This disagreement will sound irrational until white-collar workers realize they are fighting with one hand tied behind their back, lacking the infrastructure to give the model true *working memory*.

## Stop Chatting. Start Compiling.

How do you break into the First Space?

You must change what you are doing with your files. Karpathy's most important post this month was not about "AI Psychosis" at all. It was a quieter post a week earlier on the concept of "LLM knowledge bases."

The key shift is profound: stop treating documents as static inputs to query against, and start treating them as raw material for a persistent, interlinked knowledge artifact.

<div style="text-align: center; margin: 2rem 0;">
  <img src="/assets/img/posts/2026-04-10-ai-psychosis-divide/tweet-llm-kb.png" alt="Karpathy tweet on LLM Knowledge Bases" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
</div>

His phrasing in the idea gist is unusually clear: *"The knowledge is compiled once and then kept current, not re-derived on every query."*

That one sentence reframes the problem from better retrieval (RAG) to better *accumulation*. Instead of uploading files and hoping a chatbot rediscovers the right fragments on demand, a background AI model incrementally reads, summarizes, cross-references, updates, flags contradictions, and maintains a local Wiki that grows richer with every new financial model or interview transcript you drop into the folder.

In this architecture, your messy office files are the raw material. You curate them. The model does the bookkeeping. 

Humans abandon personal knowledge bases because maintenance is tedious. Cross-links drift, summaries go stale, contradictions pile up. LLMs, however, are built to swallow that exact maintenance burden without ever getting bored. The center of gravity is moving from *"can AI read my doc?"* to *"how does my AI-maintained memory system stay reliable over a 6-month consulting project?"*

## Crossing the Divide

The next meaningful AI product for white-collar work will not be a prettier chat window. It will be a local compiler for your messy knowledge.

It will ingest the ugly reality of your desk: decks with speaker notes, spreadsheets with hidden projections, and meeting transcripts with no naming discipline. It will preserve their structure rather than flattening them into anonymous text. It will maintain memory instead of pretending every prompt is the first day on the job. And it will show its work, because persistent systems need provenance and contradiction handling to earn professional trust.

This is how you escape the Third Space. It is the only way a consultant or strategist can survive the acceleration.

It starts when you stop pasting PDFs into web panels, and instead drop forty ugly, confidential project files into a local workspace. You let an agent build a maintained context around them, and then you watch the system surface a hidden liability in the valuation model that the entire deal team missed for a week.

<div style="text-align: center; margin: 3rem 0; padding: 2rem; background: #fafafa; border-radius: 8px; border: 1px solid #eaeaea;">
  <h3 style="margin-top: 0;">The Antidote to the "Folded AI" Era</h3>
  <p style="color: #666; margin-bottom: 1.5rem;">DocMason bridges the gap, turning idle AI capacity into an autonomous agent that runs directly against your messy office files.</p>
  <a href="/posts/docmason-llm-knowledge-base/" style="display: inline-block; padding: 12px 24px; background-color: #111827; color: white; text-decoration: none; border-radius: 6px; font-weight: 600; font-size: 1.1rem; transition: background-color 0.2s;">Read the DocMason Walkthrough</a>
</div>

The biggest lie in productivity right now is that you need better "prompt engineering." You don't. The gap isn't about how well you type instructions. It's about autonomy. 

The argument over whether AI is a miracle or a disappointment will keep going in circles as long as people use it as a passive chatbot that needs constant hand-holding. Coding got there first because the digital repository was ready for agents to do the driving. 

**In 2026, an AI tool without Agentic feature is already outdated.** 

If you are still manually feeding text into a chat box and waiting for an answer, you are structurally trapped in the lower fold.

## References

- Andrej Karpathy, April 2026 posts on X about the AI capability gap and "AI Psychosis": https://x.com/karpathy
- Andrej Karpathy, "LLM Wiki" idea file, April 5, 2026: https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f
