# Content-Based Recommendation System

## Overview

This repository contains a simple content-based recommendation system that suggests similar items (e.g., movies) based on a short text description provided by the user. The system uses TF-IDF vectorization and cosine similarity to rank items in a small dataset.

## Dataset

The dataset consists of a list of movies along with their plot summaries.

**Source**: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?resource=download&select=movies_metadata.csv

The dataset is preprocessed to randomly sample 500 rows for analyzing purpose. The preprocessing procedure can be seen in data_loading.ipynb

## Approach

**Text Vectorization**: The input description and each movie's summary are transformed into TF-IDF vectors.

**Similarity Computation**: Cosine similarity is computed between the user input and all dataset entries.

## Code Organization

**recommendation_system.ipynb**: Main script that runs the recommendation system

**movies_sample**: Randomly sampled 500 rows from the Source(movies_metadata.csv)for analyzing purpose

**data_loading.ipynb**: The preprocessing procedure from movies_metadata.csv

**requirement.txt**: Lists dependencies required to run the project

**README.md**: Documentation.

## Setup

**Clone the repository**

```bash
git clone https://github.com/LufeMC/lumaa-spring-2025-ai-ml.git
cd lumaa-spring-2025-ai-ml

**Install dependencies**

pip install -r requirements.txt

**Open and run the Jupyter Notebook**

jypyter notebook

## Example Output

**Input:**

I like action movies set in space.
5

**Output:**

Recommended Movies:
         original_title  cosine_similarity
221           Space Cop           0.149704
478  Monsters vs Aliens           0.146310
71            Dreamboat           0.138510
211            疯狂的赛车           0.123857
251         Šakalí léta           0.106885
