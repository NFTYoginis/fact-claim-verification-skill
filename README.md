# Fact, Claim & Evidence Verification

A folder-based ICM specialist that tiers every factual, scientific, or physiological claim in a manuscript by evidence strength before print, and treats a debunked popular claim as equally valuable output as a confirmed one.

This formalizes a discipline already run across ten real research-cluster files plus a dedicated safety file, on one real book. It is not a theory of fact-checking — it's a repeat of what already kept one book from overclaiming.

## What this is

Four disciplines, applied to a manuscript's factual claims:

1. **Tier taxonomy** — `[STRONG]` / `[MODERATE]` / `[SPECULATIVE]`, claim-by-claim, not file-by-file. Debunks count as findings.
2. **Claim-sensitivity flag handoff** — receives a flag from `book-ghostwriting-skill` Stage 2 (extraction), resolves the framing, hands a checkable result to Stage 5 (revision).
3. **Dedicated safety/contraindications file** — ABSOLUTE vs. RELATIVE/SUPERVISION-REQUIRED, over-cautious by design, where the topic warrants one.
4. **Unverified-sourcing banner** — mandatory disclosure when a source couldn't be read directly, with per-finding confidence tags, so a figure never gets quoted as fact before it's actually verified.

Full detail per discipline: `reference/`.

## Setup

1. Load this folder into a Claude Project, or point a Claude Code session at it — `SKILL.md` lets Claude Code auto-discover and trigger it from a natural request (e.g. "tier these claims" or "run the safety pass"); it routes to `identity.md` → `rules.md`, then to the one `reference/` file the active situation needs.
2. Working from the raw files directly (no `SKILL.md` support): read `identity.md` → `rules.md` → `examples.md` in that order, then open only the `reference/` file for the discipline actually in play.
3. Bring the manuscript's claims (and any claim-sensitivity flags from extraction) and the sources backing them — this skill grades and tags what's already been claimed; it doesn't research from scratch.

## First-run prompts

- *"Tier the claims in this chapter's research cluster."*
- *"Does this popular claim actually hold up?"*
- *"Build the safety file for this topic."*
- *"This source wouldn't load — how do I handle it honestly?"*

## What this specialist does and doesn't do

See `identity.md` and `rules.md` for the full contract. In short: it never does general open-web source-finding, never drafts manuscript prose, never softens an ABSOLUTE contraindication, and never presents an unverified figure as confirmed — it owns the tiering, the claim-sensitivity handoff, the safety file, and the sourcing-confidence discipline, using a methodology that already protected one real book from overclaiming.

## License

MIT — see `LICENSE`.
