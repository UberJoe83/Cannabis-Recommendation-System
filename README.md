# Cannabis-Recommendation-System


## Overview

As of October of 2020, 33 states have legalized the use of medicinal cannabis, including 11 states that have also legalized its recreational use for adults the age of 21 and over. The legal cannabis industry is very young and in constant growth and expansion and it is only a matter of time until it becomes legal on a Federal level. There are countless dispensaries that sell cannabis products through websites like Weedmaps and Leafly, you simply choose a dispensary and check out their menu and make an order, which you can then either pick up or have delivered. The website also has a section which is dedicated to the many strains of the cannabis plant to rate, report on the effects, and describe the flavors associated with the strain that the user has tried. This section is usually curated by experts in the field with the use of their experience and knowledge about marijuana.

We see recommendation systems in our everyday life more and more, Netflix, Amazon, and Instagram are just a few examples of where this technology is used to give the user an easier way to connect to people and make decisions about what to buy or watch next.


## Objective

Using the Cannabis Strains dataset found at (https://www.kaggle.com/kingburrito666/cannabis-strains), I will first explore the data focusing on the types of strains, effects, and flavors that are available to everyone, in order to gain some insight about what is important when it comes to choosing what to try out. Since there is no user-based data I will then proceed to build a content-based recommendation system which will take the input of a certain strain and return the 10 most similar strains to the user, this will be achieved using the Cosine Similarity distance metric.


## Contents

 - README.md - currently there!

 - Cannabis Recommendation System Capstone.ipynb - the Jupyter Notebook containing the finalized code for this project.

 - cannabis.csv - the file containing the dataset which comes from Kaggle (https://www.kaggle.com/kingburrito666/cannabis-strains)

 - final_strain.csv - the file containing a clean and one-hot encoded version of the cannabis.csv file

 - CAPSTONE_PROJECT.pdf - pdf of my project presentation
 

## Libraries and Packages

 - numpy
 
 - pandas
 
 - matplotlib.pyplot
 
 - seaborn
 
 - from sklearn.preprocessing - StandardScaler()
 
 - from sklearn.manifold - TSNE
 
 - from sklearn.metrics.pairwise - cosine_similarity
 
 - from sklearn.decomposition - PCA
 
 
## EDA and Visualization
 
The EDA performed in this project was performed using the pandas and numpy libraries, with the visualizations being created using Seaborn plots with arguments from the matplotplib.pyplot package.


## Conclusions

I made various comparisons with the recommendations generated from the raw data and the data that went through PCA, although both recommendations seemed to make sense and the strains that were recommended were very similar to the input strain, it seemed to me that using the entire dataset was more useful and provided more variety in the types of strains that were recommended.

We saw that in the original recommendations for the sativa type strain, the user was suggested to try a different type of strain other than a sativa. I feel like this would be a very important value of my recommendation system, which was not seen after performing dimension reduction. For now I will stick with the first version of the recommendation engine.


## Business Recommendations

 - In order to optimize this recommendation system, we must collect more user-based data with more ratings and the average of prices seen in different dispensaries. This will give us more that just categorical data to work with.
 
 - For now we should use the raw data set to model our recommendations, this data provided more variety in its suggestions which is a great feature to have.


## Future Work

 - Use the current ratings reported and implement them into the current recommender.
 
 - Gather more data about pricing and new strains that have been created, as well as more user based content so that we can apply collabrative filtering into our recommendation system.
 
 - Use the current descriptions about the strains to gain further insight about what are the most important things to consider when trying a new strain.
 
 - Use other dimensionality reduction techniques such as Autoencoders, to build different kinds of embeddings to possibly make better suggestions.


