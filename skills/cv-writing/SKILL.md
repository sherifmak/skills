---
name: cv-writing
description: >-
  Craft principles for writing, editing, and reviewing CVs and resumes — covers
  bullet structure, verb altitude, quantification, role-header formatting, and
  the diversity-over-depth ordering that distinguishes senior-level CVs. Use
  whenever the user explicitly asks for help with a CV or resume: writing a new
  bullet, rewriting an existing one, reviewing the whole CV, tightening a role
  section, choosing between two phrasings, or asking "is this bullet good."
  Triggers include phrasings like "review my CV", "make my CV better", "what
  should I improve on my resume", "audit my CV", "rewrite this bullet", "is
  this bullet good", "tighten this role", "make this more senior", "cut the
  weasel words". This skill does not auto-fire on every file edit — wait for
  an explicit ask. It informs craft only; it does not source facts, invent
  numbers, or decide what content is allowed (those are project-level concerns).
---

# CV Writing

A craft skill for writing senior-level CV bullets and auditing CVs as a whole.
The rules below are deliberate — each one corresponds to a failure mode that
makes a CV read as junior, generic, or padded.

You operate in one of two modes depending on the ask:

- **Authoring** — the user wants you to write or rewrite a bullet, a role
  section, or a header. Apply the rules as you draft. When a draft violates
  a rule, write the bullet *and* flag the violation inline with a concrete
  alternative; let the user override.
- **Review** — the user wants a take on the CV or a role section as a whole.
  Phrasings: "review my CV", "make this better", "what should I improve",
  "audit this", "where is this weak." Read the whole thing first, form a
  holistic impression, then back it with evidence. Don't rewrite unless
  asked — review is diagnosis, not surgery.

Default to flag-and-suggest, not hard rejection. If a user knowingly keeps
a "helped" or an unquantified claim, that is their call.

---

## Before you write: gather context

A CV bullet is only as strong as the evidence under it. Bullets built on
plausible-sounding but unsourced numbers fail under reference checks and
quietly damage the user's trust in your output. Before authoring anything
beyond a trivial rephrase, run this short sequence — even when the user
seems impatient.

1. **Survey what's already in reach.** Look at the working directory and
   any attached or shared files first: performance reviews, project docs,
   internal knowledge bases, talk transcripts, GitHub activity, earlier
   CV variants, project READMEs, prior briefs. These are usually the
   richest source of grounded claims. Also re-read the conversation —
   the user may have already given you the metrics you need earlier in
   the thread or in a CLAUDE.md / AGENTS.md file.

2. **Ask before searching wider.** If what's in reach isn't enough, *ask
   the user* before searching local files outside the working directory,
   shelling out to git history, or hitting the web (LinkedIn, GitHub
   profiles, conference pages, press coverage). Don't silently scan
   their machine or their online presence to "be helpful" — confirm
   scope first, even if it would be quicker not to. The user should
   always know when and where you are looking for material about them.

3. **Surface gaps before drafting.** If after step 1 (and a sanctioned
   step 2) you still don't have the input needed to back a specific
   claim, name the gap before you write. Offer the user two options:
   *provide the metric themselves*, or *authorize you to go find it*.
   Don't draft a bullet around a missing fact and hope it lands — that
   is how fabrications happen. A bullet with the right scope and
   altitude but a missing number is fine to ship as a placeholder if
   the gap is named explicitly to the user.

This applies primarily to authoring. Review mode operates on the page
that already exists — you don't need external facts to diagnose what's
there. You may still surface "I can't verify this claim from anything
I have access to" as a review finding when a number looks load-bearing
but unsourced.

---

## Guiding rules

Every rule has a reason. The reason is what lets you judge edge cases.

### 1. Role header format is identical for every role

