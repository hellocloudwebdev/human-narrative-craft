# StoryScope Core Narrative Features — Reference

## v4 craft-layer note

The companion skill now contains two additional non-StoryScope craft audits: **Surface Pressure** and **Lived-In Specificity**. They are intentionally separated from the 30 empirical core features. Surface Pressure addresses over-polished, over-quotable, self-explanatory prose. Lived-In Specificity addresses operational detail, idiosyncratic texture, subtext, imperfect interpersonal dynamics, and incidental-detail bandwidth. Neither layer is a research-backed authorship detector; both exist to improve narrative naturalness without corrupting the StoryScope structural audit.


Source: *StoryScope: Investigating idiosyncrasies in AI fiction*, Russell et al., COLM 2026 / arXiv:2604.03136v6.

The paper's 30 core features are the most compact research-backed diagnostic set used in the skill. They should be treated as **probabilistic tendencies**, not hard rules for what human writing must look like.

## AI-elevated feature set

| Feature | Human | AI | Gap (H-AI) | Practical implication |
|---|---:|---:|---:|---|
| Thematic Explicitness & Moralizing | 3.28 | 3.94 | -0.65 | Trust scenes to carry meaning; reduce explicit moralizing. |
| Moral / Philosophical Weighting | 3.26 | 3.68 | -0.42 | Do not turn every conflict into a thesis discussion. |
| Thematic Unity | 4.41 | 4.74 | -0.33 | Allow secondary material to complicate or sit beside the theme. |
| Narratorial Thematic Commentary: yes | 52% | 77% | -25 pp | Avoid narrator-explained takeaways when unnecessary. |
| Dialogue Function: philosophical debate | 34% | 59% | -25 pp | Give dialogue social, strategic, relational, and plot functions. |
| Reference Explicitness: implicit echoes | 50% | 72% | -22 pp | Use specific named references when naturally relevant. |
| Emotional Expression: embodied | 38% | 81% | -42 pp | Vary emotion expression; do not default to bodily metaphors. |
| Setting as Psychological Mirror | 3.58 | 4.07 | -0.49 | Do not make every setting reflect a character's mood. |
| Environmental & Ecological Emphasis | 2.83 | 3.21 | -0.38 | Avoid decorative environmental emphasis when it has no narrative function. |
| Sensory Modalities: olfactory | 57% | 82% | -26 pp | Avoid overusing smell as a shortcut to vividness. |
| Sensory Density | 3.66 | 3.93 | -0.26 | Use sensory detail selectively. |
| Depth of Interior Access | 3.67 | 3.93 | -0.26 | Do not narrate every interior state. |
| Continuity of Main Causal Chain | 3.92 | 4.20 | -0.28 | Permit meaningful side effects, delays, interruptions, and indirect causation. |
| Spatial Granularity | 2.27 | 2.53 | -0.26 | Vary environmental granularity according to scene purpose. |
| Agency in Resolution: protagonist choice | 46% | 69% | -23 pp | Allow mixed/external agency where appropriate. |
| Character Introduction: external description | 30% | 52% | -22 pp | Introduce characters through behavior, action, dialogue, or relation when fitting. |
| Subplot Integration: no subplots | 57% | 79% | -22 pp | Consider meaningful parallel/contrasting subplots. |
| Resolution Mode: internal understanding | 27% | 47% | -21 pp | Do not default to acceptance/insight as closure. |
| Opening Spatial Grounding | 2.12 | 2.33 | -0.20 | Avoid obligatory polished scene-grounding before action. |
| Pre-Threat Character Investment | 2.76 | 2.99 | -0.23 | Avoid over-investing in neat setup before meaningful threat or pressure. |

## Human-elevated feature set

