
---
title: "Chest X-Ray Images (Pneumonia)"
excerpt: "Help Early Diagnosis of Pneumonia<br/><img src='/images/Screen Shot 2021-10-24 at 5.34.57 PM.png'>"
collection: portfolio
---
<br/><img src='/images/Screen Shot 2021-10-24 at 5.34.57 PM.png'><br/>
Machine Learning and Deep Learning have a huge scope in healthcare but applying them in healthcare isn't that simple.
<br/>
Pneumonia is an inflammatory condition of the lung affecting primarily the small air sacs known as alveoli. Symptoms typically include some combination of productive or dry cough, chest pain, fever and difficulty breathing. The severity of the condition is variable. 
<br/><br/>
It can be either: 1) Bacterial pneumonia 2) Viral Pneumonia 3) Mycoplasma pneumonia and 4) Fungal pneumonia. This dataset consists pneumonia samples belonging to the first two classes. The dataset consists of only very few samples and that too unbalanced. The aim of this project is to develop a robust deep learning model from scratch on this limited amount of data to predict whether an X-ray scan shows presence of pneumonia. This is especially useful during these current times as COVID-19 is known to cause pneumonia.
<br/>

<img src='/images/Screen Shot 2021-10-24 at 5.38.48 PM.png'><br/>

**Figure 1: Overview of the Dataset**
<br/>
The dataset consists of 5,863 X-Ray images and 2 categories (Pneumonia/Normal). Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care. For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.
<img src='/images/Screen Shot 2021-10-24 at 5.43.22 PM.png'><br/>
**Figure 2: Building Convolutional Neural Network (CNN) – Residual Learning**
<br/>
CNN is the standard in performing image classification task. We used ResNet which is a type of CNN with residual learning feature that allows the learning weights propagate better to the deeper layers of the neural network. 
<br/><img src='/images/Screen Shot 2021-10-24 at 5.43.29 PM.png'><br/>
**Figure 3: Model Evaluation**
<br/>
Confusion matrix is calculated by applying the completed CNN model to an independent test set comprised on X-ray images unseen during the training process. Precision and recall are the two metrics used to evaluation the model. 
<br/>

**What does it do?** 
<br/>
The model determines whether or not a patient has pneumonia based on their X-Ray pictures.
Clinicians at the radiology department could use the model to assist them in pneumonia diagnosis.
<br/>

**How do I evaluate the project’s success?** 
<br/>
I would monitor the results and receive feedbacks from clinicians and ask if those who were correctly diagnosed with pneumonia were aided with the assist of my model. 
<br/>

**What did I learn from this project** 
<br/>
I learned how common it is for people to get contract pneumonia as over a million people are diagnosed each year. However, such a disease is hard to diagnose as the symptoms of coughing, fever, and chest discomfort is very synonymous with that of the flu or the common cold. Therefore, it was imperative to find other easier solutions to accurately diagnose diseases like pneumonia, like so using X-Rays.
<br/>

**What’s next for this project**
<br/>
This pneumonia diagnostic tool is developed using a dataset with limited cohort from Guangzhou, China. For expanded usage of this tool, we need to build a diagnostic model that covers various race and gender. Once this pneumonia diagnostic tool gains credible reputation, the medical staffs can use this tool to not only diagnose pneumonia, but also assist doctors in confirming such diagnostics retrospectively for quality control purpose.
<br/><img src='/images/Screen Shot 2021-10-24 at 5.45.20 PM.png'><br/>

