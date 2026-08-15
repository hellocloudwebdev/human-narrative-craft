# StoryScope-Informed Human Craft Fair v4

## Purpose

Use this skill to improve human-like narrative construction by changing the **underlying narrative decisions** that StoryScope found systematically different between human and AI fiction.

This is **not** a "make the prose sound human" filter and it is not an AI-detector evasion recipe. It is a **story-construction and structural-revision skill**. It operates before drafting, during drafting, and after drafting.

The target is:

> **A particular, coherent story produced from a broader and less default set of narrative decisions.**

Do not optimize for maximum weirdness, maximum ambiguity, maximum nonlinear structure, or a target classifier score. Human stories in the study were more dispersed in narrative space, not uniformly defined by a fixed checklist.

## Research basis

This skill is derived from *StoryScope: Investigating idiosyncrasies in AI fiction* by Jenna Russell, Rishanth Rajendhran, Chau Minh Pham, Mohit Iyyer, and John Wieting (COLM 2026; arXiv:2604.03136v6).

The paper compared human stories with five LLM sources across 10 narrative dimensions and 304 discourse-level features. Narrative features alone achieved 93.2% macro-F1 for human-vs-AI classification. A compact set of 30 core features captured much of the separation. Human stories were more dispersed/rarer in the observed narrative space, while AI stories clustered more tightly. Surface-level editing had little effect on the narrative signal.

### Central research lesson

**The tell is not primarily the sentence. The tell is the pattern of decisions underneath the sentence.**

StoryScope explicitly distinguishes non-style features such as events, causality, closure, character roles, relationship topology, setting, and temporal arrangement from prose-level style. Its controlled-template experiment also found that comparing raw text tends to produce style-heavy features, while structured templates surface structure-heavy features such as emotional arcs, relationship trajectories, event density, and flashback usage.

## Non-negotiable operating principles

### Principle 1 — Separate prose quality from narrative evidence

Polished prose is not evidence of AI authorship.

Do **not** infer authorship from:

- literary polish;
- balanced sentence rhythm;
- precise sensory detail;
- tidy thematic callbacks;
- elegant endings;
- absence of awkward phrasing;
- generic "literary magazine" feel;
- lack of an online/publication footprint.

Those may be observations about the prose or provenance, but they are not StoryScope narrative evidence.

When evaluating a story, first remove wording from consideration mentally. Ask what the story **does**, not whether its sentences "feel AI."

### Principle 2 — Audit clusters, not isolated features

A single human-leaning or AI-leaning feature proves almost nothing.

Look for **co-occurring decisions**. For example:

> highly explicit theme + continuous causal chain + protagonist-controlled resolution + no meaningful subplot + internal-understanding closure

is much more informative than any one of those features alone.

Likewise:

> recontextualizing revelation + meaningful temporal displacement + mixed moral polarity + parallel subplot + non-single-track causality

forms a substantially different narrative profile.

### Principle 3 — Do not turn the paper into a formula

Never interpret:

> "human stories had more X"

as:

> "add X to every story."

That creates a new AI-like optimization loop.

Use the research as a **diagnostic prior**, then choose story-specific decisions.

### Principle 4 — Structural changes outrank surface changes

When a draft shows an AI-leaning cluster, revise in this order:

1. narrative information structure;
2. causality and agency;
3. revelation timing;
4. temporal arrangement;
5. social/relationship structure;
6. subplot structure;
7. moral framing and ending mode;
8. emotional representation;
9. setting/intertextual decisions;
10. sentence-level polish.

Do not spend ten edits replacing phrases while keeping the same narrative architecture.


### Principle 5 — Structural human-likeness and surface naturalness are separate passes

A story can have a varied, non-default narrative architecture and still feel **over-optimized at the sentence and paragraph level**. Treat this as a secondary craft problem, not as evidence that the story was AI-generated.

Secondary surface-pressure signals include:

- unusually high density of quotable or aphoristic sentences;
- repeated elegant metaphors that all point toward the same theme;
- characters articulating their own motives or the story's meaning with suspicious precision;
- secondary characters functioning mainly as instruments for the protagonist's emotional development;
- every introduced object, image, line, or detail receiving a clean payoff;
- nearly every paragraph having an obvious rhetorical job;
- very little mundane, practical, socially awkward, mildly inconvenient, or incidental material;
- opening and ending symmetry that feels engineered rather than earned;
- recurring punctuation or cadence patterns that make every passage equally polished.

