---
title: "What Does a CNN See"
excerpt: "Model Interpretability<br/><img src='/images/Screen Shot 2021-10-29 at 2.10.08 PM.png'>"
collection: portfolio
---

<img src='/images/Screen Shot 2021-10-29 at 2.10.08 PM.png'><br/>

Machine learning models, especially Deep Learning models are often considered as a black box and hard to interpret. Well, this statement is neither completely true not it is completely false. It is a fact that debugging a deep learning model is way harder than other machine learning models but there are ways by which you can get insights about your model and to an extent, you can see what is happening.
<br/>

When you have limited data, deep models don't do very well. Deep learning models are data hungry. The more data you provide to a deep learning model, the more it performance improves (until unless your algorithm has reached a limit). This is where data augmentation really comes handy. We will be using imgaug, a very powerful library for augmenting our images. We will define a sequence of augmentations and for each image, one of these augmentations will be applied to the image during training
<br/>

<img src='/images/Screen Shot 2021-10-29 at 2.12.19 PM.png'>
<br/>

**Figure 1: Gradient-weighted Class Activation Mapping (Grad-CAM) Visual Explanations from Deep Networks via Gradient-based Localization**
<br/>
Now starts the most important part. How do we explain the output of our model? For example, given an image, what does the network consider important when classifying the image? Can we get info about it? Can we make our model a little grey box? 
<br/>

Answering the above question is a bit difficult. Although there have been many advancements in explaining the activations/outputs of a neural network, for example, check this, a lot more has to be done in this direction.
<br/>

Here, we will explore two methods that are very simple to use and can give some good insights about model predictions. These are:
<br/>

Visualizing the intermediate layers outputs
Class Activation Mapping
Here are all the steps we are going to do:
<br/>

We will start by selecting all the layers up to last convolution block in VGG16, excluding the Input layer.
<br/>

Define a new model, vis_model, that takes the same input as our model's input but outputs activations of all the intermediate layers we have selected. This will be used for displaying all the activation maps of each convolution block for any sample image from our validation data. 
<br/>

For CAM, we will take the same sample image and get the output of the last convolution layer. We also compute the gradients for this layer which we will use to generate a heatmap. 
<br/>

<img src='/images/Screen Shot 2021-10-29 at 2.26.12 PM.png'>
<br/>

**Figure 2: Model Evaluation**
Confusion matrix is calculated by applying the completed CNN model to an independent test set comprised on 10 monkey species with 5,000 independent images.
<br/>

**What does it do?**
<br/>
The model determines which species a monkey is when shown a picture of a random monkey. Can be used by zoo keepers to keep in check of the specific monkey species.
<br/>

**How do I evaluate the project’s success?**
<br/>
Test to see if the model is able to correctly label the accurate species of a shown picture of a monkey. 
<br/>

**What did I learn from this project?**
<br/>
I learned how diverse monkeys are in general as there are many such species around the world. Even with the ten species that are tested for this dataset, there were hundreds and thousands of different pictures available for testing. Therefore, it was interesting and cool to find an easy solution to correctly find the right species of monkey.
<br/>

**What’s next for this project?**
<br/>
This model can be extended for far more beyond the only ten monkeys available for testing. As there are around 260 types of monkeys in the world, it would be very cool to have a model to differentiate between every single species.
<br/>
