---
layout: post
title: "Teaching jurors to lie just enough"
excerpt: "Night Debt dev note: wrangling a tiny language model into a spiteful courtroom chorus."
tags:
  - night-debt
  - ai
  - design
---

I needed the jury in Night Debt to sound human, but not fair. The fix: a pocket LLM trained on public trial transcripts and pulp tabloids. It keeps the cadence grounded while still snapping at the player when lies pile up.

Tricks that stuck:

1. **Bias drift on purpose.** I nudge the jury embedding every time the player repeats an argument. The same plea gets colder each round.
2. **Anchor sentences.** Hand-authored opening lines keep the machine from going full technobabble.
3. **Refusal floor.** If the model tries to lecture instead of judge, I clamp the logit and force a verdict.

It’s messy, but the room now feels complicit.