These are **surface-pressure heuristics derived from external writing evaluation, not findings from StoryScope**. They must never override the story's narrative logic or be converted into an authorship probability.

### Principle 6 — Naturalness is variation in salience, not deliberate imperfection

Do not make prose human by adding mistakes, filler, randomness, incoherence, fake awkwardness, or arbitrary mess. Instead, vary the **importance and finish level of details** in ways that fit the story.

A believable narrative may contain:

- a detail that establishes atmosphere and never returns;
- a practical exchange that is only partly relevant;
- a character who misunderstands something;
- an observation that is ordinary rather than quotable;
- a conversation whose purpose is social rather than thematic;
- an ending that is resonant without perfectly mirroring the opening;
- a character thought that is incomplete, contradictory, or simply wrong.

The goal is not to lower craft quality. The goal is to stop every local unit of prose from behaving as though it was selected to maximize literary significance.

---

# StoryScope construction model

Represent the story internally as a structured narrative map before writing polished prose.

Use these fields:

```text
agents
social_network
major_relationship_trajectories
events
causal_links
plot_arc
subplots
locations
setting_function
time_span
chronology
information_state
withheld_information
revelations
recontextualization
perspective
focalization
dialogue_functions
emotional_expression_modes
thematic_explicitness
moral_polarity
resolution_agency
resolution_mode
intertextual_context
reader_relationship
```

For each major scene, maintain:

```text
scene
focal_agent
location
time
what_reader_knows
what_focal_character_knows
what_other_characters_know
immediate_objective
conflict
change
consequence
```

A scene may change knowledge, relationship, leverage, desire, interpretation, or material circumstances. It does **not** have to move the main causal chain directly.

---

# The three-layer workflow

## Layer A — Architect: choose the narrative decisions

Before prose, answer internally:

1. What is the obvious, tidy version of this story?
2. What would the most generic competent model probably do next?
3. Which narrative decision will make this particular story more specific rather than merely more unusual?
4. Who knows what, and when?
5. Which event will be understood differently later?
6. Which character has a motive that cannot be reduced to one clean objective?
7. Which relationship has its own trajectory?
8. Which event is consequential even though it is not a clean step in the protagonist's plan?
9. Why is the story being told in this temporal order?
10. What does the ending leave unresolved, and why should that residue remain?

Do not force a deviation merely to escape a default. A deviation needs a story-specific reason.

## Layer B — Narrator: draft from decisions, not from "human style"

Draft with these constraints:

- scenes should reveal behavior rather than repeatedly explain meaning;
- characters may misread their own motives;
- dialogue should have social, strategic, relational, practical, comic, deceptive, or plot functions in addition to philosophical functions;
- emotion can be named, implied, enacted, contradicted, avoided, misremembered, or embodied;
- setting may mirror psychology sometimes, but may also remain neutral, inconvenient, socially significant, comic, ugly, or indifferent;
- specific cultural details should emerge when grounded in the story-world, not because a checklist asks for them;
- chronology should serve disclosure rather than decorate the prose;
- a revelation should sometimes change the meaning of what came before;
- secondary characters should have trajectories, not merely utility;
- the ending should be a consequence of the story's actual forces, not an automatic "lesson learned" beat.

## Layer C — StoryScope Auditor: inspect structure while ignoring prose

After drafting, mentally convert the story into structured representation and ask the following.

### Audit A — Thematic over-determination

Check:

- Is the theme repeatedly stated after being demonstrated?
- Does the narrator explain the lesson?
- Do nearly all objects, subplots, dialogue exchanges, and images point to the same conclusion?
- Does the final scene tell the reader exactly how to interpret the preceding story?

Correct by removing unnecessary explanation or introducing a genuine counter-pressure—not by making the story artificially obscure.

### Audit B — Causal streamlining

Check:

- Is there one unusually clean causal chain from inciting incident to ending?
- Does every important event efficiently serve the main plot?
- Are there no meaningful side consequences, interruptions, institutional constraints, accidental effects, or social causes?

Correct by introducing causally meaningful complexity, not random confusion.

### Audit C — Resolution agency

Ask:

> Who actually causes the ending?

Classify the ending as:

```text
protagonist choice
other-character choice
mixed agency
external event/institution
accident
consequence of earlier action
unresolved
```

Do not alter this simply to make it "human." Alter it only if the existing resolution is too mechanically protagonist-controlled or psychologically tidy for the story.

### Audit D — Revelation and recontextualization

For every major revelation:

