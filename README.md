# Microsoft-Malware-Prediction

## Introduction
The entire world today runs on computers. Even traditionally non-technology fields like farming have an at least a part of the work being done by computers. This reliance means that unethical attacks on computers could cripple the world. This is an area where there is a lot of research being conducted. Most anti-malware applications today run on a single principle i.e. they scan the computer for the presence of any suspicious files or programs and then get rid of them. This is a reactive approach where no action is taken until the malware has already infiltrated the system. This is not an ideal way to deal with malware as it is possible that the files/programs may start causing damage as soon as they enter a computer. The next generation of anti-virus software needs to be smarter. A way to do this could be to take stock of the current conditions of the machine and then check if these conditions make it likelier to be infected and secure the system before the attack instead of after it. Our project aims to use data science and analysis to help determine what conditions make a computer vulnerable to attacks. The insights could help technology companies make better antivirus software as well as design more robust operating systems that can withstand malware.

## Goals
1.	Gather data and understand the feature space
  Tasks: 
    a.	Collect data- The data for this project will be used from a competition on Kaggle headed by Microsoft[1].
    b.	Understand data- Understand the features present in the data to know what parameters are being considered while determining the     result.
  Results: Data is collected and a rudimentary understanding is gained.
  Expected problems: The terminology used in the data could be difficult to understand and may need further reading in cybersecurity
2.	Clean and explore the data and decide the final features to work with
  Tasks: 
    a.	Explore features: clean data to get rid of missing values and other noise and perform numeric and graphical explorations on the features to decide what features are strong and weak and then make a list of the final features to work with
  Results: A final dataset is generated which can be used for modelling
  Expected problems: The data may have a lot of missing values. Removing them would mean losing a lot of data. So other methods must be explored.

3.	Use models to generate insights and predict on test data
  Tasks: 
    a.	Create following models:
      - Logistic Regression
      - Random Forests
      - Gradient boosted trees

    b.	Reduce the error rate to represent the data as accurately as possible.
    c.	Draw inferences from the different models.
  Results: A number of models will be generated and the error rates should be compared to find the best model
  Expected problems: The models may not be very good or they may be overfitting to the train data. This can be avoided by cross-validating the models and reconstructing the feature space to see what features describe the data the best.

4.	Consolidate the inferences to generate the final list of operating systems and anti-malware software that can help secure a system.
 Tasks:
      a.	Analyze the generated inferences to understand the types/versions of OS that are most vulnerable to attacks and anti-malware             software that is inefficient.
      b.	Analyze the generated inferences to determine the best combination of OS and anti-malware that can make a system secure.
 Results: Better understanding will be achieved by determining combinations of OS and anti-malware that make a system secure and how to            reduce the malware attacks in vulnerable systems.
  Expected problems: Combinations generated may be too similar to one another and thus may reduce the effectiveness of the solutions.

## Dataset
[1] Microsoft Malware Prediction: https://www.kaggle.com/c/microsoft-malware-prediction/data


## Tools 
spark ML, python, pyspark, numpy, matplotlib, pandas etc.

## Models
Logistic Regression, Random Forests, Gradient boosted trees

## Evaluation
AUC, cross validation
