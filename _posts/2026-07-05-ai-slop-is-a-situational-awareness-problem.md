---
title: "AI Slop Is a Situational Awareness Problem"
description: "Two blind copywriting tests for a project called CodexWork showed that AI slop is rarely about bad English. It is a failure to read where the visitor is standing: which page they are on, what they already know, and what the next click should feel like."
date: 2026-07-05 00:00:00 +0800
categories: [AI, Model Evaluation]
tags: [llm-evaluation, model-selection, context-engineering, copywriting, ai-slop, codex, governance]
image:
  path: /assets/img/posts/2026-07-05-ai-slop-situational-awareness/cover.jpg
  alt: "Two glowing doorways above a webpage panel: one filled with tangled generic shapes representing marketing noise, the other empty except for a single guiding arrow of light"
---

I was not trying to find the smartest model. I was trying to write six lines of copy for a page nobody reads for more than four seconds.

That is the part people miss when they argue about which model is "best." Writing a landing page is not a poetry contest. It is a situational judgment test disguised as a writing task. The words are almost the easy part. The hard part is knowing where the visitor is standing when they read them.

I was building CodexWork, a small guide project to help non-technical office professionals use Codex for real work: reading files, researching the web, drafting documents, building decks, reviewing spreadsheets. It is not launched. It is not affiliated with OpenAI. It is just a thing I am building, and at some point I needed website copy, and I did not want to write it myself six times to find out which model actually understood the assignment.

So I ran two small, deliberately narrow tests. Not benchmarks. Blind copywriting exercises, model names hidden until after I judged the output.

## Why the normal benchmarks do not help here

Most model comparisons measure the wrong axis for this job.

They measure reasoning depth, code correctness, factual recall, instruction following at scale. All real. None of it tells you whether a model can write a homepage hero line that does not sound like it was assembled from the same fifty SaaS templates every AI product uses.

Landing page copy has a different failure surface. The model is not being asked to solve a hard problem. It is being asked to make one small, correct judgment call, over and over: *what does this specific visitor, on this specific page, already know, already fear, and already want to click next?*

Get that wrong and you get fluent, grammatically perfect, professionally formatted text that is still garbage. Not because the English is bad. Because the model answered a question the visitor was not asking.

I now think that is the actual definition of AI slop. Not bad wording. A failure to locate the reader.

![A visitor standing inside a page context, facing a clear surface while other panels fade into the background](/assets/img/posts/2026-07-05-ai-slop-situational-awareness/situational-awareness.jpg)
_The hard part is not making the sentence prettier. It is locating the reader inside the page._

## Test one: the homepage

The task was simple on paper. Write homepage copy for a fictional tutorial site that teaches non-technical office workers how to actually use AI at work. The audience was HR, ops, sales, finance, and admin workers — not engineers, founders, or AI enthusiasts. No hype, no theory, no productivity-guru voice.

The best output, from Claude Sonnet 5, did something the others did not. It did not describe the problem. It renamed it.

Instead of "learn how to use AI," it wrote something close to: *you don't have a technology problem, you have a "what do I actually type" problem.* That line is doing real work. It is not selling capability. It is naming the exact, specific, slightly embarrassing confusion the reader already feels but has not put into words. It understood that this audience does not need to be convinced AI is powerful. They already believe that. What they need is permission to admit they do not know what a good prompt even looks like.

Gemini 3.5 Flash wrote something structurally competent and hollow underneath. It invented social proof it had no right to claim — "join thousands of professionals" for a product that does not exist yet — and slipped in the kind of quantified promise ("save two hours a day") that the brief explicitly asked to avoid. Fluent English, wrong instinct: reach for the marketing reflex the moment the topic is AI productivity.

GPT-5.5 on low thinking was the safest version. Correct structure, no violations, nothing embarrassing. Also nothing anyone would remember five minutes later. It read like a policy document that happened to be about emails and meetings.

Gemini 3.1 Pro was closer, compact, with one sharp line ("You've tried ChatGPT. Now what?") undercut by a line the brief had specifically warned against — telling the anxious reader to stop "feeling behind the curve," which is the exact anxiety the whole product was supposed to defuse, not activate.

Sonnet 4.6 had some of the best individual phrases of the whole test — "built for people who work at desks, not in data centers" is a genuinely good sentence — but the model was not asked to build a website. It built one anyway, a full HTML page, when the task was copy. Good taste, wrong boundary.

Grok 4.3 was concise and thin. It said less, but it also understood less. The hero line ("work smarter with AI") was the exact generic phrase this kind of page should escape.

## Test two: the page that exposes real judgment

The second test was narrower on purpose, and more revealing.

Write only the above-the-fold copy for the CodexWork "Start Here" page. Not the homepage. The page a visitor reaches after they already decided they were interested. I did not spell out the visitor's exact hesitation. I wanted to see which model inferred it from the page position.

A visitor on a "Start Here" page has already been sold. Re-explaining the product here is not persuasion, it is friction. The correct move is to hand them the smallest possible first step and quietly answer whatever question is stopping them from taking it.