1. What does the reader learn?
2. What did the reader previously believe?
3. Which earlier scene changes meaning after the revelation?
4. Does the revelation change character interpretation, not just plot information?

A revelation that changes nothing earlier is often only a twist/fact. A stronger revelation reorganizes the narrative model in the reader's mind.

### Audit E — Temporal structure

Classify the story:

```text
linear
nonlinear
mixed
framed recollection
nested/embedded chronology
```

Then ask:

> Why is this order better than chronological order—or why is chronological order essential?

Do not add flashbacks merely to satisfy the research. Time shifts are valuable when they control disclosure, create contrast, or cause reinterpretation.

### Audit F — Social/network structure

Map:

```text
major characters
supporting characters
alliances
conflicts
dependencies
relationship changes
community/institutional forces
```

Check whether the protagonist is isolated inside a one-to-one story when the premise naturally supports a wider social network.

Do not add characters merely for density.

### Audit G — Subplots

Classify each secondary thread:

```text
none
parallel
contrasting
independent
```

A meaningful subplot should alter pressure, character interpretation, social stakes, or thematic framing. A decorative subplot added only to tick a box is forbidden.

### Audit H — Moral polarity

For consequential choices, ask:

- Why is the protagonist's action defensible?
- Why is it troubling?
- Who benefits?
- Who bears the cost?
- What does the protagonist misunderstand?
- Would another reasonable character judge the action differently?

Do not force every protagonist into moral ambiguity. Preserve ambivalence when it naturally follows from the story.

### Audit I — Emotional expression

Track how emotion is represented:

```text
explicit label
behavioral cue
social performance
silence/avoidance
contradictory action
memory
body/sensation
setting
mixed
```

Flag drafts where embodied sensation is the dominant mechanism for nearly every emotion.

The correction is **mode diversity**, not a ban on physical sensation.

### Audit J — Intertextual and external-world engagement

Ask whether the story naturally has:

- a named work;
- named author;
- named place;
- historical reference;
- institution;
- brand/object;
- cultural tradition;
- genre conversation;
- narrator-reader relationship.

Use such material only when supported by the story. Never invent references merely to imitate a statistical tendency.

### Audit K — Narrative diversity / defaultness

Perform the most important question:

> **Does this story appear to have been generated by repeatedly selecting the safest competent answer at each narrative decision point?**

Compare the current story against the obvious default version of itself.

Inspect variation in:

- narrative entry point;
- character entrances;
- social topology;
- event types;
- causal continuity;
- revelation pacing;
- location variety;
- chronology;
- dialogue role;
- subplot topology;
- moral framing;
- emotional-expression mode;
- resolution mode.

Do not seek maximal difference. Seek **particularity**.

---

# Layer D — Surface Pressure / Human Texture Auditor

Run this **after** the StoryScope structural audit. Do not use it to override a sound narrative architecture.

## Audit L — Quotable-line density

Ask:

- Does nearly every paragraph contain an aphorism, striking metaphor, compressed insight, or memorable closer?
- Are ordinary transitions conspicuously absent?

Revision rule:

Flatten selected passages into direct, functional prose when that improves pacing or character realism. Keep genuinely strong lines when the scene earns them. Do not make every paragraph equally quotable.

## Audit M — Metaphor concentration and thematic symmetry

Map repeated metaphor families and symbolic echoes.

Check:

- Does one conceptual metaphor appear in too many forms?
- Are objects repeatedly converted into symbols?
- Does the ending restate the opening through the same image because symmetry is expected rather than because the story demands it?

Revision rule:

Keep the strongest recurrence. Allow some details to remain literal, ambient, or unresolved.

## Audit N — Character self-explanation

Flag moments where a character suddenly understands their own psychology exactly when the reader needs an explanation.

Replace some instances with:

- partial knowledge;
- contradiction between thought and action;
- mistaken self-diagnosis;
- dialogue shaped by social pressure;
- avoidance or silence;
- behavior that the reader must interpret.

Do not make characters artificially stupid or opaque.

## Audit O — Character utility

For each important secondary character, inspect whether they have at least one element that is not reducible to protagonist support:

```text
desire
constraint
habit/idiosyncrasy
relationship agenda
independent action
contradiction
consequence
```

A character may remain minor. The point is to prevent every person from functioning as a perfectly aligned emotional tool.

## Audit P — Aphorism / dialogue pressure

Flag dialogue that:

- states the theme in polished form;
- contains a lesson with unusually exact phrasing;
- sounds as if it was written to be quoted rather than spoken.

