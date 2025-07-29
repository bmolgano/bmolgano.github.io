---
layout: default
title: Naives Bayes
---


<ul class="nav">
  <li><a href="index.html">Home</a></li>
  <li><a href="introduction.html">Introduction</a></li>
  <li><a href="conclusion.html">Conclusions</a></li>
  <li class="dropdown">
    <a href="dataprep_eda.html" class="dropbtn">DataPrep_EDA</a>
    <div class="dropdown-content">
      <a href="clustering.html">Clustering</a>
      <a href="pca.html">PCA</a>
      <a href="arm.html">ARM</a>
      <a href="naivebayes.html">NaiveBayes</a>
      <a href="dectrees.html">DecTrees</a>
      <a href="svms.html">SVMs</a>
      <a href="regression.html">Regression</a>
      <a href="nn.html">NN</a>
    </div>
  </li>
</ul>

# Naives Bayes

## (a) Overview

Naive Bayes is a type of classifier that uses probability to make predictions. It is based on the Bayes' Theorem, which helps estimate the chance of something happening based 
on known information. The “naive” part refers to the assumption that all input features are independent from each other. Naive Bayes works very well with large datasets. It 
is commonly used in spam filters, document sorting, medical diagnoses, real-time predictions, and credit scoring. The model calculates the probability of each possible outcome
and picks the one with the highest score.

Bernoulli Naive Bayes is a version of this algorithm made for data with only two possible values, like yes/no or 0/1. It is particularly useful for problems where data is 
present or not. For example, if a word appears in a document or not. It uses a Bernoulli distribution and tends to penalize missing expected features more than other versions 
like Multinomial Naive Bayes. This method works best with binary or categorical data. Even though the assumption of independence is not always accurate, Naive Bayes is still 
widely used because it is easy to understand and often effective.

---

## Data Prep

---

## Code


---

## Results

---

# Conclusions
This analysis demonstrates that current patterns of low-value care utilization, combined with payer type, service type, and regional indicators, can serve as a useful proxy 
for identifying regions that may be at risk for future behavioral health service demand. By training a Naive Bayes classifier on this data, the model was able to accurately 
distinguish between regions with high versus low volumes of unnecessary services. The model achieved an overall accuracy of 80%, with balanced precision and recall across 
both categories. This performance suggests that existing claims-based utilization patterns are meaningful signals of regional healthcare behavior and potential system strain.

The ability to classify regions based on current inefficiencies provides a foundation for proactive planning. In particular, regions classified as high-usage may indicate 
underlying issues such as poor access to preventive or coordinated care factors often linked to behavioral health gaps. As Colorado's population continues to grow and shift,
this model could be extended by integrating projected demographic changes to estimate where behavioral health demand is most likely to rise. Ultimately, this work supports a 
data-driven approach to identifying future service needs and informing policy, resource allocation, and system design for mental health care in the state.

---
