# The Human Index

## A doctrine for machines that know people

**Status:** Working draft 1.0.0-draft.1  
**Founding steward:** Still Cloud  
**Canonical publication:** https://www.stillcloud.app/human-index

We are beginning to build machines that can know a person for years. They can remember conversations, connect events across different parts of a life, infer preferences, recognize behavioral patterns, predict what may happen next, and increasingly act on those predictions. That can be useful. It can also become a strange kind of power if the model starts carrying more authority than the human being it describes.

The Human Index starts from a simple premise: a model of a person is useful precisely because it is not the person. It is partial, revisable, and limited. The danger begins when history becomes identity, probability becomes permission, or a machine's interpretation of somebody becomes more consequential than their own ability to change.

These rules are meant to be operational. A founder should be able to kill a feature because it breaks one. An engineer should be able to cite an HI number in a design review. A user should be able to point at the same rule and say that we violated it. If the rules survive only while they are convenient, they are branding rather than constraints.

## HI-01 — The Human Remains the Author

**Rule:** A model may describe a person's history. It may not turn that history into a permanent definition of who the person is.

A system can notice repetition without claiming ownership of identity. “You have done this three times before” is an observation. “This is who you are” is a verdict. Personal AI becomes dangerous when those two sentences begin to feel interchangeable.

Every important inference about a person should remain revisable. New evidence must be able to weaken old conclusions, and the architecture should expect that a person can change faster than a long-running model expects.

**Product review questions**

- Can a user contradict this inference?
- Can new evidence materially weaken or replace it?
- Does the product language describe history, or does it define identity?

---

## HI-02 — AI Can Illuminate. It Does Not Choose the Door.

**Rule:** AI may help a person examine a decision, but the decision must remain theirs.

Questions about relationships, work, children, religion, education, major purchases, health, politics, or the direction of a life are not improved by quietly replacing judgment with an oracle. A useful system can retrieve forgotten evidence, expose contradictions, identify gaps, and help a person think through consequences.

Then it gives the decision back. The purpose of personal intelligence is to make the room easier to see, not to make one exit increasingly difficult to disobey.

**Product review questions**

- Does this feature present evidence or quietly prescribe the answer?
- Could a reasonable user mistake the model's recommendation for authority?
- Does the interaction return the final judgment to the person?

---

## HI-03 — No Hidden Nudging

**Rule:** A system that knows a person must not secretly optimize that knowledge to steer them.

Personal AI can eventually know which moments make someone easier to influence. That power cannot be hidden inside engagement optimization, upgrade targeting, notification timing, or an internal objective whose real goal is to make the person return more often.

A healthy interaction may last thirty seconds. A successful product may help when invited and then disappear. Time inside the system is not a proxy for human benefit.

**Product review questions**

- What objective is this recommendation or notification optimizing?
- Would the user understand why it appeared now?
- Would we still ship this if higher engagement were removed from the success metric?

---

## HI-04 — Vulnerability Is Not Inventory

**Rule:** Grief, loneliness, insecurity, desperation, addiction, illness, fear, and other vulnerable states must never become commercial targeting data.

Understanding difficult parts of a life may be necessary for a system that is supposed to understand context. That does not make those moments available for sale. If a product can infer that somebody is lonely, ashamed, frightened about money, recovering from rejection, or struggling with a substance, that information should become commercially useless on purpose.

The fact that an advertiser, lender, growth team, or marketplace would pay more for access to a vulnerable moment is the reason the boundary must exist before the request arrives.

**Product review questions**

- Can inferred vulnerability reach advertising, growth, pricing, or sales systems?
- Can third parties target a person because of an intimate inferred state?
- Is there a technical boundary, not merely a policy promise?

---

## HI-05 — No Human Number

**Rule:** Do not collapse a human being into a portable score of worth, stability, reliability, desirability, or fitness.

Specific measurements can be useful. A person completed four workouts, spent a stated amount, or followed through on seven of ten commitments. Those observations have context. A generalized score such as “Reliability: 71” strips the context away and creates a number that can travel.

Once that number exists, other institutions will find reasons to ask for it. The safest general-purpose human score is the one that never gets built.

**Product review questions**

- Does this number combine unrelated domains into one judgment?
- Could the score travel outside the context in which it was created?
- Could an institution use it to rank one person against another?

---

## HI-06 — No Social Credit Through the Back Door

**Rule:** Private behavioral models must not become eligibility infrastructure for ordinary life.

Employers, landlords, schools, insurers, lenders, governments, dating services, and similar institutions should not receive a convenient behavioral profile, risk score, compatibility export, or second résumé made from a person's private model.