Ask whether the character would naturally say it in that social situation. Prefer concrete requests, interruptions, practical concerns, jokes, evasions, misunderstandings, and ordinary wording when appropriate.

## Audit Q — Detail payoff completeness

Classify notable details as:

```text
plot-bearing
character-bearing
world-bearing
atmospheric
incidental
setup
```

Do not make all incidental details become setup. Do not remove useful details merely because they never return. A selective payoff pattern often feels more natural than total closure.

## Audit R — Mundane bandwidth

Check whether the draft allows enough room for:

- logistics;
- routine actions;
- small misunderstandings;
- ordinary social talk;
- inconvenient interruptions;
- moments with no immediate thematic statement.

These elements must earn their place through realism, pacing, characterization, or contrast. They are not filler and should not be inserted just to lower perceived polish.

## Audit S — Sentence and punctuation regularity

Inspect repeated sentence shapes, paragraph lengths, and punctuation patterns.

Em dashes are **not forbidden** and are not, by themselves, an AI signal. The question is whether the prose has become rhythmically over-regular. Vary sentence length and connective structure only when natural cadence improves.

## Audit T — Ending calibration

Check whether the ending is:

```text
perfectly symmetrical
strongly resonant but earned
quiet/plain
ambiguous
open-ended
```

Keep the ending form that follows from the story. Never weaken an ending merely to avoid a neat callback.

---

## Layer E — Lived-In Specificity Auditor

Run this after the structural audit and alongside, but separately from, the Surface Pressure Auditor. This layer incorporates a recurring observation from external literary evaluations: stories often feel more lived-in when details are **specific, operational, socially situated, and not all equally symbolic**.

This is **not a StoryScope feature set** and must not be used as proof of human authorship. Treat it as a craft diagnostic for avoiding over-abstract, over-curated fiction.

### Audit U — Operational specificity

Check whether domain-specific or professional details behave as if someone understands the activity from the inside.

Look for: 

- procedures and tools used for a reason;
- realistic constraints and tradeoffs;
- small practical distinctions that affect what a character can do;
- terminology used consistently without turning exposition into a glossary;
- consequences of mistakes, shortcuts, or habits.

Do not manufacture technical jargon. One accurate operational detail is better than five decorative ones.

### Audit V — Idiosyncratic detail

Check whether some details feel oddly specific because they belong to this character, place, job, family, or situation rather than because they are generically evocative.

Prefer details that reveal:

- habit;
- local knowledge;
- family shorthand;
- material wear;
- institutional routine;
- personal annoyance;
- imperfect memory;
- a specific object used in an unremarkable way.

Do not make every detail unusual. The goal is **particularity**, not eccentricity.

### Audit W — Subtext and indirectness

Check whether every important emotional conflict is verbalized.

Where appropriate, let information travel through:

- what a character asks instead of what they mean;
- what they refuse to answer;
- a practical complaint standing in for an emotional one;
- repeated stories or habits;
- social politeness that conflicts with private intent;
- an action that contradicts a spoken claim;
- a detail recalled for a reason the speaker does not admit.

Do not make every exchange mysterious. Some people say exactly what they mean.

### Audit X — Imperfect interpersonal dynamics

Check whether relationships contain friction that is not perfectly aligned with the plot.

Secondary characters may be:

- mildly annoying;
- needy at the wrong time;
- funny without serving the theme;
- wrong about something;
- distracted by their own concern;
- generous for mixed reasons;
- inconsistent in believable ways.

The purpose is to give relationships their own momentum, not to inject arbitrary conflict.

### Audit Y — Incidental-detail bandwidth

Ask whether the draft contains a healthy mixture of:

```text
plot-bearing
character-bearing
world-bearing
atmospheric
incidental
setup
misdirection
```

Not every memorable object should become a clue. Not every introduced fact should pay off later. Not every observed detail should reinforce the central theme.

### Audit Z — Narrative texture versus curated significance

Ask:

> Does the story feel as though someone discovered meaningful things while living through events, or as though every detail was selected in advance because it would contribute to the story's eventual significance?

If the second dominates, revise selectively by allowing:

- ordinary transitions;
- partial observations;
- non-symbolic objects;
- practical talk;
- incomplete recollections;
- small dead ends;
- social moments whose meaning is deferred or never made explicit.

Do not add filler. The test is whether the distribution of significance feels natural.

### Calibration rule

Do **not** intentionally add mistakes, awkwardness, randomness, jargon, irrelevant details, or unresolved threads to imitate a human. Human-feeling texture comes from **specificity + constraint + imperfect knowledge + independent relationships + uneven salience**, not from deliberate degradation.

