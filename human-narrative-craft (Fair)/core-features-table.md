# Full core-feature reference (StoryScope, Russell et al., COLM 2026)

Source: "StoryScope: Investigating idiosyncrasies in AI fiction," Table 16 & 17.
Human vs. AI rates below are averaged across five AI models (Claude, GPT,
Gemini, DeepSeek, Kimi). "Gap" is Human − AI; a negative gap means AI does this
*more*; a positive gap means humans do this *more*.

Use this file when you want to audit a specific manuscript feature-by-feature,
not for casual drafting — for that, the checklist in SKILL.md is enough.

## AI-elevated: thematic over-determination (AI does these more)

| Feature | Human | AI | Gap |
|---|---|---|---|
| Thematic explicitness & moralizing (1–5 scale) | 3.28 | 3.94 | −0.65 |
| Moral/philosophical weighting (1–5 scale) | 3.26 | 3.68 | −0.42 |
| Thematic unity — subplots all serve the theme (1–5) | 4.41 | 4.74 | −0.33 |
| Narrator explicitly comments on theme | 52% | 77% | −25 |
| Dialogue used for philosophical debate | 34% | 59% | −25 |
| References are vague/implicit rather than named | 50% | 72% | −22 |

## AI-elevated: sensory & embodied over-performance

| Feature | Human | AI | Gap |
|---|---|---|---|
| Emotion conveyed via embodied metaphor (tight chest, etc.) | 38% | 81% | −42 |
| Setting used as psychological mirror (1–5) | 3.58 | 4.07 | −0.49 |
| Environmental/ecological emphasis (1–5) | 2.83 | 3.21 | −0.38 |
| Smell/olfactory imagery present | 57% | 82% | −26 |
| Sensory density overall (1–5) | 3.66 | 3.93 | −0.26 |
| Depth of interior access (1–5) | 3.67 | 3.93 | −0.26 |

## AI-elevated: structural streamlining

| Feature | Human | AI | Gap |
|---|---|---|---|
| Causal-chain continuity (1–5, higher = tighter single chain) | 3.92 | 4.20 | −0.28 |
| Spatial granularity (0–ordinal) | 2.27 | 2.53 | −0.26 |
| Resolution driven by protagonist's own choice | 46% | 69% | −23 |
| Character introduced via external description | 30% | 52% | −22 |
| No subplots at all | 57% | 79% | −22 |
| Resolution = internal understanding/acceptance | 27% | 47% | −21 |
| Opening spatial grounding (ordinal) | 2.12 | 2.33 | −0.20 |
| Pre-threat character investment (1–5) | 2.76 | 2.99 | −0.23 |

## Human-elevated: intertextual richness (humans do these more)

| Feature | Human | AI | Gap |
|---|---|---|---|
| Explicit named intertextual reference | 47% | 24% | +23 |
| Balanced mix of explicit + implicit references | 37% | 16% | +21 |

## Human-elevated: reader engagement

| Feature | Human | AI | Gap |
|---|---|---|---|
| Fourth-wall permeability (ordinal) | 0.67 | 0.39 | +0.28 |
| Direct reader address (ordinal) | 0.28 | 0.07 | +0.21 |

## Human-elevated: temporal complexity

| Feature | Human | AI | Gap |
|---|---|---|---|
| Depth of recontextualization after a reveal (1–5) | 3.28 | 2.95 | +0.34 |
| Chronological discontinuity (1–5) | 2.40 | 2.12 | +0.28 |
| Nonlinear framing to delay disclosure (1–5) | 1.96 | 1.68 | +0.28 |
| Anachrony intensity — flashback/flash-forward use (1–5) | 2.58 | 2.31 | +0.27 |

## Human-elevated: narrative diversity

| Feature | Human | AI | Gap |
|---|---|---|---|
| Location variety (ordinal) | 1.34 | 1.08 | +0.26 |
| Dialogue-to-narration proportion (1–5) | 2.95 | 2.70 | +0.24 |
| Subplot thematically parallel but distinct (not identical) | 42% | 21% | +22 |
| Protagonist's moral position is ambivalent/mixed | 59% | 38% | +21 |
| Emotion conveyed via explicit naming ("she felt afraid") | 29% | 8% | +21 |

---

## Per-model fingerprints (six-way attribution, top features per source)

These are what let a classifier guess *which* model wrote a story, beyond the
general human/AI split above.

**Human** — introduces characters via dialogue, single tight focalization,
narrator rarely addresses reader directly, back-loaded revelation pacing,
crossover/literary genre ambition, plus ~27 more (subplot density, naming
conventions, twist placement, atmospheric technique).

**Claude** — strong, distinctive *flatness* in event escalation (the single
strongest fingerprint feature of any model); high event-type diversity; favors
epilogue/flash-forward endings; avoids dreams/visions as a temporal device;
leans toward uncanny/haunted setting moods; reverent/continuist toward genre
convention (62% of Claude stories extend tradition rather than subvert it, vs.
39–56% for other sources).

**GPT** — gossip/rumor as a salient plot mechanism (64% vs. 44–55% elsewhere);
narrator often speaks from a distant retrospective vantage (looking back years
or decades); subverts reader expectations more than other AI (41% vs. 27–36%);
resolutions/reconciliations left partial or ambiguous; no strong iterative/
habitual narration.

**Gemini** — protagonist's social circle tends to expand over the story; heavy
use of direct speech over indirect; favors siege/ordeal-type plot schemas;
characters given full personal names; frequent flashback use; tidiest endings
and most extended denouements of any source; bleakest/most oppressive settings
(88% tagged bleak).

**DeepSeek** — high narrator visibility/presence; emotion conveyed mainly
through behavioral cues rather than embodiment or naming; leans plot-forward
over atmosphere; backstory evenly interleaved rather than front- or back-loaded;
uses embedded storytelling-within-the-story scenes.

**Kimi** — fewest distinguishing fingerprints of any source (lowest six-way F1);
tends to introduce characters via an in-action event, opens in medias res, and
avoids explicit trait-labeling — otherwise sits at the generic center of the
AI-typical distribution, meaning the general checklist matters more here than
model-specific tics.