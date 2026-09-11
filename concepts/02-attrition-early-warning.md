# Attrition Early Warning — design concept

**Stage:** concept · **Not developed** · This is a product definition, not a specification

---

## 1. The problem, as it actually shows up

Every resignation arrives on time and is understood too late.

By the time a manager hears "I've accepted another offer", the decision was made months earlier — usually at a point when someone could have acted. The organization discovers the outcome and never sees the process.

Three properties of the problem that shape any solution:

**1. The signal is diffuse.** No single event predicts a resignation. It is a slow accumulation: scope narrowing, a manager change, a project ending, two years without a real conversation about the next step.

**2. The most useful data is the least recorded.** HR systems hold salary, grade, tenure and performance rating. They do not hold "the work stopped being interesting". The dimensions that matter most are the ones nobody types in.

**3. Acting badly is worse than not acting.** A flag that makes a manager treat someone differently will accelerate the departure it was meant to prevent. This is the failure mode that kills most versions of this product.

## 2. Where I think the real opportunity is

Not prediction. **Conversation timing.**

A risk score invites a manager to manage *the score*. A better product answers a narrower, more useful question: *who has not had a substantive career conversation in the last six months, and should?*

That reframing does three things at once:
- it uses data organizations actually have
- it produces an action that is harmless if the signal is wrong
- it improves the situation even when the prediction is entirely off

**The design principle: the output is a prompt for a human conversation, never a label attached to a person.**

## 3. What a first version might look like

| Layer | Content |
|---|---|
| Inputs | Tenure, role changes, manager changes, time since last development conversation, internal mobility history |
| Output | A short list of conversations to have this month — with the reason stated |
| Never | A per-person score visible to anyone outside the direct manager |
| Governance | Employees can see what data feeds it. This is a feature, not a compliance cost |

## 4. What would need to be true

- Managers must be able to act on a flag without it being a verdict — the framing has to be built into the interface, not just the policy
- The list must be short. A list of forty names is a list nobody uses
- Data access rules must be decided before the first version, not after

## 5. Open questions

- Does showing an employee their own "conversation due" status change its meaning? My instinct: it improves it.
- How do you measure whether this worked, when the successful outcome is a conversation that never becomes a resignation?
- Is the honest framing "this reduces avoidable attrition slightly" rather than "this predicts attrition"? I think yes, and the product should say so.

> **Note:** this concept needs a real worked example (an anonymized scenario) before it is credible as a portfolio document. To be added.
