📰 News Analysis

In this project, we aim to broadly predict what each news article is about.
We’re analyzing a dataset of 7,600 news articles, which includes 1,900 articles across four categories: sports, science and technology (sci/tech), business, and world.
Our goal is to predict whether business or world news articles carry a positive or negative tone. For sports news, we’ll classify whether the article reports match results or discusses general sports topics. For sci/tech news, we want to determine whether the article is related to artificial intelligence or covers another subject.
Below is a brief overview of how we’ll approach the project. As we progress, we’ll describe each step in detail to make the work as clear and practical as possible.
First, we’ll load and import all the necessary libraries for the project, such as sklearn, nltk, spacy, pandas, among others.
We’ll load the CSV file containing all the news articles and perform a brief exploratory data analysis.
We’ll create a copy of the dataset to work more safely, avoiding any risk of data loss or incorrect manipulation.
Next, we’ll begin the natural language processing phase, applying common techniques such as tokenization, converting all characters to lowercase, lemmatization, stemming, removing stopwords, and eliminating punctuation marks.
Finally, we’ll move on to prediction and deep learning. Using classification models like RandomForest or LogisticRegression, along with techniques such as TF-IDF or Bag of Words, we’ll train models to accurately predict the content of each article.
At the end, we’ll present a final conclusion summarizing the project and the results obtained.

Conclusion

We can conclude that both deep learning approaches used in this project performed effectively and delivered strong results. Among the techniques applied, we leaned toward the TF-IDF method, and the prediction model that achieved the highest accuracy was XGBoost.
In the analysis of whether business or world news articles carried a positive or negative tone, we used the Sentiment Intensity Analyzer, along with a custom function to classify each text based on its sentiment score.
For the sports category, we applied the TF-IDF methodology and compared three different prediction models to determine which yielded the best performance. In this case, XGBoost again stood out, achieving an accuracy of 0.92.
In the final case study, we aimed to identify whether sci/tech news articles were related to artificial intelligence. To do this, we vectorized the text and applied a Random Forest Classifier, enhanced with GridSearchCV for hyperparameter tuning. This approach delivered near-perfect results, with an accuracy of 0.99.
🔮 Future Outlook
If we scale this project to a larger dataset with more news articles, we’ll need to carefully evaluate model performance and, if necessary, adjust parameters or explore alternative models to maintain high accuracy levels.
