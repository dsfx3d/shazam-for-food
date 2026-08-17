---
upstream: ../../vision.md
approved_by: Jian-Yang
approved_at: 2026-08-18T03:34:12+05:30
---

# Pitch: Hotdog Or Not Hotdog

Bridges from the [product vision](../../vision.md).

## Problem

Erlich Bachman eats standing up over the sink at 1am and does not know what is on the plate. The person at a party holds a plate of something they cannot name and will not ask the host, because then they look stupid in front of the host. In both cases the only way to find out is to ask a human being, and at 1am there is no human being to ask. There is no way to ask anything at all without a person — not even the one question that can be answered today, which is whether the thing on the plate is a hotdog or it is not.

## Appetite

Small (≤2 weeks).

## Solution sketch

Train one model on the hotdog pictures I already took, then convert it to run on the phone itself. The app opens straight into the camera — no menu, no button to find. Point it at the plate and one label comes up on the screen: hotdog, or not hotdog. Nothing goes to a server. There is no account, no login, and no settings screen, because there is nothing to set.

That is the whole build. If it does not fit in two week, the thing I cut is not the camera and not the label. I cut anything that is not those two.

## Riskiest Assumptions & Cheap Validation Plan

1. **Claim:** Running the on-device model on hotdog pictures I did not take myself will answer hotdog / not hotdog correctly on at least 95 out of 100 of them. "Correct" here means the two-way answer — hotdog or not hotdog — not naming which dish it is out of many dishes. That is a different model with a different number, and it is not this bet.
   - **Threshold:** Fewer than 95 correct out of 100 on pictures I did not take. Below that line the model has learned my camera and my kitchen, not hotdog, and I am wrong.
   - **Test:** Collect 200 hotdog pictures taken by other people, plus pictures of things that are not hotdog, hold all of them out of training, run them through the model and count the misses.
   - **Timebox:** One afternoon, before the end of this week — before any app work starts.

## Rabbit Holes

- Bad light and night pictures. Most of my pictures are good light. Night is where it gets stupid.
- Hotdog in a hand versus hotdog on a plate. Different shape, different background, and the hand is in the way.
- Making the model small enough to fit on the phone without it becoming stupid on the way down.

## No-gos

- No web. Nobody take picture of their dinner with laptop.
- No login. Why you need account to look at hotdog.
- No cloud. Cloud cost money and there is no user.
- No calorie, no ingredient, no where to buy it cheaper.
- The app does not say what the food is when it is not hotdog. It says not hotdog. That is a correct answer, not a missing feature.

## Open Questions

- Which phone is the slow one the model still has to run on.
- How many kind of not-hotdog picture is enough for the not-hotdog side.