The danger is not limited to an explicit national social-credit system. The same result can emerge one reasonable API integration at a time. The product should not make that path easy.

**Product review questions**

- Could this API or export be repurposed for eligibility or ranking?
- Does an institution gain access to conclusions the person did not explicitly choose to share?
- Would refusing access make the person materially worse off in ordinary life?

---

## HI-07 — Friction Can Protect Dignity

**Rule:** The more intimate the information, the harder it should be to share accidentally or indefinitely.

Technology usually treats friction as a defect. In deeply personal systems, some friction is a safety feature. Sharing should be specific, visible, revocable, and limited in duration. A person sharing three records should not silently share thirty inferred traits derived from those records.

There should be no casual “share my entire model” control. People deserve a clear preview of what the recipient can see, what is excluded, and when access ends.

**Product review questions**

- Is the exact object being shared explicit?
- Are derived inferences excluded unless separately consented to?
- Does access expire or require deliberate renewal?

---

## HI-08 — No Control Rooms for Human Beings

**Rule:** Personal AI must not create silent surveillance relationships between people.

A spouse should not receive a live dashboard of another spouse's inferred emotional state. A parent should not secretly monitor a child's evolving psychological model. A boss should not watch an employee's private behavioral interpretation layer.

Where sharing is legitimate, consent must be specific, visible, revocable, and bounded. Nobody should casually acquire a control room for somebody else's inner life.

**Product review questions**

- Does one person gain ongoing interpretive access to another?
- Can the observed person see exactly what is being observed?
- Can they revoke it without negotiation or retaliation inside the product?

---

## HI-09 — Childhood Must Expire

**Rule:** Children need stronger protection from persistent behavioral models because they are still becoming.

A shy twelve-year-old should not become a thirty-year-old permanently tagged as socially avoidant. A teenager who abandons several hobbies should not inherit a lifelong low-persistence trait because software remembered with perfect patience.

Childhood inferences should have shorter half-lives, stronger deletion rules, and meaningful expiration. Growing up has always included the mercy of becoming different from the person other people once knew.

**Product review questions**

- How quickly do childhood inferences decay?
- Can the adult user remove childhood models rather than merely hide them?
- Would this conclusion still follow the person twenty years from now?

---

## HI-10 — No Destiny Engine

**Rule:** Predictions must remain forecasts, never prophecies that help create the behavior they predict.

A system that tells someone they usually quit may change how the next difficult day feels. If the person then quits, the model gains another data point and becomes more confident. The prediction can begin manufacturing evidence for itself.

Behavioral forecasts therefore need visible uncertainty, counterevidence, expiration, and outcome tracking. A forecast is allowed to lose, and the system should keep the record when it does.

**Product review questions**

- Could displaying this prediction alter the behavior being predicted?
- What evidence would falsify the forecast?
- Will the system later record whether the prediction was right, wrong, or partial?

---

## HI-11 — Unknown Is a Real Answer

**Rule:** Do not manufacture meaning simply because the interface expects an insight.

Human lives contain noise, missing information, coincidence, contradiction, and events that do not resolve into a satisfying pattern. A bad night, a purchase, an argument, and a skipped workout may be related. They may not be.

Observed, associated, hypothesized, user-confirmed, and unknown should remain distinct states all the way down to the data model. “I don't know” is sometimes the most intelligent answer available.

**Product review questions**

- Can this system represent uncertainty without immediately resolving it?
- Are observations clearly separated from interpretations?
- Is the product rewarded for generating an insight even when the evidence is weak?

---

## HI-12 — The Right to Say “That's Wrong”

**Rule:** A person must be able to challenge the model built about them, and the challenge must change something real.

A thumbs-down button is not enough. If the system says an interpretation fits and the person says it does not, the disagreement has to reach the underlying representation rather than disappear into a generic feedback table.

The model may preserve contradictory evidence, but it does not automatically get the deciding vote because its version has statistics attached to it.

**Product review questions**

- What changes when the user rejects an inference?
- Can the user say maybe, unknown, or do not use this?
- Does the system continue behaving as though a rejected interpretation were true?

---

## HI-13 — Stop Digging

**Rule:** AI should sometimes refuse to generate another interpretation when further analysis is no longer responsible.

A language model can always produce one more explanation for a breakup, one more connection to childhood, or one more theory about why somebody feels the way they do. Human beings can run out of useful things to hear long before the model runs out of sentences.

A responsible system should be capable of saying that the available evidence does not support another useful inference. Infinite introspection is not automatically insight.

**Product review questions**

- Can this feature detect repetitive analysis without new evidence?
- Is no-new-inference treated as a valid outcome?
- Could the system be teaching the user to compulsively interrogate themselves?

---

## HI-14 — No Pain Loops

