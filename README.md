# Text-Classification-With-Deep-Learning
Implementation of text classifiers using various Deep Learning Algorithms 

## Table of Contents
  - [Text Classifiers](#Text-Classifiers)
    - [Text Classification with BERT](#text-classification-BERT)
    - [Text Classification with LongFormer](#adjust-tab-space)
    

## Text Classifiers

Text classification is a techniquie in deep learning where the model is trained on a dataset to figure out unique patterns in the text which helps in classifying the given text to its correct label or class. In this series, I will try to implement different types of Deep Learning Models which are used for text classification.

### Text Classification with BERT

BERT(Bidirectional Encoder Representation from Transformer) is a variant of Transformer model which has two encoders so that it has the ability to encode the text from both the directions to get the better contextual representation of Text. BERT was introduced in october 2018 and took the NLP community by storm as it achieved state of the art techniques in varios NLP Tasks like Sentiment classification, Machine Translation, Question Answering to name a few. Kindly go through the paper (https://arxiv.org/abs/1810.04805) to learn more about the architecture of BERT. Here we will finetune the pretrained BERT model on a small dataset to detect author of a given article, due to confidentiality I will not be able to share the dataset but this model can be used for any sort of text classification task.

### Text Classification with LongFormer

To use LongFormer one should have the understading of how transformer works. In the previous section we implemented text classification with BERT though it has capability to provide very good accuracy but one major drawback of the BERT is that it can only process 512 tokens, so if we are working on a long passage we have to split the passage and by doing this we may lose important information which might not give us the best accuracy and hence we should use LongFormer Model instead. The LongFormer's attention mechanism is a drop in replacement for the standard self-attention and combines a local windowed attention with a task motivated global attention due to which it has the capability to process larger text. LongFormer achieved state of the art accuracy on datasets like text8 and enwiki8. Kindly go through Longformer paper (https://arxiv.org/pdf/2004.05150.pdf) to understand more about LongFormer. Here we will use the LongFormer model on the same dataset for text classification. 
