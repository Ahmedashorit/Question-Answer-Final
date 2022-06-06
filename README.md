# Question Answering with SQuAD using BERT,RoBERTa,DeBERTa models

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fgjbae1212%2Fhit-counter&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
Implemented a Bidirectional encoder representations from transformers as a baseline.

### Optimizing parameters and investigation of sensitivity in the datasets and using the selected model.
### Add new two layers to existing model and train the data and measure the accuracy with this adding.
 
# Requirements
PyTorch 1.11
Python 3.7
RAM 30
CPU 16
you can use paperspace.com to rent VM for runing your code

# Model Architecture

![This is an image](https://github.com/Ahmedashorit/Question-Answer-Final/blob/main/Code/images/BERT%20Architecture.jpg)


[Source](https://arxiv.org/abs/1810.04805)


# Adding 2 layers to BERT and RoBERTa

![This is an image](https://github.com/Ahmedashorit/Question-Answer-Final/blob/main/Code/images/Advanced-model.png)

Sample from SQuAD 1.1

![This is an image](https://github.com/Ahmedashorit/Question-Answer-Final/blob/main/Code/images/SQuAD%20sample%20of%20data.png)

# Code Organization

├── run_squad.py
<--- main program, create dataset (tokenization and encode), 
create dataloader, load pretrained model, train model, evaluate model

├── trainer_qa.py
<--- Training engine

├── utils_qa.py
<--- Decode prediction, preprocess prediction

├── Advanced_models.py  
<--- Advanced model architecures

├── run_qa_advanced.py  
<---  main program, create dataset (tokenization and encode), create dataloader, load pretrained model, train advanced model, evaluate advanced model

# Results

![This is an image](https://github.com/Ahmedashorit/Question-Answer-Final/blob/main/Code/images/result.jpg)

Exact-Match and F1 Score on Validation set after training:

EM	F1
85.30%  91.85  

# Useful Articles

SQuAD: 100,000+ Questions for Machine Comprehension of Text, 2016: https://arxiv.org/pdf/1606.05250.pdf

Know What You Don’t Know: Unanswerable Questions for SQuAD, 2018: https://arxiv.org/pdf/1806.03822.pdf

BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding https://arxiv.org/abs/1810.04805

RoBERTa: A Robustly Optimized BERT Pretraining Approach https://arxiv.org/abs/1907.11692

DeBERTa: Decoding-Enhanced BERT with Disentangled Attention

https://www.microsoft.com/en-us/research/publication/deberta-decoding-enhanced-bert-with-disentangled-attention-2/

Pytorch Tip: Yielding Image Sizes https://medium.com/@yvanscher/pytorch-tip-yielding-image-sizes-6a776eb4115b
