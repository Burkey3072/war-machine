# War Machine

This repository was created for a semester project in Michigan State University's CMSE 202, Computational Modeling Tools and Techniques during the Fall of 2024 taught by Dr. Nathan Haut at the Department of Computational Mathematics, Science, and Engineering. This project comes under the social sciences.

## Group members:

1. Kyle Cowden (Graph Theory)
2. Lowell Monis (Machine Learning)
3. Joseph Burke (Data Processing and Graph Theory)
4. Saif Sheikh (Machine Learning and Visualization)
5. Adhvik Kolar (Machine Learning and Visualization)

## Runtime:

The primary code used to generate plots of how accurate our war predictions are is in the `graph theory-isolated portion.ipynb` file. This file contains our primary submission for this project. You can also find code for making graphics and simulations of how alliances change in our raw data in `archive/Correlates_of_war.ipynb`, `archive/svm.ipynb` contains an exploratory attempt at using SVMs alone to predict alliance changes, but is not used in the main simulation that we present.

## Abstract

Our project focuses on modeling and predicting international alliances and the likelihood of conflict using the Correlates of War (CoW) datasets. This work integrates computational modeling, data analysis, and machine learning to answer the following central question: 

>How do alliance configurations shift over time?
>Thus, when will war break out?
>What factors in alliances historically correlate with wars?
>Can graph theory and machine learning models predict alliance instability?

These questions are motivated by the need to better understand the dynamic nature of global alliances and the conditions under which conflict arises, contributing to the broader field of political science, international relations, and social relations.

### Background and Motivation

The CoW datasets provide a comprehensive archive of historical and contemporary data on interstate conflicts, alliances, trade, and diplomatic exchanges. Leveraging this dataset allows us to analyze how various factors influence alliance stability and the onset of conflict. Our motivation lies in advancing predictive capabilities using computational tools and exploring the theoretical implications of alliance dynamics through graph theory and machine learning.

**Objectives of this study**:

- Understand stable alliance configurations using graph theory principles.
- Use these configurations to predict war likelihood.


### Methodology

We employed a multi-faceted approach combining graph theory, and machine learning. The first phase involved constructing network graphs where nodes represented countries and edges depicted alliances. We implemented graph-theoretical stability rules to identify two configurations: complete graphs, which signify stable alliances, and disjoint subgraphs, which often predict conflict. For the second phase, we utilized Python-based libraries such as `NetworkX` for graph analysis, `pandas` for data processing, and `sklearn` for machine learning. We chose logistic regression to simplify the model. It was also chosen for its interpretability and effectiveness in binary classification tasks like predicting war likelihood and alliance shifts.

The logistic model is based on the logistic function, also known as the sigmoid function.

$$f:\mathbb{R}\rightarrow[-1,1], f(x) = \frac{e^x}{1+e^x}$$

This makes it great to use as a binary classifier by using the probabilistic concept of likelihood.

Graph theory was used as a medium for this project. Nodes were used to represent states, while edges were used to represent relationships or alliances. For the sake of simplicity, the lack of an edge indicates hostility. Relationships were assumed to be bi-directional, which removed the need to create directed graphs.

There were a few rules set up for the sake of stability.

1. Allies cannot share a mutual enemy.
2. Alliances must form; no isolated nodes are allowed.

From these rules, two stable configurations were achieved:

1. Complete Graph ($K_n$: All states are allies.
2. Disjoint Complete Subgraphs: States form two or more distinct alliances with hostility between the groups, making war inevitable.

Returning to computational techniques used, we used the following libraries and tools:

1. `NetworkX': For constructing and analyzing graphs, particularly for stability analysis.
2. `Pandas` and `Numpy`: For data processing and manipulation.
3. `SKLearn`: For building machine learning models to predict the likelihood of war based on alliances and graph properties.

This is a brief timeline of the steps followed to complete this project.






### Data Source

In this study, the Correlates of War (COW) Datasets were used. In particular, we used Version 4 of the Alliance Data, which has data of all defense, entente, and non-aggression alliance agreements from 1860 to 2007. The scope of this project entails data from 1860 to 1918, i.e., until the First World War. The data is publicly available and widely recognized in international relations research. There are a few quirks in the data set that reduce its perceived rating on data science websites like Kaggle which we will explore in this study. The data was pre-processed to filter relevant alliances, convert dates into numeric formats, and handle missing or incomplete data.

### Results

### Discussion

### Conclusion



## References

[1] Rai, Khushwant (2020). The math behind Logistic Regression. Accessed on Novermber 16, 2024 from https://medium.com/analytics-vidhya/the-math-behind-logistic-regression-c2f04ca27bca
[2] COW War Data, 1816 – 2007 (v4.0): Sarkees, Meredith Reid and Frank Wayman (2010). Resort to War: 1816 – 2007. Washington DC: CQ Press. Accessed on November 5, 2024 from https://correlatesofwar.org/data-sets/
[3] Gibler, Douglas M. (2009). International military alliances, 1648-2008. CQ Press.
[4] PBS Digital Studios. (2017). Network Mathematics and Rival Factions. (June 2017). Accessed on November 10, 2024 from https://www.pbs.org/video/network-mathematics-and-rival-factions-infinite-series-ijmbu2/ 