[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

# Safecity_BERT-LSTM-LogisticRegression
# SafeCity Data [SafeCity: Understanding Diverse Forms of Sexual Harassment Personal Stories](http://arxiv.org/abs/1809.04739), EMNLP 2018   Authors: Sweta Karlekar &amp; Mohit Bansal, University of North Carolina at Chapel Hill  

# Techniques:
- Method 1 : Extracting 768 Dim vector corresponding to [CLS].
- Method 2 : Extracting 768Dim Vec from last 4 layers corresponding to [CLS] concating them.

![](https://camo.githubusercontent.com/a294fd2ef0f04be622a71bc77afed77041238cd2/68747470733a2f2f6a616c616d6d61722e6769746875622e696f2f696d616765732f64697374696c424552542f64697374696c626572742d626572742d73656e74696d656e742d636c61737369666965722e706e67)



#Refrence: https://jalammar.github.io/

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

![](https://camo.githubusercontent.com/7c092d2fd20a0cd922bdd15a862e31155f6adcb7/68747470733a2f2f6a616c616d6d61722e6769746875622e696f2f696d616765732f64697374696c424552542f626572742d64697374696c626572742d7475746f7269616c2d73656e74656e63652d656d62656464696e672e706e67)
