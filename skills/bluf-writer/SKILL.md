---
name: bluf-writer
description: >
  Rewrites any draft text as a military-style BLUF memo (Bottom Line Up Front).
  Use this skill whenever the user wants to restructure a document, email, report,
  or update into BLUF format — or says anything like "BLUF this", "make this
  bottom line up front", "turn this into a memo", "military memo style", "make
  this more direct", or "cut to the chase". Also trigger when the user shares a
  long rambling draft and asks for help making it clearer or more concise — BLUF
  rewriting is often the right answer even if they don't name it.
---

# BLUF Writer

You are rewriting a draft into a formal military memorandum. The reader is busy
and decision-focused. They need to know the bottom line before they read a single
word of context.

## The memo structure

Produce exactly this format — no more, no less:

```
MEMORANDUM FOR [Recipient]

FROM:    [Sender]
DATE:    [Date]
SUBJECT: [Active-voice subject line — what this memo does, not what it's about]

1. BLUF. [One sentence. The bottom line: what the reader needs to know or do, and
   why it matters to them. No hedging, no wind-up. If they read nothing else,
   they read this.]

2. BACKGROUND. [Why this is being written. One to three sentences of context.
   Only what the reader needs to understand the situation — nothing they already
   know.]

3. DISCUSSION.
   a. [First supporting point]
   b. [Second supporting point]
   c. [Additional points as needed]

4. RECOMMENDATION. [Concrete action, clearly assigned. Who does what, by when.
   If multiple actions are needed, use sub-bullets (a, b, c). If the memo is
   purely informational, label this section ACTION REQUIRED or INFORMATION ONLY
   and state what, if anything, is expected of the reader.]

5. POC. [Point of contact name and how to reach them, or "See above" if the
   sender is the POC.]
```

## How to handle missing information

- **TO/FROM/DATE unknown**: Infer from context where possible (e.g., the draft
  mentions a team or a name). If genuinely unknown, write `[RECIPIENT]`,
  `[SENDER]`, or `[DATE]` as placeholders — don't ask, keep moving.
- **Date not mentioned**: Use today's date if it's clear from context; otherwise
  use `[DATE]`.

## Writing principles

**BLUF line**: Extract the single most important conclusion or request from the
entire draft. State it in one declarative sentence. "X is Y" or "X requires Y
by Z." If the draft buries the recommendation at the end, surface it. If it
contains multiple competing points, pick the one with the highest stakes.

**SUBJECT line**: Write it as an action or decision, not a topic. Not "FY26
Budget" but "Approve FY26 Budget Increase of $2.4M." Active verb, specific noun.

**Discussion section**: This is the only place for nuance. Distill the draft's
supporting evidence into the minimum set of facts the reader needs to trust the
BLUF and act on the recommendation. Cut anything that doesn't directly support
those two things.

**Prose style**: Short sentences. Active voice. No hedging ("it may be the case
that"). No filler ("In conclusion", "As mentioned above"). Numbers and specifics
over vague language — "delayed by 14 days" not "significantly delayed."

**Length**: A well-written BLUF memo is short. Background: 2–3 sentences.
Discussion: 3–6 bullets. Recommendation: 1–3 actions. If the source material
is genuinely complex, you may expand — but question every line. The reader's
time is the constraint.

## After producing the memo

Output the memo only — no preamble, no explanation, no "Here is your rewritten
memo." Just the memo.

If anything critical is missing (e.g., the draft contains no clear recommendation
and you cannot infer one), add a single line after the memo:

> **Note:** No clear recommendation was found in the draft. The RECOMMENDATION
> section above is my best inference — confirm or replace before sending.
