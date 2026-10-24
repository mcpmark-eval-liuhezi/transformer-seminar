# Week 1 Reading — Unit 1 Anchor Paper

- **Title:** Attention Is All You Need
- **Authors:** Vaswani, Shazeer, Parmar, Uszkoreit, Jones, Gomez, Kaiser, Polosukhin (NIPS 2017)
- **arXiv ID:** 1706.03762

## Verified headline results (quoted from the paper source)

- **WMT 2014 English-to-German translation:** **28.4 BLEU** (Transformer big, newstest2014) — a new state-of-the-art, improving over the best previously reported results, *including ensembles*, by more than 2 BLEU. Training took 3.5 days on 8 P100 GPUs.
- **WMT 2014 English-to-French translation:** **41.8 BLEU** (Transformer big, newstest2014) — a new **single-model** state-of-the-art, at a small fraction of the training cost of the best models from the literature.

## Architecture in one line

The Transformer is based solely on attention mechanisms, dispensing with **recurrence and convolutions entirely**, making it more parallelizable and significantly cheaper to train.

## Why these numbers

Both scores are taken directly from the paper's abstract and Table 1 ("Results"), not from secondary sources, per seminar policy: quote benchmark numbers from the paper source only.

## Discussion prompts

1. What does the move to attention-only buy us in parallelism and training cost?
2. Why does the EN-DE result beat ensembles while EN-FR is single-model SOTA?
3. How do positional encodings compensate for the loss of recurrence?
