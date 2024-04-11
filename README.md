## What is DESY?

DESY is one of the world's leading accelerator centres. The accelerators as well as the detection instruments that DESY develops and builds are unique tools for research: they generate the strongest X-ray light in the world, bring particles to record energies and open completely new windows into the universe. 

I was selected for DESY summer program 2021.
[DESY summer program](https://summerstudents.desy.de/)

This repository contains the work that I have done for DESY summer program 2021. 

## :woman_scientist: Project Abstract

Developed and implemented a robust Anomaly Detection algorithm to identify system failures within the dCache system at DESY. In order to construct this algorithm, I embarked on a comprehensive data collection process, gathering approximately 10TB of transfer and telemetry data from the archived dCache system. Leveraging the powerful capabilities of the pyspark module, I transformed and preprocessed the data to ensure its suitability for analysis.

Utilizing this transformed dataset, I constructed a basic yet effective logistic regression algorithm. Through rigorous testing and fine-tuning, the algorithm demonstrated an impressive accuracy rate of 85% in detecting system failures. This accomplishment not only enabled proactive identification of potential issues but also facilitated prompt resolution and preventive measures.

## What is dCache?

Built in Java, dCache is a distributed mass-storage system that allows us to manage huge ammount of scientific data. The data are distributed among the large number of heterogenous pools(nodes) that handle with data storage and transfer. 

## How we dealt with Big Data?

Since, dCache stores scientific data, it stores a huge amount of Data which has to be processed using distributed systems. For that purpose we used Spark.

![Apache spark logo](/images/spark.png)

## Methodology and results

We had 2 classes to distinguish - signal(correct transaction) and background(wrong transaction), we had to use a classification model for our problem. So, we used Logistic regression.

We got an accuracy score of 85% and auc of 0.90.

![auc](/images/auc.png)
