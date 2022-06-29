# Using BERT for Joint Sentence Classification in Medical Paper Abstracts

 Millions of scholarly biomedical articles have been published. Each year this number keeps on increasing. It will be easier for reaserchers if these reports are well structured. But unfortunately, many of them are unstructured.
 
 Through this model, I aim to classify sentences from report into "BACKGROUND", "OBJECTIVE", "METHODS", "RESULTS" and "CONCLUSIONS".
 
 I fine tune Bert-base-uncased model with classification head for this task and able to achieve 87% of accuracy.
 
 ## Motivation
 
 I wanted to utilize power of BERT to do some real life application. I stumbled upon paper called "Neural Networks for Joint Sentence Classification
in Medical Paper Abstracts". This paper utilized Bi-LSTM and positional embedding to acheive this task. This paper intrigued me as it was real life application and utilized my knowledge. Unlike this paper, I decided to finetune BERT for the given task.
 
 ## Technical Aspect
 
 1. BERT-base-uncased model is finetuned for 3 epochs. Huggingface library is used to achieve this.
 2. PubMed 200k RCT dataset introduced in paper "PubMed 200k RCT: a Dataset for Sequential Sentence Classification in Medical Abstracts", https://arxiv.org/pdf/1710.06071.pdf is used as train and test dataset. Only 20K data is used.
 
 ## Directory and files
 
 1. Skimlit_with_BERT.ipynb
 
 -> This is a main notebook of this project. Through this project I explore this dataset and perform various Exploratory Data Analysis. In the same notebook I finetune bert and save the model.
 
 2. Skimlit
 
 -> Deployment of model using django.
 
