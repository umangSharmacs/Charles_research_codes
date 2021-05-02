# Charles_research_codes
 Exploration and Experimentation on various datasets

 ## 1. CNN and DailyMail Dataset
Divided the stories into texts and their respective summaries.
Preprocessed them and calculated the following features:
1. Frequency (BoW)
2. Proper nouns
3. Numerical Data
4. Sentence length
5. Sentence position
6. Uppercase

These are contained in the Processed_csv folder. Each csv roughly contains 10,000 rows. 

Labelled the sentences depending on whether they are in the summary or not. used Word2Vec and applied cosine similarity between sentences to find this label. 
Then trained several models with the with an accuracy of 78.5% and F1-score of 33.4

## 2. ICSI dataset
Used the dialogue from transcripts and removed any annotations in between.
Applied BoW approach to calculate the highest scoring sentences i.e. the sentences which contain the most frequent words. 
 <b>TODO: Use these as checkpoints to find more important sentences, and thus minimise the text.</b>

Similarly, divided the text into 4 parts, treated each part as a document and applied TF-IDF to it. 
Best scoring sentences can again be used as checkpoints. 

Checkpoint and TFIDF parameter can be based on length of document, length of highest scoring sentence, highest score and distribution of score etc.

## 3. AMI Corpus

Used the 137 transcripts out of 172 that had both Abstractive and Extractive summaries.
Calculated a number of features:
1. Average sentence length
2. Average word length
3. Maximum sentences
4. Maximum sentence length
5. Maximum sentence position
6. Minimum sentences
7. Minimum  sentence length
8. Minimum  sentence position
9. Median and mean of sentence positions that were also in the extractive summary.
10. Maximum scoring 5 words per transcript

Used them to experiment and explore the dataset more. 
The colab notebook is well organised for this corpus so I am not going into much detail here.


 

