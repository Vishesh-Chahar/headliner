# headliner
News Article Analysis with Transformers and Text Processing
This repository contains Python code snippets for processing and analyzing news articles using various libraries such as Transformers, NLTK, Pandas, NumPy, and Scikit-learn. The code demonstrates tasks like data preprocessing, text vectorization, clustering, and sentiment analysis.

Features
Data Processing: Concatenate and shuffle news articles from multiple CSV files for analysis.
Text Preprocessing: Remove stopwords from text documents using NLTK and tokenize the content for further analysis.
TF-IDF Vectorization: Vectorize text data using the TF-IDF technique to prepare it for clustering.
K-means Clustering: Apply K-means clustering to group news articles based on their content.
Sequence-to-Sequence Tasks: Utilize Transformers library for sequence-to-sequence tasks in natural language processing.

Project:
The project uses LoRA to fine-tune 27.36% of the parameters of flan-t5-large, an open source LLM from huggingface. It uses cuda to utilize the processing power of my GPU for faster calculation.
The dataset is the "All the news" dataset and the main idea was to generate headlines for a given corpus of news article content. 
The focus was on business emails, so k means clustering was used to first separate and clean the data. 
50% of that was used to train the dataset.
top_k and top_p were also used to fine tune the output of the model which upon human evaluation appears to be much better results than the untuned model.

Usage
Install the required Python libraries by running pip install -r requirements.txt.
Run the provided code snippets in a Python environment to process and analyze news articles data.
Customize the code as needed for your specific text analysis tasks.

