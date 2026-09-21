### Enterprise contract language

The following clauses are illustrative starting points for U.S. counsel, not substitutes for jurisdiction-specific legal review. They are intentionally stricter than “comply with applicable law” because the purpose is to bind customers to the Human Index even where the law has not yet caught up.

**Prohibited Eligibility Use**

> Customer shall not use, permit, or facilitate use of Personal Model Data or Derived Personal Inferences to determine, rank, materially influence, or condition any natural person’s eligibility for employment, promotion, termination, housing, education, insurance, credit, healthcare, public benefits, immigration status, legal treatment, or access to essential services.

This aligns with the Index’s HI-06 boundary and also avoids pushing intimate personal-model data into areas where existing U.S. employment and credit laws already impose significant anti-discrimination and explanation duties.

**No Generalized Human Scoring**

> Customer shall not combine Personal Model Data or Derived Personal Inferences into a generalized score, grade, rank, tier, index, or classification purporting to measure a person’s trustworthiness, stability, reliability, employability, desirability, parenting fitness, psychological fitness, social value, or equivalent generalized characteristic.

**No Vulnerability Exploitation**

> Customer shall not use Personal Model Data, Derived Personal Inferences, or system outputs to identify, target, price, persuade, solicit, or otherwise influence a person based on grief, loneliness, financial distress, addiction, insecurity, mental or emotional distress, family conflict, sexual vulnerability, or another state of heightened susceptibility.

The FTC’s dark-pattern and biometric-policy work makes clear that manipulative design, unexpected data use, and failures to evaluate foreseeable consumer harm are already areas of regulatory attention.

**Purpose Limitation and No Derivative Laundering**

> Customer may process Personal Model Data solely for the Approved Purpose stated in this Agreement. Customer shall not derive, infer, transform, embed, aggregate, pseudonymize, or otherwise process such data for the purpose of circumventing a prohibited-use restriction. A prohibited inference remains prohibited when represented as an embedding, latent variable, composite metric, segment, or proxy.

**Revocation, Deletion, and Downstream Control**

> Upon expiration or revocation of access, Customer shall cease new processing immediately and shall delete or render inaccessible covered data and derived representations within the contractual deletion period, except where retention is required by law. Customer shall propagate deletion obligations to subprocessors and provide auditable confirmation upon request.

**Audit and Incident Disclosure**

> Provider may audit Customer’s compliance with the Human Index restrictions through reasonable technical, documentary, and independent third-party review. Customer shall notify Provider without undue delay of any actual or suspected use inconsistent with the Human Index, shall preserve relevant records, and shall cooperate in mitigation, user notification, access suspension, and deletion.

Contracts alone are not enough. Prohibited use should also be enforced technically through scoped APIs, customer segmentation, permission boundaries, monitoring, rate controls, derived-feature restrictions, and termination rights. The point is to make violating the Index inconvenient even for a customer willing to ignore a PDF.
