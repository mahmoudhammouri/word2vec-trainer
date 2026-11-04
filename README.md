# Word2Vec Trainer — how an embedding model is trained

An interactive teaching app that shows, step by step, how Word2Vec learns word embeddings
with **Skip-gram** and **CBOW**.

**Live demo:** `https://mahmoudhammouri.github.io/word2vec-trainer/`

## The 7 pages
1. **Sentences** – the training corpus and pre-processing (stop words).
2. **Vocabulary** – word IDs and one-hot vectors.
3. **Training pairs** – watch the sliding window create the training pairs.
4. **Settings** – method, vector dimensions, window size, learning rate, epochs.
5. **Train step by step** – the neural network and the five phases of one training step
   (window → hidden layer → softmax → error & loss → weight update).
6. **Weights = vectors** – the weight matrices; each row of W_in is a word's embedding.
7. **Vector space** – words as points, cosine similarity, and the loss curve.

Use the **Skip-gram | CBOW** switch at the top right to compare the two methods.
Direct links to a page work, e.g. `.../#3` opens the sliding-window page.

## Run it
It is a single self-contained `index.html` — no installation, no build, no internet needed.
Open it in any browser, or host it with GitHub Pages:
Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.

## Notes
A small teaching implementation: full softmax and plain stochastic gradient descent
(no negative sampling), so it is meant for small vocabularies.

Course: AI Agent Development — The Hope International.
