---
approved_by: Jian-Yang
approved_at: 2026-08-18T02:00:28+05:30
---

# Vision

## Vision Statement

Point your phone at a plate and it tells you the dish — no typing, no account, no internet.

## Customer & Problem

The first person is Erlich Bachman, the roommate. He eats standing up over the sink at 1am and does not know or care what he is eating. The second is the person at a party holding a plate of something they cannot name, who will not ask the host what it is.

What is broken is the same thing in both cases: the only way to find out what is on the plate is to ask a human being. At 1am there is no human being to ask. At the party there is one, and asking him is embarrassing, so the question goes unasked and the food stays unidentified.

The thing being identified is the dish as it sits on the plate — hotdog, not pork and bread and mustard, and not a packaged product on a shelf. Ingredients, calories and where to buy it cheaper are later; the dish is the product.

## Future State

You open the app and the camera is already open. You point the phone at the plate and the phone says the dish. No typing, no account, no waiting.

The answer comes from the phone, not from a server. That means it works in a restaurant basement with no signal, and it means each additional user costs nothing to serve.

Nobody does this today. Shazam does music, and music is finished.

## Grounding Insight

Food recognition is not a model problem. It is a data problem. The models are already good enough, and phone chips are now fast enough to run one on the device itself. The only thing standing between this idea and a working app is labelled pictures.

The corollary, and the reason the build order is what it is: you start where the data is. One food identified correctly beats ten thousand foods identified wrong.

What would make this wrong: if a model trained to identify one food perfectly cannot be extended to a second and a third food without starting over from zero, then the whole plan is wrong.

## Why Us / Why Now

The data exists in one place and it is here. Thousands of hotdog pictures, taken by hand — on a plate, in a hand, at night, close, far. Nobody else has that set, because nobody else took it.

Now is the moment because phones only recently became fast enough to run inference on the device. Doing this two years ago meant a server, and a server means a bill.

And the position: no salary, no cloud bill, no investor, no co-founder. This project can be wrong for two years and it costs nothing. A funded competitor cannot be wrong for two years.

## Vision Pivot Trigger

Two checkable signals, either of which kills this vision:

1. The app names the hotdog correctly and people still open it one time and never open it again. Correct answers with no return use means nobody wanted this.
2. After the hotdog model works, a second food cannot be added without retraining from zero. That breaks the "start where the data is, then repeat" plan the whole vision rests on.
