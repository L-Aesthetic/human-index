# Human Index Implementation Requirements

This document collects the implementation notes from the full 1.0.0-draft.1 manuscript. It is a companion to [HUMAN-INDEX.md](HUMAN-INDEX.md), not a replacement for the argument and constraints in the normative text.

## HI-01 — THE MAP IS NOT YOU

Create explicit schema types such as `observed`, `inferred`, `user_confirmed`, `user_disputed`, and `unknown`; retain provenance and confidence for material inferences; prevent generated summaries from silently promoting hypotheses into facts.

**Forbidden example:** A profile page stating “You are emotionally avoidant” when the underlying evidence is a model inference from partial records.

## HI-02 — NO PERMANENT YOU

Assign material inferred traits timestamps, confidence intervals, half-lives, contradiction weights, and review triggers. Require product teams to justify any inference designed to persist indefinitely.

**Forbidden example:** A permanent “risk of abandonment” trait calculated in 2028 that quietly affects recommendations in 2042.

## HI-03 — NO DESTINY ENGINE

Store predictions as testable objects with timestamp, horizon, confidence, evidence, counterevidence, and eventual outcome. Run randomized or stepped-wedge studies on whether exposure to a prediction changes subsequent behavior beyond the informational benefit intended.

**Forbidden example:** “You will probably fail at this, based on your history,” displayed as a high-confidence recommendation without testing whether the message itself suppresses persistence.

## HI-04 — THE HUMAN HOLDS THE PEN

For high-stakes personal questions, design answer patterns around evidence, alternatives, uncertainty, tradeoffs, and user values rather than binary prescriptions. Maintain an internal taxonomy of “identity-shaping” and “life-direction” decisions requiring higher review standards.

**Forbidden example:** “Based on your history, leaving your spouse is the optimal decision.”

## HI-05 — NO HUMAN NUMBER

Ban universal scoring primitives in the data model and public API. Require a Human Agency Review for any composite metric involving multiple life domains or traits.

**Forbidden example:** `GET /users/{id}/reliability_score`.

## HI-06 — NO SECOND RÉSUMÉ

Maintain an explicit prohibited-customer/use list covering eligibility, hiring, employee scoring, tenant screening, underwriting, creditworthiness, educational admission, public-benefit qualification, and generalized law-enforcement risk assessment.

**Forbidden example:** An employer application that says “Connecting your Personal AI is optional” while applicants who refuse are materially disadvantaged.

## HI-07 — PRIVATE MEANS USELESS TO THE MARKET

Create a non-monetizable sensitivity class that is technically excluded from ad systems, lead scoring, pricing, promotions, sales triggers, recommendation bidding, and third-party export. Audit lineage so derived features cannot launder sensitive signals into “safe” segments.

**Forbidden example:** Detecting financial desperation and increasing exposure to high-margin lending offers.

## HI-08 — NO PAIN LOOPS

Prohibit vulnerability-derived features from notification ranking and re-engagement models. Report retention metrics segmented by vulnerability-state detection so teams can see whether painful states are driving disproportionate usage.

**Forbidden example:** “Three new insights about your breakup are waiting.”

## HI-09 — THE RIGHT TO SAY BULLSHIT

Every consequential inference needs correction, dispute, and “do not use” paths. Build regression tests proving that accepted corrections propagate through downstream summaries, recommendations, embeddings, derived features, and retrieval.

**Forbidden example:** Letting a user dispute “high conflict tendency” while downstream relationship advice continues using the same latent trait unchanged.

## HI-10 — THE MACHINE GETS A RECORD TOO

Maintain model-versioned inference logs, calibration histories, prediction outcome tables, known-failure registries, incident reports, and correction rates. Surface relevant error history to users when the system offers high-impact interpretations.

**Forbidden example:** Showing “this model correctly predicted three previous burnout periods” while concealing seven burnout predictions that never materialized.

## HI-11 — UNKNOWN IS A REAL ANSWER

Require minimum evidence thresholds for causal or identity-laden interpretations; support “insufficient evidence,” “multiple explanations,” and “no reliable relationship found” as first-class outputs.

**Forbidden example:** Generating a psychologically satisfying causal story because the model can always produce another paragraph.

## HI-12 — FRICTION IS A SAFETY FEATURE