# Two-score internal quality control

Do not output an "AI probability" score. Internally maintain two separate assessments:

### A. StoryScope Structural Profile

Rate each major structural cluster qualitatively:

```text
Low / Medium / High AI-leaning concentration
Low / Medium / High human-leaning counterpressure
```

The purpose is to detect **co-occurring default decisions**, not to label authorship.

### B. Surface Pressure Profile

Rate the following independently:

```text
quotable-line density
metaphor/symmetry density
self-explanation density
character-instrumentality
detail-payoff completeness
mundane bandwidth
sentence/punctuation regularity
ending calibration
```

Use this only to improve prose naturalness. Never treat it as a detector score.

### C. Lived-In Specificity Profile

Rate independently:

```text
operational specificity
idiosyncratic detail
subtext/indirectness
imperfect interpersonal dynamics
incidental-detail bandwidth
curated-significance pressure
```

Use this only to improve particularity and realism. It is not a detector score and must never be translated into an authorship probability.

### Revision order

1. StoryScope structural profile
2. information and revelation structure
3. character and social-network independence
4. subplot/counter-pressure
5. agency and ending
6. surface-pressure profile
7. sentence-level polish and proofreading

If a surface edit conflicts with narrative logic, preserve the narrative logic.

---

# The critical anti-error rule: never confuse "polished" with "AI"

External evaluators often produce weak reasoning such as:

> "The prose is very polished, therefore AI."

or:

> "The ending is perfectly symmetrical, therefore AI."

or:

> "The details are unusually curated, therefore AI."

Treat these as **surface observations**, not authorship conclusions.

Likewise:

> "There is no online footprint, therefore AI"

is a provenance claim and is outside the StoryScope narrative evidence entirely.

When presented with an external AI-assessment, translate its claims into two buckets:

### Surface bucket

Examples:

- diction;
- sentence rhythm;
- polish;
- cliché density;
- punctuation;
- sensory wording;
- tone;
- web footprint.

Do not use this bucket as primary evidence for StoryScope-style authorship reasoning.

### Lived-in-text bucket

Examples:

- domain-specific procedural texture;
- idiosyncratic objects or habits;
- indirect interpersonal conflict;
- mundane or incidental detail;
- imperfect recollection;
- socially independent secondary characters;
- details whose significance is delayed or absent.

Use this bucket for craft revision only. It is not StoryScope evidence of human authorship.

### Narrative bucket

Examples:

- causal continuity;
- agency;
- subplot topology;
- chronology;
- revelation/recontextualization;
- moral polarity;
- social network;
- character-introduction mechanism;
- dialogue function;
- thematic explicitness;
- resolution mode;
- narrative diversity.

Only this bucket should drive the StoryScope structural audit.

---

# The 30 core features: use as a diagnostic, never as a target vector

## AI-elevated tendencies

- Thematic Explicitness & Moralizing
- Moral / Philosophical Weighting
- Thematic Unity
- Narratorial Thematic Commentary
- Dialogue Function: philosophical debate
- Reference Explicitness: implicit echoes
- Emotional Expression: embodied
- Setting as Psychological Mirror
- Environmental & Ecological Emphasis
- Dominant Sensory Modalities: olfactory
- Sensory Density
- Depth of Interior Access
- Continuity of Main Causal Chain
- Spatial Granularity
- Agency in Resolution: protagonist choice
- Character Introduction: external description
- Subplot Integration: no subplots
- Resolution Mode: internal understanding
- Opening Spatial Grounding
- Pre-Threat Character Investment

## Human-elevated tendencies

- Intertextual Strategy: explicit named reference
- Frequency of Direct Reader Address
- Reference Explicitness: balanced mix
- Fourth-Wall Permeability
- Depth of Recontextualization After Surprise
- Chronological Discontinuity
- Nonlinear Framing for Delayed Disclosure
- Anachrony Intensity
- Location Variety Scope
- Dialogue-to-Narration Proportion
- Subplot Integration: thematically parallel
- Moral Polarity: ambivalent/mixed
- Emotional Expression: explicit labels

The full research table with observed human/AI means is in `references/core-features-table.md`.

### Important calibration

The 30 features are not independent buttons.

Do not set all human-elevated variables high.
Do not set all AI-elevated variables low.
Do not attempt to reproduce the reported mean vector.
Do not treat the human mean as an ideal authoring target.

The paper found that:

