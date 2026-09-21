# Implementation Notes

The Human Index is not satisfied by good copy alone. Many of its commitments require architectural boundaries.

## Provenance and epistemic state

Systems that infer things about people should preserve source material and distinguish observation, association, hypothesis, user-confirmed interpretation, and unknown. A generated narrative should not erase the difference between those states.

## Correction and contestability

A user's rejection of an important inference should change the model or remove the inference from active reasoning. "Thanks for your feedback" is not contestability if downstream behavior remains unchanged.

## Decay and obsolescence

Behavioral inferences need lifetimes. Old evidence should lose authority where appropriate, and childhood inferences require substantially stronger decay and deletion behavior. Permanent identity fields should be exceptional.

## Prediction receipts

Predictions should be timestamped, scoped, falsifiable, and revisited after the relevant window. Outcome tracking should preserve misses as well as hits. A system that remembers the user's failures while forgetting its own will systematically overstate its authority.

## Sharing boundaries

Sharing should be object-specific. Derived inferences, hidden metadata, and private source material should not ride along unless separately selected and disclosed. High-impact sharing should include recipient, purpose, duration, preview, revocation, and logging.

## Analytics and commercial separation

Sensitive inferred states should be technically separated from advertising, pricing, growth, engagement, and sales targeting systems. A policy promise is weaker than an architecture in which the prohibited use cannot occur.

## Institutional APIs

Avoid general-purpose endpoints that return behavioral risk, reliability, employability, compatibility, parenting fitness, psychological stability, or similar portable judgments. If an API would make HI-06 easy to violate, redesign the API rather than relying only on downstream terms.

## The unmodeled zone

Users should be able to stop inference for a domain, time period, relationship, or source without necessarily deleting every underlying record. Background jobs, embeddings, summaries, relationship generation, and prediction pipelines must respect that state.

## Children and posthumous use

Childhood data should use stronger defaults for minimization, decay, deletion, and adult re-consent. Posthumous simulation should be isolated from ordinary memory-preservation features, unmistakably synthetic, and never implied to be authentic speech.

## Review trail

Human Index reviews should be durable artifacts attached to major features, model behaviors, data flows, and enterprise uses. The review should be revisited when scope, model capability, data access, or business use changes.
