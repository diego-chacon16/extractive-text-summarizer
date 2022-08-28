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

+** How will the scoring work? Score = Average(non-zero TD-IDF values)**
+ Ie. if row = [0, 1, 0, 0, 0, 2, 3, 0, 0, 0] then score = avg(1,2,3) = 2
