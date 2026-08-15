---
name: human-narrative-craft
description: Use whenever writing, drafting, continuing, or revising fiction — short stories, novel chapters, scripts, or any narrative creative writing — even if the user only says "write a story about X." Also use when a user asks to make writing sound less AI-generated, less like "AI slop," more human, more literary, or wants a critique of a draft for AI tells. Grounded in the StoryScope research (Russell et al., COLM 2026), which found that AI fiction is identifiable both by discourse-level narrative *choices* (plot shape, causality, temporal structure, character agency) and by sentence-level style habits — so fixing one without the other leaves signal on the table. Trigger this proactively for any task involving plot, character, or story structure, since these choices get locked in early and are hard to fix after a draft is finished.
---

# Human Narrative Craft

## Why this exists

A 2026 study (StoryScope, Russell et al.) trained classifiers to tell human short
stories apart from AI ones — Claude, GPT, Gemini, DeepSeek, and Kimi — using only
*narrative* features (plot shape, causality, temporal structure, agency) with
every stylistic cue (word choice, sentence rhythm, figurative density) removed.
Those narrative-only features still hit 93% accuracy. The five AI models cluster
tightly together in "narrative space"; human stories are far more scattered and
occupy the rare, unusual regions almost twice as often. In short: **the tell
isn't the prose, it's the structure of the decisions underneath the prose.**
That's what this skill is for — making the underlying decisions differently, not
just varnishing the sentences afterward.

Apply this at the *planning* stage, before or while drafting — these are
structural choices, not a copyedit pass you can run at the end.

## The five AI tells to actively avoid

For each, the AI-typical rate vs. the human rate is given so you know how strong
the default pull is.

**1. Over-explaining the theme.** AI stories have the narrator state the moral or
meaning outright 77% of the time (vs. 52% for humans). Fix: let the theme live in
what happens, not in a sentence that names it. If you've written a line where the
narrator or a character summarizes "the lesson," cut it or bury it in something
more oblique.

**2. A single tidy plot thread.** AI stories skip subplots 79% of the time (vs.
57% for humans) and resolve almost entirely through the protagonist's own choices
(69% vs. 46%), usually ending in quiet internal acceptance. Fix: give the story at
least one subplot that doesn't perfectly serve the main theme — a contrasting or
independent thread, not a mirror of it. Let something outside the protagonist's
control matter to the ending.

**3. Emotion rendered only through the body.** AI conveys feeling via physical
sensation and bodily metaphor 81% of the time (tight chest, cold sweat) vs. 38%
for humans, and reaches for smell-imagery constantly (82% vs. 57%). Fix: sometimes
just name the feeling plainly ("she was afraid," used 29% of the time by humans
vs. 8% by AI). Mix registers — direct naming, behavior, and bodily sensation — 
rather than defaulting to the body every time.

**4. Linear, single-track time.** AI stories tell events in the order they
happened far more consistently than humans, who jump in time, flash back, and
delay revelations more often. Fix: consider whether the story is more interesting
told out of order — opening on a consequence and working backward, or
withholding a fact the narrator already knows.

**5. Vague, generic allusions.** AI references other works and culture in vague,
unnamed ways 72% of the time (vs. 50% for humans), and rarely addresses the
reader directly (7% vs. 28%) or breaks the fourth wall (39% vs. 67%). Fix: use
specific, named references — an actual book, song, painter, street — rather than
"a novel about loss." Consider, at least occasionally, letting the narrator
acknowledge the reader is there.

## What to do instead — five moves that read as human

1. **Let a subplot go somewhere the theme doesn't.** Not every thread needs to
   rhyme with the main one.
2. **Make the protagonist's central choice morally ambiguous.** Humans write
   ambivalent, defensible-but-wrong choices 59% of the time; AI defaults to clear
   moral framing 62% of the time. Resist giving the reader an obviously correct
   answer.
3. **Break linear time on purpose.** A flashback, a flash-forward, or an opening
   that starts after the ending and loops back all read as more human than strict
   chronology.
4. **Let the ending stay a little open.** AI favors resolutions of internal
   understanding/acceptance; humans are more comfortable leaving something
   unresolved or externally decided (a person, an accident, bad luck).
5. **Name things.** Real books, real places, real brands, specific sensory
   details tied to a particular world — not placeholder generality.

## Aim for the statistically unusual choice

