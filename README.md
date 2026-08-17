# SeeFood

**The Shazam for food.**

Point your camera at anything edible. Know what it is.

---

## Why this repo exists

This is a hypothetical product, taken seriously.

The point is not the app. The point is to run [`98kb/skills`](https://github.com/98kb/skills)
against a product that behaves like a real one — a vision that outruns its
implementation, a backlog that argues with itself, issues that arrive half-specified,
branches that need isolating, decisions that need recording before everyone forgets
why they were made.

A toy repo exercises the happy path. A product with an unreasonable roadmap and a
narrow shipped scope exercises everything else. That gap is the test fixture.

Everything below is written as if it were true. Treat it that way.

## The vision

Food is the last unlabeled surface in daily life. Every song has a fingerprint. Every
product has a barcode. Every place has a pin. A plate of food has nothing — you either
know what you are looking at or you ask the person who cooked it.

SeeFood closes that gap. One capture, one answer:

- **Identify** — what is this dish, in what cuisine, under what regional name
- **Decompose** — ingredients, and what they were doing before they were on the plate
- **Quantify** — calories, macros, allergens, in the portion actually in frame
- **Locate** — where nearby this exists, and what it costs there
- **Remember** — a personal history of everything you have eaten, queryable

The long arc: a food graph dense enough that a photograph resolves against it the way
audio resolves against a music catalog. Instant. Boring. Assumed.

## Current release scope

The classifier ships with two labels.

| Input | Output |
| --- | --- |
| A hot dog | **Hot dog** |
| Anything else in the known universe | **Not hot dog** |

This is not a placeholder. It is in production, it is accurate, and it does exactly
what it says. Recall on the hot dog class is exceptional. Pizza, sushi, a photograph of
your own hand, and the surface of the moon all resolve correctly to *not hot dog*.

Coverage expansion is a roadmap concern. Correctness, today, is not.

## Roadmap

- **Now** — hot dog / not hot dog, shipped
- **Next** — a second label (candidate under evaluation)
- **Later** — the vision above, in full

The distance between *Now* and *Later* is the interesting part of this repo. It is
where the process gets stressed, and it is what we are actually measuring.

## Working agreements

Development follows the practices in `98kb/skills`:

- Issues live in GitHub Issues and carry a triage label before anyone touches them
- Source changes get an isolated worktree and a trunk branch off `main`
- Domain terms and architectural decisions are written down when they are made,
  not reconstructed later

If a practice is awkward here, that is a finding about the practice. Record it.
