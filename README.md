# Capstone-Project

## Research Question
To find the sentiments on movie reviews

## Expected Data Source
https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/data

## Techniques expected to use in the analysis
Natural Language Processing, N-gram

## Expected Results
Movie reviews are labelled with sentiments like negative, somewhat negative, neutral, somewhat positive, positive.
Based on the sentiments, recommend/not recommend the movie to people.

## Importance of the topic
It can help people to know whether the movie is good or not before watching. It can save a lot of their time and money when choosing movie to watch. 
It can let the movie producer to know how to improve the movie quality by understanding audiences' feelings.

## Conclusion
Movie reviews are labelled with sentiments like negative, somewhat negative, neutral, somewhat positive, positive. Natural Language processing techniques are used to understand the sentiment in the moview reviews. Based on the model I built, movies can be recommended/not recommended to people. It can also helps the filming industry to know what kind of movies the large audience likes to watch.

I have first applied stemming and lemmatizing to preprocess the data. Then I used GridSearchCV to find the best machine learning model. The machine learning methods I have used include CountVectorizer, TfidfVectorizer, Logistic Regression, DecisionTreeClassifier and Naive Bayes. To balance between auuracy score and time used to build the model, I found that Stemmed Content + CountVectorizer with Decision Tree is the best among all methods. 

The mean cross validation score for the model is 0.6042 (std:  0.0019 ), Precision is 0.5973, Recall is 0.6152 and the F1 score is 0.5969 .

By inputting new phrases or sentences, the model can tell the sentiment of the review. Hence, the movie rating can be indirectly deduced.

## Further Works
1) Instead of removing name tags in the text, may be try to extract the tokenized verb for classification
2) Try more parameters in GridSearchCV
3) Apart from GridSearchCV, maybe try HalvingGridSearchCV to find the best model 
4) Apart from Logistic Regression, Bayers, Decision Tree, use other methods.
5) Since the original dataset was preprocessed, a sentence is divided into pieces. Maybe try to take the longest sentence in each PhraseId and rebuild the model
6) Filter the spam texts before building the sentiment analysis model

## Link to the project
https://github.com/crystalsw/Capstone-Project
