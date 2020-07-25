# DEEP-LEARNING-FOR-SENTIMENT-ANALYSIS-ON-REVIEWS-OF-MODERN-AZERBAIJANI-MOVIES

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/8c4076012b6640b3a8440c25c7ed1ee3)](https://app.codacy.com/manual/NijatZeynalov/DEEP-LEARNING-FOR-SENTIMENT-ANALYSIS-ON-REVIEWS-OF-MODERN-AZERBAIJANI-MOVIES?utm_source=github.com&utm_medium=referral&utm_content=NijatZeynalov/DEEP-LEARNING-FOR-SENTIMENT-ANALYSIS-ON-REVIEWS-OF-MODERN-AZERBAIJANI-MOVIES&utm_campaign=Badge_Grade_Dashboard)

In this project, I investigate the comments associated with a set of modern Azerbaijani movies and perform sentiment analysis of each comment which is classified into positive or negative polarity. The project mainly describes the implementation of the Multilayer Perceptron (MLP) model  that can be used to detect sentiments from the text. 

The project consists of three primary components:

* [__PREPARING MOVIE REVIEW TEXT DATA FOR SENTIMENT ANALYSIS IN AZERBAIJANI__ ](https://www.researchgate.net/publication/340933198_PREPARING_MOVIE_REVIEW_TEXT_DATA_FOR_SENTIMENT_ANALYSIS_IN_AZERBAIJANI "Study link")

  The main objective of this component is to retrieve and pre-process movie review text data in the Azerbaijani which will use for predicting sentiments of new reviews. Although, most of data on social media is text-based, it is not possible to directly apply deep learning processes to this raw data and text data preparation is different for each problem. Preparation starts with simple steps, like loading data, but quickly gets difficult with cleaning tasks, filtering only the relevant data which are very specific to the data we are working with.
  
   One of the biggest obstacles to this study was the lack of resources that prevents us to produce better quality text data in the
Azerbaijani language. Some processes are required to prepare the data before the algorithms are implemented and in this project,you will discover how to prepare movie review text data for sentiment analysis in Azerbaijani.

* [__DEVELOPING A NEURAL BAG-OF-WORDS MODEL FOR SENTIMENT ANALYSIS__ ](https://www.researchgate.net/publication/341114898_DEVELOPING_A_NEURAL_BAG-OF-WORDS_MODEL_FOR_SENTIMENT_ANALYSIS "Study link")

  The goal of most sentiment tasks is to identify the overall sentiment polarity of the documents in question, i.e. is the sentiment of the document positive or negative? For our case, we use online user reviews from the most popular Azerbaijan movies. In order to perform this sentiment task, we use a mixture of baseline machine learning models and deep learning models to learn and predict the sentiment of binary reviews.
 
    This poses a supervised learning task. For this purpose, we will use bag-of-words features with machine learning algorithms which is very simply and efficient, while having the ability to achieve very high accuracy. In this paper, we will develop a neural bag-of-words model, which collects high-level structural and semantic meaning of the words. The paper performs sentiment classification via neural bag-of-words approach.
    
 * [__PREDICTING SENTIMENT FOR REVIEWS (COMMENTS) IN MODERN AZERBAIJANI MOVIES__ ](https://www.researchgate.net/publication/341135595_PREDICTING_SENTIMENT_FOR_REVIEWS_COMMENTS_IN_MODERN_AZERBAIJANI_MOVIES "Study link")

    In this paper, I have prepared a dataset on Azerbaijani movies which consists of 82.806 comments from YouTube for predicting sentiment values. In a movie review context, it is possible to use Sentiment Analysis to give the user a single rating for each movie that is a cumulative result of the reviews, comments that have been posted on Youtube. This paper also contains some details regarding sentiment-based classification of data. Data regarding the trailers of a movie from YouTube can provide useful insights for sentiment analysis.
  
    After preprocessing, I have developed a MLP model to predict the sentiment of encoded reviews. The model will have an input layer that equals the number of words in the vocabulary and in turn the length of the input documents. 

  * __RESULTS__
  
    We wanted to predict sentiment movie reviews. For the experiment purpose, we collected more than 80.000 reviews of 33 modern Azerbaijan movies. Next, we used a final model to make predictions for new textual reviews. Predicting the sentiment of new reviews involves following the same steps used to prepare the test data. Specifically, loading the text, cleaning the document, filtering tokens by the chosen vocabulary, converting the remaining tokens to a line, encoding it using the Tokenizer, and making a prediction. 
    
    We can then make predictions for new review texts. You will see an example with both a clearly positive and a clearly negative review using the simple MLP developed above with the frequency word scoring mode.
    
    ![picture alt](https://i.ibb.co/q9B7VCN/untitled.png "Title is optional")

     As you see from the chart above, “My name is Intigam” and “Zeher tulugu 4” movies have maximum positive sentiments, while “Yumurta” has received the worst comments from the users. Besides of this, although “Ikinci perde” movie is considered one of the best in our country, the most negative words used in the comments are about the subject of this film and it affects sentiment value badly. For example the movie subject is about betrayal and most comments contain this word which accepted as negative sentiment by our model. 

    Moreover, the movies in the list belong to different genres and we are  able to see the positive reviews for each movie mostly. The reason for this is not just because this movie is perfect, but because the audience group is different.
