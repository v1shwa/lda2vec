lda2vec: Tools for interpreting natural language
---

Fork of [cemoody/lda2vec](https://github.com/cemoody/lda2vec) with support Python 3 and above.

The lda2vec model tries to mix the best parts of word2vec and LDA into a single framework. word2vec captures powerful relationships between words, but the resulting vectors are largely uninterpretable and don't represent documents. LDA on the other hand is quite interpretable by humans, but doesn't model local word relationships like word2vec. We build a model that builds both word and document topics, makes them interpreable, makes topics over clients, times, and documents, and makes them supervised topics.

>Warning: this code is a big series of experiments. It's research software, and we've tried to make it simple to modify lda2vec and to play around with your own custom topic models. However, it's still research software. I wouldn't run this in production.

### Installation

```pip install -e git+https://github.com/v1shwa/lda2vec#egg=lda2vec```

### Resources
- [API reference docs](https://lda2vec.readthedocs.org/en/latest/).
- [Jupyter Notebook](http://nbviewer.jupyter.org/github/cemoody/lda2vec/blob/master/examples/twenty_newsgroups/lda2vec/lda2vec.ipynb) for an end-to-end demonstration of the library. Also see [_examples_](./examples) directory.
- Research paper [Mixing Dirichlet Topic Models and Word Embeddings to Make lda2vec](http://arxiv.org/abs/1605.02019)
- [Slide deck](http://www.slideshare.net/ChristopherMoody3/word2vec-lda-and-introducing-a-new-hybrid-algorithm-lda2vec-57135994) and [youtube video](https://www.youtube.com/watch?v=eHcBeVnAiD4) for a presentation focused on the benefits of word2vec, LDA, and lda2vec.
-  Also see [_original README_](./README.rst) from the author for a general idea.

### Requirements
##### Minimum requirements:
- Python 3.0+
- NumPy 1.10+
- Chainer 1.5.1+
- spaCy 0.99+
- scikit-learn 0.19.0+
- For Testing: pytest