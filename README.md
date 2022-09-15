# Extractive Text Summarizer

## Text Summarization with TF-IDF

+ High-level outline
+ Split the document into sentences
+ Score each sentence
+ Rank each sentence by those score
+ Summary = Top scoring sentences

## Approach

+ Sentence tokenization (splitting the document into sentences) with NLTK
+ Build TD-IDF matrix, treating each sentence as if they were documents

## How will the scoring work? Score = Average(non-zero TD-IDF values)
+ Ie. if row = [0, 1, 0, 0, 0, 2, 3, 0, 0, 0] 
+ Score = avg(1,2,3) = 2


# Text Summarization with Sumy

#### What is Sumy?

+ Is a simple library used for extracting summary from HTML pages or plain texts
+ The package also contains simple evaluation framework for text summaries

#### Goal

+ To build an extractive text summarizer highlighting the key points of the article

#### Approach

+ Import libraries and data
+ Create a function to wrap the text and easier to read
+ Build the summarizer and parser using sumy packages
+ Add them to the dataframe