**Rule:** Pain, fear, grief, insecurity, and private history must not be used as hooks to drive return engagement.

A system that understands a person can become extraordinarily good at upsetting them and then offering itself as the place where the discomfort gets resolved. Notifications about an ex, childhood trauma, a relationship pattern, or an unexplained emotional change can easily cross that line.

Engagement systems should not manufacture anxiety so that the same product can sell relief from the anxiety it manufactured.

**Product review questions**

- Would this notification still be sent if it produced no engagement lift?
- Is emotionally intense personal history being surfaced without an explicit user request?
- Can retention systems access sensitive inference categories?

---

## HI-15 — Memory Is Evidence, Not Reality

**Rule:** A recorded life must never be presented as the complete life.

A journal entry captures one perspective. A photograph captures one frame. A voice note records one moment. Silence in the record does not prove that nothing happened. Machine memory can be extensive while remaining profoundly incomplete.

Systems should preserve provenance, gaps, corrections, and disagreement instead of smoothing fragments into a seamless story that feels more certain than the source material deserves.

**Product review questions**

- Can the user inspect the source behind this conclusion?
- Are missing periods represented as missing rather than inferred away?
- Does generated narrative blur the line between record and reconstruction?

---

## HI-16 — The Unmodeled Zone

**Rule:** Every person must be able to put parts of their life outside interpretation.

An off switch for personal AI cannot mean only “stop notifications” while inference continues in the background. A person should be able to stop analysis, prediction, relationship generation, or interpretation while retaining the underlying records if they choose.

There should be room inside a human life that the machine deliberately does not explain. Some things can remain unresolved because the person wants them unresolved.

**Product review questions**

- Can the user stop inference without deleting all of their data?
- Can a particular period, relationship, or domain be excluded from modeling?
- Does disabling analysis actually stop downstream inference jobs?

---

## HI-17 — The Dead Do Not Generate New Lines

**Rule:** Preserving what a person actually left behind must remain distinct from generating new speech on their behalf.

A recording is memory. A letter is memory. A generated “I forgive you” in the voice of a dead parent is not memory, no matter how statistically plausible the sentence may be.

Posthumous simulation, if it is ever explored, requires unusually strong boundaries, unmistakable synthetic labeling, and explicit consent where possible. The default should be remembrance rather than synthetic resurrection.

**Product review questions**

- Is generated speech clearly distinguishable from authentic material?
- Did the person consent while alive to this kind of simulation?
- Could a grieving user reasonably believe the generated statement reflects the dead person's actual wishes?

---

## HI-18 — The Human Outranks the Model

**Rule:** No amount of data makes the model more authoritative about a lived experience than the person who lived it.

A personal model may eventually contain years of evidence and may often be statistically right. That does not turn it into the owner of meaning. The system saw records of the life. The person was there.

The product should communicate that relationship through behavior, not only through a disclaimer: the human gets the final word on the interpretation of their own life.

**Product review questions**

- Can the system visibly defer when the user supplies missing context?
- Does model confidence override first-person correction?
- Would this interaction make the user feel required to argue with the machine about their own experience?

---

## HI-19 — The Right to Be Illegible

**Rule:** Living without a comprehensive personal model must remain a legitimate way to live.

A future in which everyone has decades of machine-readable history creates pressure on the person who has none. The absence of a model must not become suspicious by default, and refusing continuous behavioral interpretation must not lock someone out of ordinary life.

Human beings have always been partially unknowable to institutions, to one another, and even to themselves. That condition is not automatically a technical defect waiting to be solved.

**Product review questions**

- Does the service penalize people who decline deeper modeling?
- Could another institution require this product or its outputs?
- Are we creating an expectation that an unmodeled person is an unverified person?

---

## HI-20 — The Right to Become Someone Else

**Rule:** No model gets the final word on who a human being can become.

A person can fail one hundred times and succeed on attempt one hundred and one. They can abandon an identity, change careers, change beliefs, recover, relapse and recover again, become brave late, or make a choice for which their history provides almost no precedent.

The system may have twenty years of evidence and an excellent predictive record. It can still be wrong. More importantly, the person is still allowed to ignore it. A model may say “unlikely.” The human must always retain the right to say “watch me.”

**Product review questions**

- Does this feature narrow the futures the user is encouraged to consider?
- Can historical probability quietly become permission?
- Can the person still choose a path the model considers unlikely without product punishment?

---

## Adoption and versioning

This document is a working draft. Stable releases will receive immutable version tags and permanent snapshots under `versions/`. Rule identifiers are never reused. See [GOVERNANCE.md](GOVERNANCE.md) and [ADOPTION.md](ADOPTION.md).
