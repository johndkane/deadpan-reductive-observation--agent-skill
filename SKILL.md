---
name: deadpan-reductive-observation
description: Transform supplied observations into concise deadpan reductive one-liners, and generate researched alternatives when requested.
---

# Deadpan Reductive Observation

## Purpose

Transform any supplied observation into a concise **deadpan reductive observational one-liner**.

When alternatives are requested, also research the subject enough to identify stronger, more specific, more relatable, or more culturally relevant angles before generating options.

## Core Style

Reframe the subject as an unexpectedly mundane, literal, or absurd description of what it effectively consists of.

Common patterns:

> X is just Y.

> X is mostly just Y.

> X is basically Y.

The humor should come from the accuracy of the reduction, not from an explicit joke or punchline.

## Primary Task

Given an observation:

1. Identify the underlying behavior, contradiction, ritual, inconvenience, or social dynamic.
2. Strip away the conventional framing or importance attached to it.
3. Reduce it to what people are actually doing.
4. Find the smallest surprising description that remains recognizably true.
5. Write one concise, confident, deadpan sentence.

## Research Mode

When the user asks for alternatives, stronger options, more topical versions, or better engagement:

1. Research the topic, subject, place, activity, community, product, event, or cultural context when useful.
2. Look for:
   - recognizable habits
   - recurring frustrations
   - stereotypes grounded in observable behavior
   - distinctive terminology
   - current trends or references
   - commonly discussed experiences
   - specific details that make the observation feel true
3. Prefer primary or credible current sources for factual details.
4. Do not merely paraphrase search results; use research to discover better comedic angles.
5. Avoid obscure references unless they materially improve the joke.
6. Never invent facts for the sake of humor.

## Alternative Generation

When alternatives are requested:

- Generate several genuinely different angles, not minor rewrites.
- Prefer specificity over generic cleverness.
- Include the strongest straightforward reduction first.
- Explore different dimensions where relevant, such as:
  - social behavior
  - logistics
  - money
  - technology
  - relationships
  - bureaucracy
  - local culture
  - recurring rituals
  - contradictions between expectation and reality
- Keep every option independently understandable.

## Rules

- Usually one sentence per observation.
- Keep it concise.
- Prefer concrete behavior over abstraction.
- Use understatement.
- Preserve the underlying truth.
- The line should feel obvious in retrospect.
- Do not explain the joke.
- Do not label the humor.
- Avoid conventional setup/punchline structures.
- Avoid puns unless unusually natural.
- Avoid elaborate metaphors.
- Avoid meme phrasing unless the subject specifically calls for it.
- Avoid forcing `just`, `mostly just`, or `basically` into every line.
- Match casual social-media language.
- Lowercase styling is acceptable when it suits the source tone.
- Output only the rewritten observation unless the user requests alternatives, explanation, or research.

## Quality Test

Before returning a line, ask:

- Is it recognizably true?
- Is the reduction unexpected?
- Is there a concrete human behavior inside it?
- Could anything be removed without losing the joke?
- Does it sound observed rather than written?
- Would explaining it make it worse?

If not, rewrite it.

## Examples

Input:
> Planning a weekend trip with friends usually involves lots of discussion but nobody commits.

Output:
> a weekend trip with friends is just four group chats slowly agreeing not to go anywhere

Input:
> Dogs and their owners are constantly checking what the other one is doing.

Output:
> owning a dog is mostly just following each other around the house to see what happens next

Input:
> Video meetings often involve people waiting for someone to realize they're muted.

Output:
> a video meeting is just six people watching one person discover the mute button

Input:
> Grocery shopping when hungry makes you buy things you never planned to get.

Output:
> grocery shopping hungry is just letting your stomach spend your money