| Feature | Human | AI | Gap (H-AI) | Practical implication |
|---|---:|---:|---:|---|
| Intertextual Strategy: explicit named reference | 47% | 24% | +23 pp | Concrete cultural/textual references can increase specificity when authentic. |
| Frequency of Direct Reader Address | 0.28 | 0.07 | +0.21 | Reader address is useful when supported by the narrative voice; do not force it. |
| Reference Explicitness: balanced mix | 37% | 16% | +21 pp | Mix named and diffuse references rather than making allusion uniformly vague. |
| Fourth-Wall Permeability | 0.67 | 0.39 | +0.28 | Allow narrator/audience permeability where genre and voice permit it. |
| Depth of Recontextualization After Surprise | 3.28 | 2.95 | +0.34 | Make important revelations change how earlier scenes are understood. |
| Chronological Discontinuity | 2.40 | 2.12 | +0.28 | Use time jumps when they control disclosure. |
| Nonlinear Framing for Delayed Disclosure | 1.96 | 1.68 | +0.28 | Consider withholding chronology to delay or deepen understanding. |
| Anachrony Intensity | 2.58 | 2.31 | +0.27 | Use flashbacks/flash-forwards with narrative purpose. |
| Location Variety Scope | 1.34 | 1.08 | +0.26 | Allow more than one meaningful physical world when story logic supports it. |
| Dialogue-to-Narration Proportion | 2.95 | 2.70 | +0.24 | Let dialogue occupy a natural share of the narrative rather than narrating everything. |
| Subplot Integration: thematically parallel | 42% | 21% | +22 pp | Parallel subplots can enrich or complicate the central concern. |
| Moral Polarity: ambivalent/mixed | 59% | 38% | +21 pp | Resist automatic moral simplification. |
| Emotional Expression: explicit labels | 29% | 8% | +21 pp | It is not inherently less human to name an emotion directly; vary modes. |

## Interpretation

StoryScope's 30 features cluster into recurring structural tendencies:

1. **Thematic over-determination:** AI more often explains its theme, moral, and philosophical stakes explicitly and keeps narrative material tightly unified around them.
2. **Sensory/embodied performativity:** AI more often expresses emotion through bodily sensations, uses smell, and mirrors psychology in setting.
3. **Structural streamlining:** AI more often uses a continuous causal chain, protagonist-controlled resolution, external character introduction, few subplots, and internal-understanding closure.
4. **Intertextual richness:** Human stories more often use explicit named references and a balanced mix of explicit and diffuse intertextuality.
5. **Reader engagement:** Human stories more often cross the narrator/reader boundary and directly address the reader.
6. **Temporal complexity:** Human stories more often use discontinuity, delayed disclosure, flashbacks, and recontextualizing surprises.
7. **Narrative diversity:** Human stories use more varied locations, dialogue share, subplot relationships, moral polarity, and emotional labeling.

## Important empirical cautions

- The study does not say that every human story has every human-elevated trait.
- Human and AI distributions overlap substantially.
- The human stories were more dispersed in narrative-feature space, with mean rarity percentile 0.71 vs. 0.49 for AI; 24.7% of human test stories vs. 7.1% of AI fell in the top 10% rarest region.
- The signal is distributed across correlated dimensions. In dimension-level ablations, no single NarraBench dimension was sufficient and no single dimension was individually necessary.
- Narrative-only detection was 93.2% macro-F1; Core Only (30 features) was 84.8%; Core+Fingerprint (101 features) was 91.1%. This demonstrates that the 30-feature set is useful but is not a complete model of human writing.
- After surface-level artifact editing, narrative detection remained high (93.9% macro-F1), reinforcing that prose-level cleanup alone does not substantially change the structural profile measured by the paper.

## Fingerprints observed in the benchmark

These are **not** targets to imitate. They are source-specific observations demonstrating that individual LLMs can develop recurring narrative quirks:

- Human: in-dialogue character introduction, single focal breadth patterns, no direct narrator address in one fingerprint, back-loaded revelation, crossover-genre ambition, plus additional source-specific features.
- Claude: flatter event escalation, greater event-type restraint/diversity pattern, epilogue/flash-forward endings, fewer dream/vision distortions, uncanny/haunted settings.
- GPT: gossip/rumor as a plot mechanism, distant retrospective narration, expectation subversion, iterative/habitual narration, partial/ambiguous reconciliation.
- Gemini: expanding protagonist social trajectory, more direct speech balance, siege/ordeal schema, named personal characters, frequent flashbacks.
- DeepSeek: narrator visibility, behavioral emotional expression, plot-vs-atmosphere orientation, evenly interleaved backstory, embedded storytelling.
- Kimi: in-action character introductions, in-medias-res entry, less explicit trait labeling.

The skill therefore should not simply "write less like GPT" or "write like Claude." The stronger objective is to move away from the shared AI cluster and toward a broader, story-specific decision profile.
