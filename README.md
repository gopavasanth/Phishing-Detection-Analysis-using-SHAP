# ICSML 2019 Course Final Project Report

Data Mining and Business Intelligence with its applications in Cyber Security


# Analysis of Phishing Detection using SHAP

## Abstract

Phishing is a form of fraud in which the attacker tries to learn sensitive information such as login credentials or account information by sending as a reputable entity or person in email or other communication channels.

SHAP is A unified approach to explain the output of any machine learning model.
 
Our aim is to perform an analysis of the Phishing Detection project to bring the most important features which are contributing to the different results.

## Problem Statement

Build a system which helps in explaining why some domains are malicious. There are 549 features for each URL to estimate whether the URL is malicious or benign. Our goal is to perform an analysis using SHAP and pick up the most important features contributing to the URL is malicious.

## Dataset and Models

We have received the dataset which is a huge collection of public data-sets of fishing domains and model (pre-trained XGBoost model for phishing domain classification) from Shai Cohen. The dataset consists of 6166033 rows × 551 columns, where 549 are the features. 

## Why SHAP?

SHAP (SHapley Additive exPlanations) is a unified approach to explain the output of any machine learning model. SHAP connects game theory with local explanations, uniting several previous methods [1-7] and representing the only possible consistent and locally accurate additive feature attribution method based on expectations.

## Solution Approach

We performed an analysis of the whole dataset and the model. But according to our guide suggestions, we changed our plan.

The main motive is to detect the features responsible for classifying benign URLs as Malicious. It means we need FP (false-positive) dataset. Adding to this we want to add one more feature to this project, detect the features responsible for classifying the malicious URLs are classified as benign. This means we need the FN (false-negative) dataset.

True Positive (TP) : If the instance is positive and it is classified as positive
False Negative (FN): If the instance is positive but it is classified as negative
True Negative (TN) : If the instance is negative and it is classified as negative
False Positive (FP): If the instance is negative but it is classified as positive

We got the FP and FN dataset and we performed the analysis.

## Team Members

1. [Gopa Vasanth](https://github.com/gopavasanth)
2. [Venu Vardhan Reddy Tekula](https://github.com/vchrombie)
3. [Chejarla Santhosh Kumar](https://github.com/chsantoshkumar211)

