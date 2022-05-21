# Tales-from-the-Crypto
NLP Homework Assignment 

![image](https://user-images.githubusercontent.com/99493522/169658999-86c437e6-42de-43be-bad2-5cae681ea07d.png)

## Background
Due to the hype in the news regarding cryptocurrency, the latest news headlines regarding Bitcoin and Ethereum will be anayzed to get a better feel for the current public sentiment around each coin. In this assignment, Natural Language Processing will be applied to understand factors involved with coin prices such as common words and phrases, and organizations and entities mentioned in the articles. 

## Resources
Vader Sentiment Analysis,
Python, 
NLK library, 
NER, 
SpaCY library, 
News API Client, 
Pandas, 
Jupyter Lab,  

## Procedure
### Sentiment Analysis:
The [newsapi](https://newsapi.org/) was used to pull the latest news articles for Bitcoin and Ethereum, a DataFrame of sentiment scores for each coin was then created. 
Descriptive statistics was used to answer the following questions:


![image](https://user-images.githubusercontent.com/99493522/169659578-f4644718-f515-49bd-9252-a6bd9683ed07.png)

### Natural Language Processing:
NLTK and Python were used to tokenize text, find n-gram counts and create word clouds for both coins. 

**Bitcoin Word Cloud**

![image](https://user-images.githubusercontent.com/99493522/169659759-c6ad0894-e096-461a-8ad1-d2bb5575ed3a.png)


**Ethereum Word Cloud**

![image](https://user-images.githubusercontent.com/99493522/169659775-867c55bc-68c6-41d3-8f43-bd445a413246.png)

### Named Entity Recognition
A named entity recognition model for both coins were built and visualized using SpaCy. Example code shown below. 

    # Run the NER processor on all of the text
    bitcoin_doc = nlp(concat_bitcoin)
    bitcoin_doc

    # Add a title to the document
    bitcoin_doc.user_data["Title"] = "Bitcoin NER"
    
    # Render the visualization
    displacy.render(bitcoin_doc, style = 'ent')
    
 ## Contributors
 Chantal Garnett


