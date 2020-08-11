# Quantitative Text Analysis of Citizenship Amendment Act

These code files are part of my MSc Applied Social Science thesis on Citizenship Amendment Analysis. 
In this topic, following three broad questions were explored:

Q1 - How did the Pro CAA and Anti CAA groups characterized the Act and the related events?

Hypothesis 1 - The popular terms in tweets are a reflection of news events in real time. 

Hypothesis 2 - A very few users create bulk of the tweets during politically charged events. And most users engage in copy pasting or broadcasting the 
available content.

<b>Method</b>

Data bifurcation - The dataset was divided on the basis of languages - Hindi and English and languages other than these two were exlcuded for the ease of analysis. 

Tweet classification - I manually classified some of the tweets into Pro CAA (supporters of the Act), Anti CAA (Critics), and Neutral (this group incluuded users displaying a neutral political stance and breaking news tweets). Rest of the tweets were labelled using linear support vector machines algorithms, which yielded an accuracy of 86% in label predictions. 

             precision    recall  f1-score   support

     Pro_CAA       0.87      0.89      0.88      1890
    Anti_CAA       0.78      0.74      0.76       971
     Neutral       0.91      0.92      0.91       714

    accuracy                           0.86      3575
   macro avg       0.85      0.85      0.85      3575
weighted avg       0.85      0.86      0.86      3575


Cosine Similarity - To check if the users were creating original content, cosine similarity was measured in both the language based dataset apart from counting duplicated tweets and re-tweets.

Relative and regular term Frequency analysis - These methods were used to find the most popular words in the twoo-language based corpus and hashtags were removed before applying the frequency analysis. Keyness analysis (Relative Frequency Analysis)is a method to identiy the distinguishing keywords in text classification. In this case, I used it to identify the keywords that three groups used to describe the Act.  



