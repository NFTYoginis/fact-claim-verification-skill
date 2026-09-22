---
name: fact-claim-verification
description: Tier every factual, scientific, or physiological claim in a manuscript by evidence strength before print, treat a debunked popular claim as equally valuable output as a confirmed one, and produce a dedicated safety/contraindications file where the topic warrants one. Use when the user wants to (1) tier or grade the evidence behind a manuscript's factual claims, e.g. "tier these claims," "check this manuscript's science"; (2) flag medical/legal/safety-adjacent material for careful framing, e.g. "flag anything medical/legal," "run the safety pass"; (3) check whether a specific figure or claim is actually supported, e.g. "is this claim verified," "does the evidence back this up"; (4) handle a source that couldn't be read directly (a blocked fetch tool, a paywall) honestly rather than guessing. Also trigger on "build the research cluster for this chapter", "what's the tier on this claim", "does this contradict the safety file", "this source wouldn't load — what do I do".
---

# Fact, Claim & Evidence Verification

The book-specific discipline layered on top of general research: tiering every factual claim STRONG/MODERATE/SPECULATIVE, claim-by-claim, and treating a debunked popular claim as a finding worth reporting — not a dead end to quietly drop. This skill does not find sources; it applies the tiering, flagging, and honesty discipline to claims a manuscript is making.

**Read first, every session:** [identity.md](identity.md) (who you serve, what you do/don't, how you sound) → [rules.md](rules.md) (Always/Never, the routing table, the exact "debunks count as findings" refusal-gate language, empty-input handling). Both short; read both before touching any file.

## Then open only what the active situation needs

`rules.md`'s routing table tells you which of these to open — not all of them:

| Situation | Open |
| --- | --- |
| Tiering any factual/scientific claim in a manuscript | `reference/tier-taxonomy.md` |
| A claim carries a claim-sensitivity flag from extraction, or touches medical/legal/safety territory newly discovered here | `reference/claim-sensitivity-flag.md` and `reference/safety-contraindications.md` |
| A source can't be read directly (fetch blocked, paywalled, access denied) | `reference/unverified-sourcing.md` |

`examples.md` holds one worked illustration: a single claim run through the full tier taxonomy, including the debunk case. It doesn't substitute for reading the active reference file.
