# Yesterday's workflow retrospective

2025-11-20

Good morning, pivoteurs!

Yesterday was supposed to be an exercise in time-SAVING, but turned into an exercise of putting-out-fire-after-fire because my model did not match the pivot-pool state.

![All models are wrong, but some are useful ~ George Box](imgs/01-models-useful.png)

Lesson learned: check, and recheck, the model to the pool before executing trades.

Yesterday's work, ending at 3:14 am this morning, took much longer than usual... 'disproving' that automation helps?

Nah. This is all part of the process. I have to iron out the kinks in the system, and it's better to catch them sooner, rather than later.

AND we closed a pivot!

![Moe, Moe, Kyuu!](imgs/02-moe-moe.png)

## Checksum

To this end, that end being 'self-policing,' I've added checksums to the automated recommendations, so that I can quickly check that the internal Rust-model is the same as the active pivots I have on the pivot pool being analyzed.

![Embedded checksums](imgs/03-checksum.png)

Still very manual, but a step toward automation.
