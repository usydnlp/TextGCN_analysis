# Understanding Graph Convolutional Networks for Text Classification
Official Implementation for AAAI 2022 on DLG
(https://arxiv.org/abs/2203.16060)

<h3>
  <b>Han, C.*, Yuan, Z.*, Wang, K., Long, S., & Poon, J. (2022). <br/><a href="https://arxiv.org/abs/2203.16060">Understanding Graph Convolutional Networks for Text Classification</a><br/>In proceeding of AAAI 2022 on DLG</b></span>
</h3>



## Easy running using .ipynb file
You can simply run the code with your data using `final.ipynb`, remember to fill in your dataset into a list of documents/labels
```python
original_train_sentences = 
original_labels_train = 
original_test_sentences = 
original_labels_test = 

# example 
# original_train_sentences = ['this is sample 1','this is sample 2']
# original_labels_train = ['postive','negative']
# original_test_sentences = ['this is sample 1','this is sample 2']
# original_labels_test = ['postive','negative']
```
Also, some other parameters can be modified
```python

# EDGE: 0 means only d2w edge, 1 means d2w+w2w, 2 means d2w+w2w+d2d edge
EDGE = 0

# NODE: 0 means one-hot as input, 1 means BERT embedding as input
NODE = 0 

NUM_LAYERS = 2 
HIDDEN_DIM = 200
DROP_OUT = 0.5
LR = 0.02
WEIGHT_DECAY = 0
EARLY_STOPPING = 10
NUM_EPOCHS = 200
```
