# Human Index Pre-Ship Test

The Human Index Test is not a score. It is a review that forces a team to state what a feature is doing to, with, or on behalf of a human model before the feature ships. A vague answer is a reason to keep reviewing rather than a box to check.

## HIT-01

What claim about a person is this feature making, and what evidence would cause the system to change its mind?

## HIT-02

Could showing this prediction influence the behavior it predicts?

## HIT-03

Can the person disagree with this interpretation in a way that changes the underlying model?

## HIT-04

Does any old inference survive indefinitely? If so, why?

## HIT-05

Could this data, API, score, or derivative be useful to an employer, school, insurer, lender, landlord, partner, or government?

## HIT-06

Are we compressing unrelated parts of a person into a general judgment?

## HIT-07

Could a growth, advertising, pricing, or sales system learn when this person is unusually vulnerable?

## HIT-08

Can the user stop inference without deleting everything?

## HIT-09

If this person were twelve, should this conclusion still exist when they are thirty?

## HIT-10

If the model is wrong, where is the record of that failure?

## Recording a review

A review should name the feature, product or model surface, owner, date, HI rules implicated, evidence considered, unresolved questions, mitigation, and final disposition. The available dispositions are **ship**, **ship with constraints**, **return for revision**, and **do not ship**. Teams should preserve the written review with the same seriousness they preserve security or privacy decisions.

A failed test does not always imply the same remedy. Sometimes the answer is a narrower permission boundary, shorter retention, explicit provenance, a different metric, or a user-visible correction path. Sometimes the correct answer is that the feature should not exist.
