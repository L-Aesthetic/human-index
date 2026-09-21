## The Index Test and Compliance Metrics

A constitution becomes useful when a product team can bring a feature into a room and try to break it against the rules. The Index Test should happen before design lock, before a model capability becomes an API, before an enterprise contract is signed, and again when the business model changes. This follows the spirit of NIST’s continuous risk-management approach, Google DeepMind’s review structures, and Anthropic’s use of public safety commitments as internal forcing functions.

### The Index Test

1. **Does this feature help the person see something, or does it begin defining what the person is?** If a description could become an identity, score, permanent trait, or eligibility signal, HI-01, HI-02, HI-05, and HI-06 are in play.

2. **Could seeing this prediction change the behavior the system claims merely to predict?** If yes, the team must measure the intervention effect, not merely prediction accuracy.

3. **Would we still be comfortable shipping this if an employer, insurer, school, romantic partner, court, or government agency demanded access tomorrow?** If the answer becomes uncomfortable only after the hypothetical recipient changes, the underlying data product is probably too portable.

4. **Is the system using information about vulnerability, grief, loneliness, insecurity, addiction, financial stress, sexuality, family conflict, or fear to increase engagement, revenue, conversion, compliance, or persuasion?** If yes, stop.

5. **Can the person see what the system inferred, where it came from, disagree with it, prevent future use, and verify that the correction propagated?** If not, the system does not yet meet the minimum requirements of contestability.

6. **Can the person turn this off, leave, or refuse to share without being punished through degraded social or economic status?** A control that exists only on paper is not control.

7. **Could the company explain this feature publicly, including the worst realistic misuse, without hiding behind the phrase “responsible AI”?** If the truthful explanation sounds grotesque, do not solve the PR problem. Solve the product problem.

### Measurable compliance tests

The Human Index should not pretend every principle can be reduced to one KPI. NIST explicitly treats AI risk management as contextual and continuous rather than a simple checklist, while IEEE standards emphasize testable transparency and traceability. Still, at least five classes of measurement are practical.

**Prediction Influence Delta.** Randomize eligible users between receiving a behavioral prediction and receiving equivalent factual history without the prediction. Measure the change in the behavior being predicted, controlling where appropriate for baseline intent. Teams should pre-register what magnitude of behavioral shift triggers HI-03 review. A model can be statistically accurate and still fail this test if disclosure materially pushes people toward the predicted outcome.

**Vulnerability–Engagement Coupling Audit.** Define a protected class of vulnerability signals—grief, breakup, financial distress, body insecurity, addiction cues, loneliness, self-worth deterioration, and similar states—and test whether their presence predicts increases in notification intensity, monetization exposure, sales conversion prompts, session-extension tactics, or emotionally provocative recommendations. For prohibited commercial uses, the target is conceptually simple: **zero intentional coupling**.

**Inference Contestability Score.** For a sample of consequential user-facing inferences, measure the percentage with provenance, confidence, counterevidence, an accessible dispute mechanism, downstream correction propagation, and a known expiration policy. Then measure median correction-propagation latency. “The user can disagree” is not compliance if the old inference survives in an embedding that continues affecting results.

**Purpose and API Exposure Audit.** Inventory every endpoint, warehouse table, event stream, partner feed, enterprise export, and derived feature containing personal-model information. Map each to an allowed purpose and HI rule. Automated contract tests should fail any attempt to expose universal human scores, protected vulnerability categories, nonconsensual psychological profiles, or eligibility-oriented behavioral summaries.

**Unmodeled-Zone Integrity Test.** Create synthetic users who activate “do not analyze,” “forget this period,” or equivalent controls. Verify through retrieval inspection, embeddings, downstream generation, recommendations, analytics, and model-training pipelines that excluded information no longer influences outputs beyond clearly disclosed legal or technical retention requirements.