Claude Sonnet 5 got this right again, and the reason is more interesting than the fact that it won. Its H1 — "Give Codex your first real task" — did not introduce anything. It just moved the visitor forward one step, using language that assumed they already knew what Codex was. Its secondary link was the actual tell: *"Not sure what to ask? See example tasks."* That is not copy about the product. That is copy about the exact hesitation happening in the reader's head at that literal moment. No brief told it to write that. It inferred the hesitation from the page's position in the funnel.

GPT-5.5 low thinking did not produce the most striking line, but it produced the most disciplined page. Its flow — choose a task, add files and context, review the result — was internally consistent from the lead paragraph down to the card labels, and it was the only version, alongside Sonnet 5, that stayed honest about what the site actually is: a guide, not a connected product. It did not claim it could "connect your account," because it correctly modeled CodexWork as an independent teaching site rather than the tool itself.

That distinction sounds small. It is not. It is an entity boundary, and getting it wrong is a factual error dressed up as tone.

Sonnet 4.6 wrote the single best headline of the batch and then drifted straight back into homepage language for the lead paragraph, re-explaining what Codex does to someone who had already agreed to start. Good phrase generator, wrong sense of where it was standing on the page.

Gemini 3.1 Pro slipped into the same reflex from test one, opening with "discover how to turn Codex into your most reliable assistant" — the exact register a burned-out AI-tool-review reader has learned to skip. Worse, its reassurance line ("setup takes just 10 minutes") tried to soothe and instead raised the stakes, turning a zero-friction moment into a ten-minute commitment.

Grok 4.3 made the entity mistake outright: it wrote a button that said "Connect Codex" and a card labeled "Connect account," treating an independent guide site as if it were the product with OAuth and a login flow. Fluent, wrong facts about its own subject.

## The compact version, honestly

I want to be careful here, because it is tempting to turn this into a leaderboard, and the ranking is not the point. Two small blind tests on one narrow task is not a benchmark. It is a signal, not a verdict.

But the pattern across both tests was consistent enough to name:

| Role | What it actually did well |
|---|---|
| Sonnet 5 | Located the reader's unspoken next question and answered it directly |
| GPT-5.5 (low) | Held the factual and structural boundaries without drifting or inventing |
| Sonnet 4.6 | Produced strong individual lines, weak sense of page and task boundaries |

Three roles, not three ranks. That framing turned out to matter more than the scores.

![Three connected model roles labeled judgment, discipline, and phrasing](/assets/img/posts/2026-07-05-ai-slop-situational-awareness/model-roles.jpg)
_For this task, the useful split was not a leaderboard. It was a division of labor._

## This is the same failure I keep finding everywhere

I have written before about why [vibe coding is not a prompting problem but a governance problem](https://jetxu-llm.github.io/posts/vibe-coding-is-not-prompting-it-is-governance/) — the repository becomes the real system once an agent works unsupervised for an hour, and what matters is what the repo makes legal, repeatable, and hard to forget.

Copywriting judgment is the same failure mode wearing a different shirt.

A landing page also has law. Not written in an `AGENTS.md`, but real all the same: what page this is, what the visitor already believes, what they are afraid of admitting, what the next click should feel like. A model that writes fluent English but does not read that law will still produce something a real reviewer has to catch — an invented statistic, a wrong entity claim, a re-sold pitch on a page where the sale already happened.

That is also why I no longer expect one model to be good at everything, and why I stopped being surprised when it isn't. I have written about the industry's slow admission that a single ["God Model"](https://jetxu-llm.github.io/posts/the-death-of-the-god-model/) tuned to be great at all things ends up biased toward none of them — logic-heavy models trained hard on reasoning benchmarks, aesthetic ones trained toward fluent creative surface. What I saw in these two tests was a small, concrete instance of that split. One model was better at reading the room. A different model was better at not lying about what room it was in. Neither trait bought the other one for free.

The [digital-staff-engineer argument](https://jetxu-llm.github.io/posts/the-future-of-ai-code-review-is-a-digital-staff-engineer/) I made about AI code review runs on the same logic. A code reviewer that does not know the company cannot review the company's code, no matter how good it is at reading diffs in the abstract. A copywriting model that does not know which page it is on, and what the visitor already knows, cannot write good copy for that page, no matter how good its English is.

## What I am actually doing with this

For CodexWork, the practical decision was straightforward once I stopped trying to find one model to trust for everything.

Sonnet 5 writes the first draft, because it is the one that consistently locates the reader before it writes the sentence.

GPT-5.5 on low thinking reviews it, because it is the one that will not let an invented number or a blurred product boundary slip through just because the sentence sounds confident.

Sonnet 4.6 stays in the rotation as a phrase generator for headlines and card labels, not as the model that owns a page end to end. Good ear, unreliable sense of scope.

That is not a hierarchy. It is a division of labor, which is the same conclusion I keep reaching every time I look closely enough at any serious AI-built system.

So the question I would actually ask, if you are choosing a model to write real copy for a real site, is not "which model writes the best English." It is two smaller questions that matter more:

Which model understands the moment the reader is in?

And which model will still tell you the truth about your own product when the sentence is tempting to write anyway?
