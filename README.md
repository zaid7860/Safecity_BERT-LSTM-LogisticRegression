[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

# Safecity_BERT-LogisticRegression
# SafeCity Data [SafeCity: Understanding Diverse Forms of Sexual Harassment Personal Stories](http://arxiv.org/abs/1809.04739), EMNLP 2018   Authors: Sweta Karlekar &amp; Mohit Bansal, University of North Carolina at Chapel Hill  


## Citation
The dataset has been taken from this phenominal paper(http://arxiv.org/abs/1809.04739).


# Requirements:
- Huggingface pipeline
- Numpy
- Sklearn LR 
- Pandas

# Explain:
- Extracted emeddings from bert using huggingface pipeline for feature extration
- out of many vectors corresponding to the tokens, we need to look particular for 768 dim vector associated with [CLS] which is always at 0th position in the sequence of sentence.
- after exracting the vectors just applied normal logestic regression 