The paper measures each story's "rarity" — how far it sits from its nearest
neighbors in narrative-feature space. Human stories score rarer than AI stories
(mean percentile 0.71 vs. 0.49), and are wildly overrepresented in the rarest
tail: 24.7% of human stories land in the top 10% rarest, vs. 7.1% of AI stories.
AI stories aren't just individually predictable — across many different
prompts, the five AI models keep landing in the *same* narrow region of
narrative-choice-space as each other, while different human authors scatter
widely.

Two practical consequences:

- **Within a story**, at each major decision point (how a character is
  introduced, how a revelation lands, how the ending resolves), ask what the
  obvious/expected choice is — the one this skill's checklist would predict —
  and consider making a different one, as long as it still serves the story.
  Not every choice needs to be unusual; a story of all-unusual choices reads as
  try-hard. But a story of all-default choices is exactly the AI cluster.
- **Across stories**, don't let your own "human-coded" moves calcify into a new
  formula (e.g., every story gets exactly one flashback and one named book
  reference). The point isn't a checklist of tics to insert — it's making the
  actual decision fresh each time, the way different human authors land in
  different places rather than one cluster.

## Sentence-level style tells

Everything above is about narrative *structure*, which is the paper's central
claim — that structure survives even after prose is stylistically edited.
But the paper's own numbers also show style alone gets you most of the way
there (85.8% macro-F1 from style features alone, barely behind the 30-feature
structural core at 84.8%). Structure and style are both real signals, and
independent readers tend to notice style first. Three sentence-level habits
are worth watching, on top of everything above:

