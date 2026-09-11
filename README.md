# HR AI Prototypes

> Language: [English](README.md) · [中文](README.zh-CN.md)

Turning fourteen years of HR practice into concrete AI product designs.

**Status:** concept stage — these are product definitions and design documents. Nothing here is built.

---

## Why this repository exists

I spent fourteen years inside HR: recruiting, workforce planning, organizational diagnosis. I know where the friction sits, because I was the one absorbing it. What I could not do was build my way out of it.

This repository is where I write down what I would build and why — starting from the process problem, not from the technology.

## What is here

| Document | Problem it addresses | Stage |
|---|---|---|
| [Recruiter matching](concepts/01-recruiter-matching.md) | Screening volume vs. signal quality | Concept |
| [Attrition early warning](concepts/02-attrition-early-warning.md) | Resignations understood only after they happen | Concept |

## The design principle I hold

Most HR AI products fail the same way: they automate the *decision* and hide the reasoning. A recruiter cannot defend a rejection they cannot explain. An HR manager will not act on a risk score they do not trust.

So both concepts share one constraint: **the system surfaces evidence and proposes; the human decides, and can always see why.**

That is not a technical limitation. It is a product position, and it comes from having been the person on the receiving end of systems that got it wrong.

## Scope and honesty

- These are **design documents, not products.** No code, no working prototype, no validation results are claimed.
- Where a design depends on data most organizations do not actually have, the document says so rather than assuming it away.
- These concepts draw on publicly known practice in people analytics. Specific internal systems of former employers are not reproduced here.

## How this connects to what I am applying for

Enterprise AI adoption is rarely blocked by model capability. It stalls on process ownership, data quality and trust — exactly the things an HR and operations background trains you to notice.

That is the perspective I bring. The engineering depth is what I am applying to add.
