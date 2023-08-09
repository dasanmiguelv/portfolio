---
title: "Behaviour Buying for BRITISH AIRWAYS"
description: "Analysis behaviour buying for BRITISH AIRWAYS !"
dateString: Jul 2023
draft: false
tags: ["Python", "Machine Learning", "Data Science", "Data Visualisation"]
showToc: false
weight: 202
cover:
    image: "projects/BA_behaviour-buying/booking.jpg"
--- 
### 🔗 [View code on Github](https://github.com/dasanmiguelv/clustering)

## Description
This project is part of a program created by **Forage** that seeks to create connections between the largest companies and candidates who lack these connections.
These programs are certified, you can consult it **[here](https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/British%20Airways/NjynCWzGSaWXQCxSX_British%20Airways_HMn4kpBMPRFe6rGnf_1691544594630_completion_certificate.pdf).**

This time, I had the opportunity to step into the shoes of a **British Airways** team member and complete tasks that replicate the work that the Data Science team does every day in British Airways.


The main objective was to build a predictive model that would allow us to evaluate how each variable contributes to the power of the model and determine if we could use them in a feasible way to predict future results about our purchasing behavior customers.

These data were provided by the program and are available to those interested in developing this type of task through the program.
The data include characteristics specific to the booking of a flight or vacation.
First, I pre-processed the data using automation tools like ydataprofiling to get a complete overview of the EDA.

Once the data was pre-processed, we went on to train the model, using a random forest model which was evaluated using cross-validation techniques and evaluation metrics.

As a result of the implementation of the model, an accuracy of 85% was obtained and the company was informed which of the characteristics of the data were most important to obtain these reuses, in turn, recommendations were delivered on features that are not as relevant and could be evaluated to improve the quality of service.