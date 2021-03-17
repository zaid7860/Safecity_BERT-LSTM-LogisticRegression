[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

# Safecity_BERT-LSTM-LogisticRegression
# SafeCity Data [SafeCity: Understanding Diverse Forms of Sexual Harassment Personal Stories](http://arxiv.org/abs/1809.04739), EMNLP 2018   Authors: Sweta Karlekar &amp; Mohit Bansal, University of North Carolina at Chapel Hill  

# Techniques:
- Method 1 : Extracting 768 Dim vector corresponding to [CLS].
- Method 2 : Extracting 768Dim Vec from last 4 layers corresponding to [CLS] concating them.


![https://camo.githubusercontent.com/0c9b76326c1d9bd7d001a3cdac1837b6b4c6b9e8/68747470733a2f2f6a616c616d6d61722e6769746875622e696f2f696d616765732f64697374696c424552542f626572742d64697374696c626572742d73656e74656e63652d636c617373696669636174696f6e2e706e67]




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
