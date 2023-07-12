# Topic Modeling for Research Articles using Latent Dirichlet Allocation(LDA)
This project is a part of the Data Mining course during my Master's at Penn State University.

#### -- Project Status: [Completed]

## Project Objective
The purpose of this project is to use Topic Modelling to classify research articles into distinct categories thus facilitating recommendation and research process.


### Partner
* Parva Jain
* Akanksha Anand

### Methods Used
* Inferential Statistics
* Machine Learning
* Natural Language Processing
* Data Visualization

### Technologies
* Python
* Jupyter

## Project Description
* **Goal:** The goal of the project is to use Latent Dirichlet Allocation (LDA) to identify core topics of research articles.
* **Data Source:** [Kaggle](https://www.kaggle.com/blessondensil294/topic-modeling-for-research-articles)
* **Data Preparation:**
  * **Sampling:** The original dataset had a skewed distribution of the documents which would result in a biased model. To prevent this from happening we sampled 250 articles from each topic.
  * **Removal of punctuations and Stopwords:** Stopwords and punctuations provide minimal semantic information. Removing these words and punctuation makes it easier to isolate and find the words required to differentiate the topics.
  * **Lemmatization, Tokenization, and Part-of-Speech Tagging:**
    * Lemmatization is the task of grouping up different forms of a word so that they can be computed as a singular item.
    * Tokenization is the process of converting a string into pieces or “tokens”. For example, converting a sentence into words or a combination of words.
    * Part-of-Speech tagging is the process of marking different words in a corpus to their corresponding “part-of-speech” (noun, adjective, verb, adverb, etc.). In our case, we only use the words tagged as nouns or adjectives.
  * **Creating Bigrams and Trigrams:** Bigrams and Trigrams played a significant role in text preprocessing to create relevant pair of words. The threshold value is kept at 100 as for lower threshold values many irrelevant and noisy data was getting added in the output hence distorting the model result.
  * **Using TF-IDF to remove low-frequency words:** Term Frequency-Inverse Document Frequency(TF-IDF) is calculated based on two different metrics. The term frequency is the frequency of each term in a document and inverse document frequency is the frequency of how many documents contain that word.
* **Modeling:** The LDA implementation was made with the library Gensim.
* **Outcome:** The finalized LDA model was achieved with a perplexity of -7.99182 and a coherence score of 0.42829.


## Needs of this project
- data processing/cleaning
- statistical modeling
- writeup/reporting

## Getting Started
1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Sampled(Stratified) Data is being kept [here](/Data/strat-sampled-dataset.csv) within this repo.

## Featured Notebooks
* [Base](/TopicModeling-LDA.ipynb) This is the base notebook for LDA implementation

## Contact
Feel free to contact me with any questions via [LinkedIn](https://www.linkedin.com/in/akshay2718/)