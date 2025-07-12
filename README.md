# Self-supervised evaluation of (L-)LDA-based clustering of word forms

This repository contains data and Jupyter Notebook to analyze it developed for my presentation at the 42nd Annual Meeting of the Japan Cognitive Science Society.

The idea behind this research is the need for a more realistic reinterpretation of “topics” in topic models such as LDA and Labeled LDA. Specifically, my point is that “topics” in topic models are not semantic in nature despite its name. I proved this by the following reduction to absurdity:

1. Build a topic model (such as LDA) of word forms (as documents) using their character n-grams (as terms).
2. Classify word forms for their language names using the topic model under self-supervision (class of classification is names of language).
3. If classification is successful, this means either character $n$-grams have meaning of their own (possibility A), or topics are not semantic (possibility B).
4. Even if possibility A cannot be theretically impossible, possibility B is far more likely. (If possibility A is correct, we should be able to describe what character n-grams mean, but who can do that?)

# Jupyter Notebook

- [Jupyter Notebook](classify-words-under-self-supervision.ipynb)

Run was checked on Python 3.10, 3.11 and 3.12.

# Data

- [Data (spell)](data-words-1k-most-common/)
- [Data (sound)](data-words-opendict-ipa/)

# Results

- [Result](results/)
- [Plots](plots/)