**The interruption-correction rhythm.** A recurring pattern — *statement, em
dash, a corrective or qualifying clause, return to the sentence* ("Not the
pin — that stayed...") — reads as careful and literary in small doses and as a
tic in large ones. If most paragraphs contain one, that rhythm is doing the
same job as a stylistic fingerprint. Fix: let some sentences just say the
thing, once, without the self-correction. Use a period instead of a dash more
often than feels natural.

**Constant hedging and qualification.** Words and constructions like *which*,
*the way*, *mostly*, *actually*, *in the tone of*, *the kind of X that Y* — 
each one is a reasonable, precise move on its own, but stacked in most
sentences it becomes its own signature, a prose style that's always circling
back to qualify itself. Fix: let some sentences be plain declaratives with no
qualifier at all.

**Aphorism density.** If nearly every paragraph contains one crafted,
quotable, insight-bearing line ("a slow leak keeps leaking whether or not
anyone's watching it"), that density is itself unusual — most sentences in
real prose are doing plain functional work (movement, information, transition)
without reaching for insight. Fix: let more sentences just move the scene
along and do nothing clever.

**Your own recurring construction.** Avoiding the generic AI hedge pattern
doesn't stop a specific phrase-level construction from becoming *your own*
tic across a piece, or across several. Concretely: "which wasn't a choice so
much as an absence of one," "which had nothing to do with," "not a choice so
much as" — three variants of the same recursive-qualification move, all in one
story, then recurring in the next. That's not the checklist working; it's a
new personal fingerprint replacing the generic one. Before finishing, scan for
any construction — not just hedge words generally, but a specific repeated
phrase shape — used more than once in a piece, or reused from something you
wrote before. If found, rewrite at least one instance into a plain, different
sentence shape.

## Second-order tells: what happens when you apply this skill too neatly

Following the checklist above item-by-item can produce a story that's still
identifiably AI — just at a level up. A too-clean pass through this skill has
its own signature:

**Symbolic over-determination.** Not stating the theme in a sentence isn't
enough if every element of the story quietly reinforces the same idea anyway —
the clock, the birthday cards, the funeral, the illness, the recurring day of
the week all rhyming with one motif. That's Thematic Unity (a core AI-elevated
feature in its own right, independent of whether the theme is ever spoken
aloud) — you've just moved the over-explanation from the sentence level to the
structural level. Fix: let at least one concrete detail in the story be
genuinely inert — present, specific, doing nothing symbolic.

**Reader address as a borrowed costume.** A line like "you, reading this" or
"she is aware that—" only earns its place when the entire narrative voice is
built around that mode — an epistolary story, a frame tale, an oral narrator
who's been talking to someone the whole time. Dropped into an otherwise
close-third narration as a single gesture, it reads as a recognizable
contemporary-literary-magazine tic rather than an organic choice — often more
identifiable as "AI doing literary voice" than silence would have been. If the
whole piece doesn't support it, cut it rather than force it in for the
checklist.

**Uniform polish and uniform restraint.** Real human prose — even published,
edited human prose — has texture: a paragraph that's flatter than its
neighbors, a metaphor that doesn't quite land, a shift in register the writer
didn't smooth over, sentences of wildly different quality sitting next to each
other. A story where every single paragraph hits the same careful, calibrated
note is its own tell, regardless of what that note is. Fix: let some passages
be plainer, rougher, or less crafted than others. Don't polish evenly.

**The elegant callback ending.** Resolving through an external event (per the
checklist) doesn't help if the ending is still constructed to rhyme precisely
with an early detail — that's tight causal/circular structure wearing a
different costume, and it's a move AI is specifically good at. Fix: consider
letting the ending introduce something the story hasn't set up, or end on a
detail that doesn't resolve anything, instead of a symmetrical echo.

The throughline: this skill's checklist is a set of individual moves to
consider, not a formula to satisfy completely and cleanly. A story that
checks every box in a controlled, tidy way has just built a new, subtler kind
of tidiness. Somewhere, on purpose, leave something unpolished, undecided, or
structurally loose.

## Self-audit checklist (run this before calling a draft finished)

Ask honestly, story in hand:

- [ ] Is there a sentence, anywhere, where the narrator or a character basically
      states "the point" of the story? If yes, cut or obscure it.
- [ ] Does every subplot serve the main theme? If yes, break one off.
- [ ] Could the protagonist's key choice be swapped for the opposite and still
      seem reasonable? If not, it's too morally clean — complicate it.
- [ ] Is the plot told start-to-finish in the order it happened? If yes, consider
      reordering at least one piece of it.
- [ ] Count emotion beats — how many are rendered as physical sensation
      (racing heart, tight throat) vs. plainly named vs. shown through action?
      If it's almost all physical sensation, vary it.
- [ ] Does the ending resolve mainly through the protagonist's own realization or
      choice? Consider whether something outside their control should matter more.
- [ ] Are any allusions or references vague ("an old song," "a famous painting")
      that could be made specific and named?
- [ ] Does the story ever acknowledge it has a reader, even once?
- [ ] Does every concrete detail in the story serve the theme? If yes, add
      something that's just there — specific, but symbolically inert.
- [ ] Is the prose evenly polished start to finish, with no rough or flatter
      patches? If yes, that uniformity is itself a tell — loosen a passage.
- [ ] Does the ending rhyme neatly with something from the opening? If it
      resolves *too* elegantly, consider ending on something unresolved instead.
- [ ] Count em-dash self-corrections ("X — actually, Y —"). If most paragraphs
      have one, that rhythm is a fingerprint on its own — cut some, let others
      stand as plain sentences instead.
- [ ] Count hedge words (*which*, *mostly*, *actually*, *the way*) per page. If
      nearly every sentence qualifies itself, flatten some into plain
      declaratives.
- [ ] Is there a quotable, crafted line in nearly every paragraph? If so, let
      more paragraphs be purely functional — moving the scene, not landing an
      insight.
- [ ] Scan for one specific phrase construction (not just hedge words in
      general) used more than once — in this piece or reused from a previous
      one. If found, rewrite one instance into a genuinely different shape.

If most boxes are already checked "no" (i.e., the story avoids the AI defaults),
it's in good shape. This isn't a rule to hit every box in every story — human
stories don't all do all of these — it's a check against defaulting to the AI
cluster on all of them at once, which is what actually gets flagged.

## Fingerprints by model — read this if you know who's holding the pen

Each AI model has its own additional tics beyond the shared ones above. If you
are one of these models (or emulating one), these are your specific defaults to
counteract — see `references/core-features-table.md` for the full breakdown, but
in short:

- **Claude**: flattens event escalation (things stay calm/even when they should
  build), is unusually reverent toward genre convention rather than subverting
  it, over-favors epilogues, avoids dream/vision sequences, and defaults to quiet
  endings. Counter-moves: let intensity spike unevenly, allow one convention to
  be broken on purpose, cut the epilogue, consider a dream/vision beat, allow a
  loud ending sometimes.
- **GPT**: over-relies on gossip/rumor as a plot mechanism and frames stories as
  looking back on events from years ago.
- **Gemini**: over-explains via external character description, produces
  unusually tidy endings and bleak/oppressive settings by default.
- **DeepSeek**: front-loads context that should be discovered gradually.
- **Kimi**: has the fewest distinguishing choices — sits at the generic center of
  AI-typical defaults; the general checklist above matters most here.

## Deeper reference

`references/core-features-table.md` has the full 30-feature table from the paper
(exact human vs. AI rates for every core feature, plus all per-model fingerprint
features) if finer-grained calibration is useful — e.g., auditing a finished
manuscript feature-by-feature rather than working from the summary above.
