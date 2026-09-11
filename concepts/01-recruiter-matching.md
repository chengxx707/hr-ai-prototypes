# Recruiter Matching — design concept

**Stage:** concept · **Not built** · No code exists for this
**Domain:** recruiting / talent acquisition

---

## 1. The problem, as it actually shows up

A job description describes an ideal. A CV describes a past. Screening is the act of bridging that gap — and in most organizations it is bridged by one person reading hundreds of documents against a mental model that has never been written down.

Three failure modes I have seen repeatedly:

**1. Keyword matching punishes non-linear careers.**
A candidate who moved from operations into analytics gets filtered out for "5 years of BI experience" while a weaker candidate with the right job titles passes. The filter encodes the path, not the capability.

**2. Requirements inflation is invisible.**
Hiring managers add requirements defensively, one at a time. Nobody sees the cumulative effect until the pipeline dries up and the role stays open for four months.

**3. The reasoning is never captured.**
Screening decisions happen in a recruiter's head and disappear. When challenged — by a manager, by a candidate, by an auditor — there is nothing to point at.

> **Note:** the specific figures and cases behind these observations need to be filled in from my own practice before this document is used as a portfolio piece. The failure modes above are the pattern; the evidence is mine to supply.

## 2. What I would design

Not a scorer. A **structured comparison tool**.

**Input:** role requirements, expressed as capability dimensions rather than keywords, weighted by the hiring manager and visible for challenge.

**Process:** the system extracts candidate evidence per dimension, and — this is the part that matters — **states what it could not find.** Gaps are shown as gaps, not as zeros.

**Output:** a shortlist with, for each candidate, a one-line rationale linked to the specific evidence that produced it.

**What the human does:** decides. Every ranking can be overridden, and overrides are logged with their reason. Those logs are the most valuable output over time — they are the organization's real hiring criteria, written down for the first time.

## 3. Why not just use an LLM to screen

Because a decision that cannot be explained cannot be defended, and an indefensible hiring decision is a legal and reputational liability. The reasoning has to survive being questioned by someone who disagrees.

This is also why the design proposes rather than decides. Removing the human does not remove the bias — it moves the bias somewhere nobody can inspect it.

## 4. What would need to be true

- Role requirements captured as dimensions, not a wish list → requires the hiring manager to commit to what matters, in writing
- Structured evidence extraction from unstructured CVs → the genuinely hard technical part
- Override logging from day one → otherwise the feedback loop never closes

## 5. Open questions

- How do you keep the dimension set from quietly converging back into a keyword list?
- Where is the line between "not found" and "not present"? The tool must not report absence as evidence of absence.
- Can override logs be used to audit the tool itself for systematic bias? That may be the most valuable use of the data.
