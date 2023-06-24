# Company Classification using NLP Approaches

## Overview

This research paper is part of a collaboration between researchers from the [Faculty of Computer Science & Engineering](https://www.finki.ukim.mk/en) at the
Ss. Cyril and Methodius University in Skopje and [Boston University](http://www.bu.edu/).

## Features

Company classification is a fundamental task in natural language processing (NLP) that aims to categorize businesses based on their textual descriptions. The purpose of the research paper is to employ various NLP approaches to tackle this problem, each with its own strengths and limitations.

## Installation

The code is available as Colab notebooks. The easiest way to use the notebooks is to upload them to and run them in [Google Colab](https://research.google.com/colaboratory). The notebooks contain imports of the necessary Python libraries. There are no dependencies and no additional modules or libraries need to be installed.

## Known Limitations

We suggest to use GPU runtime when running the notebooks for more efficient compiling.

## Usage

There are 19 Colab notebooks arranged in 5 folders used for classifying companies based of their descriptions. Each of the notebooks processes the datasets in a specific way. 

In the notebooks where OpenAI API is used, the _"YOUR-API-KEY-HERE"_ section should be filled with your API key from OpenAI. Please follow the instructions in the notebooks. 

This is the brief content for each of the folders:

1. AutoEncoder Approach
    - An Autoencoder was used to reduce the unnecessary dimensions after embedding the sentences.
    - An OneVsRest Classifier was then used for classification after reducing the dimensionality.

2. BERT Transformer
    - This notebook used 'roberta-base' transformer and 'roberta-base' tokenizer for classification.
  
3. OneVsRest Classification
    - This folder contains models utilizing the OneVsRest Classifier and the Support Vector Classifier as its estimator.
    - For embedding the sentences, the 'all-mpnet-base-v2' and 'hkunlp_instructor-large' sentence transformers were used.
    - OpenAI API was used for comparing the results of the model against ChatGPT predictions on the same data.
    - Various techniques were used for cleaning the data.

4. Unsupervised Approach
    - Agglomerative Clustering was used for clustering the 11 sectors in GICS.
    - For embedding the sentences, the 'nli-distilroberta-base-v2' sentence transformer was used.
    - To ease the visualization process, PCA was used for reducing the dimensionality.

5. Zero-Shot Classification
    - This folder contains models utilizing the Zero-Shot classification pipeline using the 'valhalla/distilbart-mnli-12-3' model.
    - TF-IDF was used for getting more precise representation of the sector names for enhancing the accuracy of the model.

## Authors

- [Maryan Rizinski](https://github.com/rizinski)
- [Andrej Jankov](https://github.com/nubs4dayz)
- Igor Miskovski
- [Dimitar Trajanov](https://github.com/trajanov)