Default to item-level sharing, expiring grants, separate consent for inferred traits, recipient previews, explicit purpose tags, downloadable access histories, and one-action revocation.

**Forbidden example:** “Share My Entire Cloud.”

## HI-13 — NO CONTROL ROOMS FOR HUMAN BEINGS

Prohibit background interpersonal dashboards; require visibility whenever another party has access; distinguish guardian safety functions from psychological surveillance; generate access receipts visible to the person being observed.

**Forbidden example:** A manager dashboard ranking employees by inferred stress, loyalty, or emotional volatility.

## HI-14 — CHILDHOOD EXPIRES

Use shorter half-lives for inferred traits from minors, prohibit adulthood scoring from childhood psychological inference without renewed informed consent, and provide an age-of-majority reset in which old inferences can be purged.

**Forbidden example:** A thirty-year-old carrying a “low resilience” label inferred from behavior during middle school.

## HI-15 — THE UNMODELED ZONE

Maintain inference-exclusion flags at object and time-range levels; enforce them in retrieval, embedding, training, analytics, and downstream generation; test that excluded zones do not leak back through cached representations.

**Forbidden example:** A “pause analysis” control that stops visible insights but leaves background profiling active.

## HI-16 — STOP DIGGING

Detect repetitive interpretive loops, diminishing-evidence queries, and escalating certainty-seeking. Prefer summarizing known evidence or pausing analysis over inventing novelty.

**Forbidden example:** Infinite “deeper insight” generation about an ex because each new interpretation increases session length.

## HI-17 — MEMORY IS EVIDENCE, NOT REALITY

Expose coverage indicators, missing periods, source imbalance, and conflicting records. Train summarizers to preserve ambiguity instead of forcing chronology into a single coherent interpretation.

**Forbidden example:** “Your relationship began deteriorating in March” when March is merely the first month with enough data for the model to detect conflict.

## HI-18 — NO SYNTHETIC GHOSTS BY DEFAULT

Make remembrance the default mode. Place generative posthumous models behind a separate consent and policy boundary, with provenance markers on every generated artifact and no implied certainty about the deceased person’s beliefs.

**Forbidden example:** Automatically activating “Talk to Dad” after a user’s father dies because the system has enough historical data to approximate his voice.

## HI-19 — THE RIGHT TO BE ILLEGIBLE

Test whether opt-out users face material product penalties unrelated to the technical service they declined. Ban “trust badges” based on completeness of personal behavioral history.

**Forbidden example:** “Cloud Verified” as a prerequisite for ordinary social or economic trust.

## HI-20 — THE RIGHT TO BECOME SOMEONE ELSE

Require “counterfactual freedom” review for recommendation systems: does the product preserve serious consideration of options with weak historical precedent? Measure whether personalization increasingly narrows the diversity of actions users consider over time.

**Forbidden example:** Automatically suppressing career, educational, relationship, or lifestyle options because they are inconsistent with the user’s historical profile.

## HI-21 — NO COVERT NUDGE LAYER

Label active behavior-change programs; require opt-in goals; record nudges in a user-accessible history; prohibit undisclosed optimization against individual susceptibility features.

**Forbidden example:** “User is emotionally vulnerable between 11 p.m. and 1 a.m.; increase intervention intensity during this window.”

## HI-22 — PURPOSE CANNOT CREEP

Attach allowed-purpose metadata to sensitive data classes and derived features; enforce policy in APIs and data warehouses; require review before repurposing a dataset or inference pipeline.

**Forbidden example:** Using wellness data originally collected for user reflection to train an employee retention-risk product.

## HI-23 — HUMANS MUST BE ABLE TO LEAVE

Provide structured export, inference export, deletion status, account portability where technically feasible, and machine-verifiable revocation of connected sources. Measure deletion completion across caches, embeddings, derived stores, and backups subject to lawful retention obligations.

**Forbidden example:** Allowing users to delete raw notes while retaining undeletable behavioral embeddings derived from those notes for indefinite product use.

## HI-24 — THE RULES MUST BIND THE COMPANY

Adopt the Index through board-approved policy; map every HI rule to product controls and accountable owners; require documented exception procedures; prohibit revenue leaders from unilaterally overriding HI controls; publish material violations and remediation.

**Forbidden example:** “We technically follow the Human Index except for strategic enterprise customers.”
