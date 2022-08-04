# DigikalaCommentAnalysis
Digikala is a popular online shop in Iran. This project analysis costumer's comments on different products from Natural Language Processing aspects. 

## Configuration
- vectsize = 150 (vector size)
- wordnum = 10 (number of words in each comment)
- samplenum = 60035 (number of samples)
- stopwords = [] (List of removing meaningless words)

## Data preparation
In this phase, ponctuations are removed from the corpus. Additionally, a dictionary which contain comments and their labels is defined.

## Tokenizer
Stanza word tokenizer is used for this phase. One of two following configuration can be choosed.
- tokenizer + skip grams
- lemmatizer + CBOW

As the purpose of evaluating there two configuration some statistics are compared:
- Similar words to a particular in addition to defined positive and negative words
- Similary of two given words
- Words similar to a given word
- Most repeated words

## Model Archineture

### CNN
![atl text]()
Branches:
1. tokenizer
2. word2vec
3. cnn
