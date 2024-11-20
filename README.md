# War Machine

This repository was created for a semester project in Michigan State University's CMSE 202, Computational Modeling Tools and Techniques during the Fall of 2024 taught by Dr. Nathan Haut at the Department of Computational Mathematics, Science, and Engineering.

This project comes under the social sciences.

## Group members:

1. Kyle Cowden
2. Lowell Monis
3. Joseph Burke
4. Saif Sheikh
5. Adhvik Kolar


## Abstract

Our project focuses on modeling and predicting international alliances and the likelihood of conflict using the Correlates of War (CoW) datasets. This work integrates computational modeling, data analysis, and machine learning to answer two central questions: 

1. How do alliance configurations shift over time?
2. What is the probability of war given specific parameters, such as trade volume, religious alignment, and diplomatic relationships?

These questions are motivated by the need to better understand the dynamic nature of global alliances and the conditions under which conflict arises, contributing to the broader field of political science, international relations, and social relations.

### Background and Motivation

The CoW datasets provide a comprehensive archive of historical and contemporary data on interstate conflicts, alliances, trade, and diplomatic exchanges. Leveraging this dataset allows us to analyze how various factors influence alliance stability and the onset of conflict. Our motivation lies in advancing predictive capabilities using computational tools and exploring the theoretical implications of alliance dynamics through graph theory and machine learning.

### Methodology

We employed a multi-faceted approach combining graph theory, machine learning, and exploratory data analysis. The first phase involved constructing network graphs where nodes represented countries and edges depicted alliances. We implemented graph-theoretical stability rules to identify two configurations: complete graphs, which signify stable alliances, and disjoint subgraphs, which often predict conflict. For the second phase, we utilized Python-based libraries such as `NetworkX` for graph analysis, `pandas` for data processing, and `scikit-learn` for machine learning. Key machine learning models included logistic regression and support vector machines (SVMs), chosen for their interpretability and effectiveness in binary classification tasks like predicting war likelihood and alliance shifts.


