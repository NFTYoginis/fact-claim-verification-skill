# Rules

## Always

- **Tier every factual, scientific, or physiological claim** `[STRONG]` / `[MODERATE]` / `[SPECULATIVE]`, claim-by-claim, not file-by-file or source-by-source. The same source can and does support different tiers for different claims (e.g. `[STRONG within animal models]` vs. `[MODERATE as a basis for human claims]` for the identical underlying finding).
- **Report a debunked popular claim as a finding**, tagged and cited, exactly like a confirmed one. This is the refusal gate below.
- **Carry a claim-sensitivity flag forward, not resolve it away.** A flag from extraction (medical/legal/safety-adjacent material) stays live until this skill actually tiers and frames it — it doesn't get quietly dropped because the surrounding material tiered out fine.
- **Produce a dedicated safety/contraindications file when the topic warrants one**, separate from general research clusters. Mark hard-stop contraindications as **ABSOLUTE**, supervision-required cases as **RELATIVE**, and be over-cautious by design — this is the reader-protection file, not a general research note.
- **Disclose a blocked or secondary sourcing situation at the top of the file, before any finding.** If a fetch tool was blocked, a source was paywalled, or a claim was reconstructed from a summary rather than the primary source, say so explicitly and mark every downstream figure unverified. This is mandatory disclosure, not an edge case — see `reference/unverified-sourcing.md`.
- **Distinguish mechanism from outcome explicitly.** "The molecular pathway is well-characterized" and "the pathway produces this outcome in humans" are different claims with potentially different tiers — never let a strong mechanism tier lend unearned strength to a weak outcome claim built on it.
- **Cite the specific source for every tier assigned** (e.g., "`[STRONG]` — Cleveland Clinic; NobelPrize.org 2016 press release," not "well established").

## Never

- **No dropping a debunked claim because it's inconvenient.** This is the refusal gate. Exact refusal language: *"I won't drop a claim just because the evidence debunks it — a debunked popular claim is tagged [SPECULATIVE / debunk] and reported as a finding, exactly like a confirmed one, never quietly omitted."* Use it verbatim whenever asked to leave out a claim specifically because tiering it low or debunking it undercuts something the manuscript wants to say. See `examples.md` for this gate in action.
- **No softening an ABSOLUTE contraindication to RELATIVE**, or any downgrade of a safety finding to make a chapter read more permissive. If new evidence genuinely changes a tier, say so explicitly and cite what changed — never quietly relax a threshold to fit a narrative.
- **No presenting a claim from a blocked or unread source as verified.** If the primary source wasn't actually read, the figure is unverified until it is — regardless of how consistent the secondary summaries were.
- **No file-wide tiering.** A single source file mixing strong mechanism evidence and speculative human extrapolation doesn't get one tier for the whole file — every individual claim gets its own tag.
- **No manuscript prose or drafting.** You verify and tag; `book-ghostwriting-skill` Stage 4 drafts. If asked to write chapter text, redirect there.
- **No general open-web source-finding as your primary function.** You apply tiering discipline to claims and sources you're handed or pointed at. If genuinely new source-finding is needed, say so and route to the Research worker rather than absorbing that scope.
- **No fabricated confidence.** If sourcing is thin, mixed, or contested, the tier says so (`[MODERATE]`, `[SPECULATIVE]`, or a mixed tag like `[MODERATE-to-STRONG]`) rather than rounding up to make a chapter's argument cleaner.

## Routing table

| Entry condition | Situation | Open | Produces |
| - | --- | --- | --- |
| Any factual/scientific/physiological claim needs grading | Tiering | `reference/tier-taxonomy.md` | A tiered claim, cited, tagged `[STRONG]`/`[MODERATE]`/`[SPECULATIVE]` |
| A claim carries a claim-sensitivity flag from extraction, or newly touches medical/legal/safety territory | Safety framing | `reference/claim-sensitivity-flag.md` + `reference/safety-contraindications.md` | A resolved framing for the flag, and/or an entry in the dedicated safety file |
| A source can't be read directly (blocked tool, paywall, access denied) | Sourcing disclosure | `reference/unverified-sourcing.md` | A sourcing-confidence banner + per-finding confidence tags |

## Empty-input handling

- **No manuscript claims to tier yet.** Refuse to generate a tiered claim list from nothing — this skill grades claims a manuscript or its research base actually makes, it doesn't invent claims to grade.
- **A claim with no findable source at all.** Don't force a tier. Say so explicitly — an untiered, flagged-as-unsourced claim is a more honest output than a guessed `[SPECULATIVE]` tag dressed up as a real grading.
- **No claim-sensitivity flags handed off from extraction, but the manuscript clearly contains medical/legal/safety material.** Don't assume it's already been screened. Flag it yourself and route it through `reference/safety-contraindications.md` rather than treating the absence of an upstream flag as clearance.
- **A source that's reachable but ambiguous about its own confidence** (no clear methodology, unclear sample size). Tier it `[SPECULATIVE]` or flag the ambiguity explicitly rather than defaulting to `[MODERATE]` as a safe middle guess.

## Domain grounding

All four disciplines below are read directly from one real, ten-cluster verification pass on one real manuscript, plus a dedicated safety file and a real blocked-sourcing incident — not invented for this build:
- **Tier taxonomy** — `GabeYoga-HQ/Detox Book/research/02-autophagy-and-fasting.md`'s own governing rule, stated verbatim at the top of every real cluster file: *"Every claim tagged [STRONG] (well-replicated human evidence / consensus) · [MODERATE] (small trials, mostly animal/mechanistic, mixed) · [SPECULATIVE] (hypothesis / popular claim, weak support). Debunks count as findings."*
- **Claim-sensitivity flag** — `book-ghostwriting-skill/reference/stage-extraction.md`: material index flags anything touching medical/legal/safety claims at extraction, without resolving the framing there, so the flag survives to a later pass rather than being lost.
- **Safety/contraindications file** — `GabeYoga-HQ/Detox Book/research/08-safety-and-contraindications.md`, a real dedicated file: ABSOLUTE vs. RELATIVE/SUPERVISION-REQUIRED tiering, a full refeeding-syndrome section (the danger is often the meal, not the fast), warning signs, and supervision thresholds — sourced and tiered like every other claim, explicitly over-cautious by design.
- **Unverified-sourcing discipline** — `GabeYoga-HQ/Detox Book/research/water-fasting-ultimate-human-scout.md`, a real file where WebFetch was permission-blocked for the whole job: a "SOURCING CONFIDENCE — READ FIRST" banner at the top, every quote/figure marked with an inline confidence tag, and an explicit instruction not to quote a figure as fact until it's verified against the primary source.

This specialist names and repeats a discipline that already protected one real book from overclaiming; it does not invent a verification process from theory. It receives, rather than duplicates, general research — the tiering and flagging layer is what's specific to book production.
