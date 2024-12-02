
# IMDB Movie Comment Classification

  

This project utilizes machine learning to classify movie comments from the [IMDB platform](https://www.imdb.com/) into two categories: positive and negative. The aim is to build a model that can accurately classify comments based on sentiment.

  

## Project Overview

  

The dataset used for this project is contained within the `imdb` folder, which includes a subset of [IMDB movie](https://www.imdb.com/) criticism data. The dataset consists of 1250 positive and 1250 negative comments, organized in files named `pos` and `neg`, respectively.

  

### Specifications

  

The complete solution for this problem is implemented in the `4.py` file. When executed, this file will perform the following tasks:

  

1. **Data Cleaning and Feature Vector Creation:**

    - Clean the dataset and create feature vectors.
    
    - Split the dataset into training (80%) and testing (20%) sets.
    
    - Fit a Multinomial [Naive Bayes model](https://en.wikipedia.org/wiki/Naive_Bayes_classifier) to the training data.
    
    - Achieve an accuracy of at least 75% on the test set, averaged over three consecutive runs.

  

2. **Confusion Matrix:**

    - Generate a [confusion matrix](https://en.wikipedia.org/wiki/Confusion_matrix#:~:text=In%20predictive%20analytics,%20a%20table,false%20positives,%20and%20true%20negatives.) in the format `[[TN, FP], [FN, TP]]` to evaluate the model's performance.

  

3. **Most Common Words Analysis:**

    - Identify the five most frequently used words in positive comments, and similarly for negative comments, including commentary on the results.
    
    - Introduce the metric `LR(word)`, defined as:
    
      > LR(word) = {Count in Positive Comments} / {Count in Negative Comments}
    
    - Find the five words with the highest and the five with the lowest values of this metric, ensuring that only words appearing at least 10 times in both positive and negative comments are considered.
    
    - Provide commentary on the ten identified words, comparing them with previous results and explaining the significance of the `LR` metric in the context of this analysis.

  

## Requirements

  

- [Python 3.x](https://www.python.org/downloads/)

- Libraries: `tensorflow`, `numpy`, `pandas`, `sklearn`, `matplotlib`

  

## How to Run

  

1. Clone the repository:

```bash

git clone https://github.com/yourusername/imdb-comment-classification.git

cd imdb-comment-classification