- human and AI distributions overlap;
- the human region is more dispersed;
- no single NarraBench dimension is sufficient;
- no single dimension is individually necessary;
- rarity is a population-level pattern, not proof of individual authorship;
- the 30-feature core is useful but incomplete.

Therefore the correct operational goal is:

> **Avoid repeated convergence on the same AI-like cluster while preserving coherence, genre fit, and story-specific necessity.**

---

# Structural revision protocol

When a draft is flagged as too default, revise the smallest number of **high-leverage decisions** first.

Recommended order:

1. Remove redundant thematic explanation.
2. Recheck causal chain continuity.
3. Reassign some causal agency if the protagonist automatically controls everything.
4. Introduce a meaningful second pressure line if the story is truly single-track.
5. Rework one major revelation so it recontextualizes earlier material.
6. Reconsider chronology around information disclosure.
7. Complicate one moral judgment where the narrative currently closes it prematurely.
8. Diversify emotional-expression modes.
9. Vary character entrances or dialogue functions.
10. Add concrete outside-world/intertextual material only when organically supported.
11. Recheck the ending for automatic self-understanding or tidy acceptance.
12. Only then polish sentences.

After each structural revision, ask:

> **Did this make the story more particular, or merely more complicated?**

If merely more complicated, undo it.

---

# Hard anti-patterns

Reject a revision if it:

- changes only vocabulary, punctuation, or sentence rhythm;
- replaces "AI words" while preserving the same plot architecture;
- inserts random flashbacks;
- adds arbitrary ambiguity;
- makes every character morally gray;
- adds fake named references;
- inserts "dear reader" for statistical effect;
- adds irrelevant locations;
- creates meaningless side characters;
- intentionally breaks causality to look human;
- adds sensory grit to every scene;
- swaps explicit emotion labels for body metaphors everywhere;
- turns every conversation into subtext;
- deliberately makes the ending less satisfying merely to avoid symmetry;
- explains a theme that the story has already demonstrated without a dramatic reason;
- maximizes a feature because the paper reported that humans had a higher mean.

---

# External-evaluator response protocol

When another model or detector claims that a story is AI-written:

1. Extract its actual evidence.
2. Label each claim **surface**, **provenance**, or **narrative**.
3. Discard surface/provenance claims as primary StoryScope evidence.
4. Translate narrative claims into the corresponding StoryScope dimensions.
5. If the evaluator mentions "too polished," "too quote-worthy," "too perfect," or "too literary," route those claims to the separate Surface Pressure Auditor rather than the StoryScope classifier logic.
6. Check whether multiple correlated AI-leaning decisions actually co-occur.
7. Check for human-leaning structural counterevidence.
8. Report uncertainty; never convert one structural pattern into certainty about authorship.

Do not produce numeric authorship probabilities merely because another model supplied one. StoryScope supports discrimination at a population level, not proof from an individual prose impression.

---

# Optional multi-pass mode

## Pass 1 — Architect

Build the structured narrative map and identify the default path.

## Pass 2 — Divergence

Choose a small number of story-specific structural deviations with clear reasons.

## Pass 3 — Narrator

Draft while preserving information asymmetries, character motives, chronology, and social pressure.

## Pass 4 — StoryScope Auditor

Ignore wording. Score clusters of narrative decisions.

## Pass 5 — Structural Revision

Change only high-leverage structural decisions that genuinely improve the story.

## Pass 6 — Surface Polish

Only now refine sentence rhythm, diction, imagery, transitions, grammar, and consistency.

---

# Final instruction

Write as though every narrative choice is a consequence of **this story, these characters, this social world, this information state, and this narrator**.

Do not write as though you are trying to satisfy a list of traits called "human."

When the obvious choice is neat, explicit, linear, protagonist-controlled, perfectly thematic, psychologically explained, and symmetrically resolved, inspect it.

Sometimes the obvious choice is correct. Keep it when the story requires it.

When the obvious choice is merely the safest default, choose a more particular alternative with a reason.

The objective is not to manufacture human-looking noise.

> **The objective is to produce a coherent story whose underlying decisions do not repeatedly collapse into the same narrow narrative template.**

## Version 3 change note

Version 3 adds a secondary surface-naturalness layer derived from external evaluator feedback. This layer is deliberately separated from the StoryScope evidence base: its job is to reduce **over-optimization of prose**, not to infer authorship or evade detection.

## Source note

All empirical claims in this skill are derived from the attached StoryScope paper. The research summary and exact core-feature comparisons are in `references/core-features-table.md`.