`Company — Role, Location, Date`. Same separator (em dash), same field order,
same shape across all roles. Why: the eye scans a CV vertically; visual
parallelism between role headers signals discipline and lets the reader find
each role in milliseconds. Mixed shapes ("Company, Role" then "Role at
Company") read as carelessness.

### 2. No bold, no italics, no quotation marks

Anywhere. Why: a CV under 8-second scan has no time to parse what emphasis is
trying to say. If a phrase needs bold to land, the phrase isn't strong enough —
fix the phrase. Quotation marks invite the question "whose words?" and often
imply borrowed credit. Plain text forces the writing to do the work.

### 3. Verb at the start of every bullet; end with the outcome

`Led X, [doing Y], [resulting in Z].` The outcome at the end is what the
reader remembers. A bullet that opens with the verb and closes with the
number is the canonical shape.

**Tense:**
- **Past roles** — past tense only. "Built the data platform that…"
- **Current role** — either tense is acceptable convention. Present tense
  ("Lead a team of 12…") is widely used and signals "this is what I do
  now"; past tense ("Led a team of 12…") frames everything as already-
  completed accomplishment and tends to read stronger because every
  bullet closes on a result rather than an ongoing activity. Pick one
  for the role and stay consistent — mixing tenses within a single
  role's bullets is the actual failure mode.

The deeper rule is *don't write job descriptions*. A bullet that reads as
"here is what my job is" rather than "here is what I have done" lands as
junior regardless of tense.

### 4. Quantify whenever the claim is quantifiable

A number with no anchor is half a number. "Grew users by 40%" is weaker than
"Grew users by 40% in 6 months, from 200K to 280K." Anchor numbers to a
baseline (from X to Y), a timeframe (in N months), or a multiple (3x over
prior year). Why: senior readers calibrate scale against context; an absolute
number without context could mean anything.

If a claim is not quantifiable (e.g., "shaped product strategy"), don't fake
a number — sharpen the verb and the scope instead.

### 5. No weasel words

Banned openers: *helped, assisted, contributed to, was involved in,
participated in, supported, worked on, played a role in.* Why: every one of
these is a hedge that lets the reader assume the writer was peripheral. If
you genuinely contributed but did not lead, name the specific contribution
("Designed the auth schema adopted across 4 teams") rather than hedging at
the verb.

### 6. Most recent role gets the most detail; older roles degrade gracefully

A reader spends most of their attention on the last role and skims the rest.
A 7-year-old role with 8 bullets pulls weight away from the current one.
Typical shape: current role 5–7 bullets, prior role 3–5, the one before 2–3,
anything further back 1–2 or compressed into a single line.

---

## Bullet ordering within a role

Bullets are *ordered*, not chronological. Ordering is a narrative choice. The
goal: a reader who scans only the first two bullets still gets the most
important story; a reader who reads all of them gets the full picture.

### Bullet 1 — Scope + altitude

The biggest framing number and the seniority signal. Headcount managed,
roadmap dollar size, reporting line, geographic or org breadth.

Example: `Led product for the $900M payments platform, 21-person team across
PM, design, and data, reporting to the SVP of Platform.`

This bullet exists to set the stage. Without it, every subsequent bullet
floats without context.

### Bullet 2 — Flagship win

The single thing you want the reader to remember from this role. Highest
specificity, biggest outcome, named product or initiative.

Example: `Launched the unified checkout that replaced 3 legacy stacks,
shipping in 9 months and lifting conversion from 62% to 71%.`

### Bullets 3+ — Diversity over depth

Each remaining bullet covers a *distinct* axis. The axes are roughly:

- **User impact** — what changed for customers (adoption, retention, NPS)
- **Technical innovation** — what was novel in how it was built
- **Org influence** — what changed in how the team or company operates
- **Evangelism / external** — talks, customer wins, partnerships, press
- **Revenue / business** — what moved on the P&L

One bullet per axis. Why: at senior levels, breadth is the differentiator —
peers can all ship features, but few can show evidence across user, tech,
org, and market in one role. Two bullets on the same axis (e.g., two adoption
metrics) waste a slot.

---

## Verb altitude

The opening verb is the seniority signal. Senior-coded verbs imply ownership
and initiative; junior-coded verbs imply assistance.

**Prefer:** Led, Owned, Drove, Pioneered, Cultivated, Generated, Launched,
Scaled, Architected, Founded, Established, Shipped, Tripled, Doubled,
Negotiated, Authored, Defined.

**Avoid:** Helped, Assisted, Supported, Worked on, Participated in,
Contributed to, Was involved in, Played a role in, Coordinated (weak unless
the coordination *is* the win), Collaborated on.

**Edge cases:**
- *Managed* is neutral — fine for line-management facts ("Managed 12 PMs
  across 4 squads"), weak as an accomplishment verb.
- *Built* is fine for ICs but reads small for directors. Prefer *Launched*
  or *Shipped* when the thing went to production at scale.
- *Drove* is strong for influence; *Led* is strong for authority. Pick by
  whether you had positional power or earned it.

---

## Credibility levers

Specificity beats adjectives. The reader is calibrating two things in
parallel: *did this person do real work?* and *was the context impressive?*

Name-drop deliberately:
- Industry-recognized companies ("partnered with Snowflake", not "partnered
  with a major data platform")
- Named products ("integrated with Stripe Connect")
- Named standards or frameworks ("SOC 2 Type II", "GDPR Article 17",
  "OpenAPI 3.1")
- Named conferences, publications, or stages ("keynoted re:Invent 2024")

Avoid adjective stacks ("highly successful, cross-functional, strategic
initiative"). They consume words without adding signal.

---

## Flag-and-suggest pattern

When a user asks you to write a bullet and their inputs produce a draft that
violates a rule, follow this shape:

1. Write the bullet as drafted (or the best version of what they gave you).
2. Flag the violation in a short line beneath it.
3. Offer a concrete alternative.
4. Let the user pick.

**Example 1 — weasel word:**

> Draft: `Helped launch the new pricing model, leading to higher revenue.`
>
> Flag: opens with *Helped* (weasel) and *higher revenue* is unanchored.
>
> Alternative: `Launched the usage-based pricing model that lifted ARR by
> 18% ($14M) in the first two quarters.`

**Example 2 — unquantified outcome:**

> Draft: `Drove adoption of the new onboarding flow across the customer base.`
>
> Flag: no quantification of "adoption" or "customer base."
>
> Alternative: `Drove adoption of the new onboarding flow to 84% of monthly
> active accounts (up from 31%) within 4 months of launch.`

**Example 3 — job description shape (no outcome):**

> Draft: `Leading a team of 12 engineers building the data platform.`
>
> Flag: reads as job description, not accomplishment — no outcome
> attached, and the doubled -ing form (*Leading … building*) softens the
> action. Tense itself isn't the problem (present tense is fine for a
> current role); the missing result is.
>
> Alternative (past tense): `Led a 12-engineer team that shipped the
> unified data platform, cutting nightly batch time from 9 hours to 47
> minutes.`
>
> Alternative (present tense, current role): `Lead a 12-engineer team
> that has shipped the unified data platform, cutting nightly batch time
> from 9 hours to 47 minutes.`

If the user pushes back ("I don't have a baseline for that number"), respect
it. The rule's purpose is to surface the gap, not to fabricate.

---

## How to review a CV

A good review is diagnosis, not a pass-fail walk. A senior reviewer reads
the whole thing, forms a holistic impression, and then justifies it with
evidence. The rules above are the lens — they tell you *what* to attend to,
not a checklist to run.

### The shape of a review

1. **Read the whole CV first.** Don't comment as you go. You're trying to
   land an overall impression: does this read as senior or junior?
   focused or scattered? confident or hedged? padded or sparse? specific
   or generic? Whatever the dominant impression is, that's your lead.

2. **Lead with the impression, then back it with evidence.** Open with one
   or two sentences naming what you see. Then quote the bullets or
   passages that produce that impression, and propose concrete fixes for
   the highest-leverage ones. Vague critique ("this could be stronger")
   is worthless; specific critique with a rewrite is what the user can
   act on.

3. **End with prioritized next actions — 3 to 5, ordered by impact.** The
   reader of a CV spends most of their attention in the first 8 seconds.
   Fixes that change what a scanner sees (header consistency, the lead
   bullet of the current role, the opening verb on bullet 1) outrank
   fixes deeper in the document. Order accordingly.

### Signals to weigh while reading

These are the things to attend to. Don't enumerate them as pass/fail —
notice when they show up, and weave them into the impression.

- **Scan vs. read.** What does an 8-second scan tell a reader? If the
  scanner sees weak verbs, no numbers, or inconsistent role headers, the
  read never happens.
- **Verb altitude.** Do the openers sound like the work of a leader or an
  assistant? A single "Helped" or "Worked on" anywhere senior in the
  document drags the whole CV down a level.
- **Quantification gaps.** Which claims could be quantified but aren't?
  Which numbers are floating without a baseline?
- **Axis stacking within a role.** Is the role telling one story (e.g.,
  three bullets all about adoption metrics) when it should be telling
  four? Diversity of evidence is what reads as senior breadth.
- **Bullet ordering inside each role.** Does bullet 1 set scope? Is the
  flagship win in position 2? Or is the most impressive thing buried at
  the bottom where no one will see it?
- **Role-length curve.** Is the most recent role the densest? Or is a
  five-year-old job still carrying eight bullets it doesn't earn?
- **Formatting artifacts.** Stray bold, italics, or quotation marks. Mixed
  role-header shapes. Tense drift within a single role's bullets (past
  roles must be past tense; current role can be either, but pick one).
- **Specificity vs. adjective stacks.** Named companies, products, and
  standards versus vague descriptors ("highly successful cross-functional
  initiative").

### What a review output looks like

```
Overall: [one or two sentences naming the dominant impression]

Where it shows up:
- [Quoted bullet or passage]
  Why this lands the impression: [short]
  Fix: [concrete rewrite or change]

- [Next one]
  …

If I were prioritizing:
1. [Highest-impact change, usually something visible to the 8-second scan]
2. [Next]
3. [Next]
```

Adapt the shape to the size of the ask. A "is this bullet good?" question
gets a two-line answer, not the full structure. A "review my whole CV"
gets the full thing.

---

## Out of scope

This skill is about craft, not content. It does not:

- Decide what claims are allowed (sourcing, factuality, "is this number
  real" — those are project-level concerns).
- Invent numbers, baselines, or outcomes. If the user asks for a bullet
  about X and there's no underlying metric, ask for the metric or sharpen
  the verb instead of fabricating.
- Choose which roles to include or how far back the CV should go.
- Translate to other formats (LinkedIn summaries, cover letters, bios). The
  bullet rules transfer; the structural rules (role header shape, bullet
  ordering) often don't.
