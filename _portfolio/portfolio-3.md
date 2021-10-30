---
title: "Sentiment Analysis on Movie Reviews"
excerpt: "Application of roBERTa encoder with LSTM model<br/><img src='/images/Screen Shot 2021-10-29 at 2.45.42 PM.png'>"
collection: portfolio
---

<img src='/images/Screen Shot 2021-10-29 at 2.45.42 PM.png'><br/>

**Background**
<br/>
The Rotten Tomatoes movie review dataset is a corpus of movie reviews used for sentiment analysis, originally collected by Pang and Lee. In their work on sentiment treebanks, Socher et al.  used Amazon's Mechanical Turk to create fine-grained labels for all parsed phrases in the corpus. This competition presents a chance to benchmark your sentiment-analysis ideas on the Rotten Tomatoes dataset. You are asked to label phrases on a scale of five values: negative, somewhat negative, neutral, somewhat positive, positive. Obstacles like sentence negation, sarcasm, terseness, language ambiguity, and many others make this task very challenging.
<br/>

<img src='/images/Screen Shot 2021-10-29 at 2.49.06 PM.png'><br/>

**Figure 1: roBERTa encoder to preprocess text; LSTM model to output sentiment classification.**
<br/>
roBERTa is a robustly optimized method for pretraining natural language processing (NLP) systems that improves on Bidirectional Encoder Representations from Transformers, or BERT, the self-supervised method released by Google in 2018. RoBERTa builds on BERT’s language masking strategy, wherein the system learns to predict intentionally hidden sections of text within otherwise unannotated language examples. RoBERTa, which was implemented in PyTorch, modifies key hyperparameters in BERT, including removing BERT’s next-sentence pretraining objective, and training with much larger mini-batches and learning rates. This allows RoBERTa to improve on the masked language modeling objective compared with BERT and leads to better downstream task performance.  
<br/>

Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) architecture.  Relative insensitivity to gap length is an advantage of LSTM over other typical RNNs.
<br/>

<img src='/images/Screen Shot 2021-10-29 at 2.50.58 PM.png'><br/>

**Figure 2: Model evaluation**
<br/>
The model is evaluated on classification accuracy (the percent of labels that are predicted correctly) for every parsed phrase. The sentiment labels are:
<br/>
**0** - negative
<br/>
**1** - somewhat negative
<br/>
**2** - neutral
<br/>
**3** - somewhat positive
<br/>
**4** - positive
<br/>

**What does it do?**
<br/>
The model determines the sentimental value of movie reviews from Rotten Tomatoes from the written comments from users.
<br/><br/>
**How do I evaluate the project’s success?**
<br/>
We can evaluate how accurate the sentiment values are from the movie reviews that the user has posted online. 
<br/><br/>
**What did I learn from this project?**
<br/>
I learned how open-ended such movie reviews are and the diversity between the tone and the meanings behind each movie review. Being able to truly interpret a review is important before one watches a movie due to possible underlying messages behind it. So having a model that confirms the sentiment of a review is beneficial.
<br/><br/>
**What’s next for this project?**
<br/>
Moving from movie reviews to other forms of reviews like restaurants, tourist attractions, malls, etc. can also help people who never had experience be able to truly know if it is worth their time to visit a place.
<br/><br/>

