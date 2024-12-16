# MapReduce-Algorithm
This project utilizes the MapReduce algorithm to analyze a dataset of over 2,500 fraudulent emails. The **Fraudulent E-Mail Corpus**, available from Kaggle. The objective is to count word frequencies in the dataset and identify the 20 most frequently used words. The project also evaluates whether the dataset's nature as phishing emails can be inferred from the frequent words and suggests improvements to the word counting technique for enhanced spam detection.

## Key Features

- Implemented the MapReduce algorithm in Python for word frequency analysis.
- Processed text data without using inherently sorted data structures like dictionaries.
- Identified the top 20 most frequent words from phishing emails.
- Analyzed the linguistic characteristics of fraudulent emails based on word frequencies.

## Steps Followed

1. **Data Extraction:**
   - Downloaded and extracted the **Fraudulent E-Mail Corpus** dataset from [Kaggle](https://www.kaggle.com/datasets/rtatman/fraudulent-email-corpus).
   - Processed the `fradulent emails.txt` file as input for the analysis.

2. **Implementation of MapReduce:**
   - Designed a Map task to process the text and generate `(key, value)` pairs for each word.
   - Grouped the `(key, value)` pairs for processing by the Reduce task.
   - Calculated word frequencies using the Reduce task, ensuring no reliance on dictionary-like structures.

3. **Analysis:**
   - Extracted the 20 most frequent words.
   - Evaluated whether these frequent words reflect the phishing nature of the dataset.
   - Discussed improvements for using word frequency analysis as a spam detection tool.

## Results

1. **Top 20 Frequent Words:**
   - A table or visualization highlights the most common words and their counts.

2. **Insights on Dataset:**
   - The most frequent words often relate to phishing tactics, such as references to financial transactions or urgency.

3. **Improvement Suggestions:**
   - Include stopword removal, stemming/lemmatization, and bigram/trigram analysis for improved detection.

## Tools Used

- Python
- Jupyter Notebook

## How to Run the Code

1. Clone the repository and download the dataset from the [Kaggle link](https://www.kaggle.com/datasets/rtatman/fraudulent-email-corpus).
2. Place the `fradulent emails.txt` file in the project directory.
3. Open and execute the provided Jupyter Notebook in any Python environment.

## Visualizations

- Bar chart of top 20 frequent words.
- Word cloud of frequent words to visualize trends in phishing emails.

## Future Work

- Expand the analysis by integrating Natural Language Processing (NLP) techniques for better spam classification.
- Implement a more robust method to evaluate the context of words within emails.
