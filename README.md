# Skim-Lit

In this project we implement a deep NLP model to make reading medical abstracts easier. The model is mostly based on the one described in [this article](https://arxiv.org/pdf/1612.05251.pdf).

The data was made publicly available by the authors and, for this project, we only use 10% of their original dataset. This allows to greatly reduce computing times.

The model has three components:

- A token-level model.
- A character-level model.
- Two positional models: the first one for the line number within the abstract and the second one for the total number of lines in the abstract.

When trained on the subset of 20k abstracts, the model achives an f-score of 87%, which is close to the 90% reported by the authors of the article.

## Dependencies

The project is a single Jupyter Notebook file (skim-lit.ipynb) and depends on a few libraries:

* `numpy` and `pandas` for data manipulation.
* `tensorflow` for deep learning.
* `sklearn` for computing performance metrics.
* `matplotlib` for the visualizations.
