# Tweet_Sentiment_Analysis_Capstone

## **Project Overview**
Social Listening is a powerful method for understanding public sentiments. In the past, surveys were the primary means of gauging public opinion on specific topics. However, today, a more organic approach involves monitoring online conversations to glean real-time insights. Social Listening, achieved through the extraction and analysis of thousands, and ideally millions, of comments on social media platforms, has emerged as an effective way to gather data and empower businesses, individuals, and brands.

When engaging in Social Listening, both quantitative and qualitative information can be delivered to comprehensively grasp the dynamics of the digital world. By tracking online discussions, one can decipher what people are saying, when, and why. These insights are invaluable for tailoring strategies to target audiences effectively.

### **Scope**

The scope of this project extends beyond Social Listening and initiates with the acquisition of a robust dataset of Twitter conversations. Initially, it was planned to directly scrape conversations from Twitter using the Twitter API. However, due to high associated costs and fundamental data quality issues observed with truncated text in the alternative dataset obtained from from [Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets). A decision has been made to rectify this by directly scraping data from Twitter for Sprint 3.

Following an analysis of the dataset to identify and address data quality issues, as well as explore feature engineering opportunities and other notable observations related to data processing, the data will undergo preprocessing for further analysis. All tweets will be tokenized to lower case, removing punctuations, handles, hashtags, stop words, and links to ensure a standardized and cleaner dataset.

The initial analysis will involve Sentiment Analysis to categorize conversations into positive, negative, or neutral tones. Additionally, features such as counts of the most positive and negative words, word cloud representations, and other descriptive visualizations will be extracted.

Furthermore, a clustering analysis will be conducted to develop a functional algorithm trained on our dataset. This algorithm will later identify new topic-related comments and assess the sentiment's alignment with the existing clusters, aiming to predict accurately the cluster to which a new tweet belongs.

For the clustering algorithm, pre-labeled datasets have been extracted to generate features for either Democrats or Republicans, aiming to identify words indicative of political alignment commonly used by each group (e.g., "pro-life" or "pro-choice").

In addition to the planned Logistic Regression using CountVectorizer, a pipeline will be implemented to model a Random Forest and a Naive Bayes, providing a more comprehensive analysis.

The analysis will also explore the modeling of words in tweets and hashtags to predict if a tweet has a Democrat or Republican inclination. This involves leveraging the unique characteristics of language used by each political group.

Furthermore, the project will consider potential applications of advanced techniques such as Neural Networks or Generative AI for more nuanced and sophisticated analyses. These approaches may offer enhanced capabilities in predicting sentiment, identifying political alignment, and exploring intricate patterns within the Twitter conversations dataset.

### **Objectives**
This project focuses on analyzing political conversations on Twitter, specifically targeting Senators from both the Democrat and Republican parties in the USA. The primary objectives are outlined as follows:

1. **Data Acquisition:**
   - Scrape political tweets from Senators of both the Democrat and Republican parties in the USA. This will be performed for Sprint 3.
  
2. **Exploratory Data Analysis (EDA):**
   - Conduct EDA to extract valuable insights from the acquired dataset.
   - Implement feature engineering techniques to enhance the dataset's analytical potential.

3. **Data Cleaning:**
   - Tokenize all tweets to standardize the text data and facilitate further analysis.
   - Remove noise and irrelevant information to ensure a clean dataset.

4. **Feature Representation:**
   - Implement a Count Vectorizer to convert text data into a format suitable for machine learning models.

5. **Modeling:**
   - Run a Logistic Regression model to classify tweets into Democrat or Republican categories.
   - Implement a pipeline for Naive Bayes and Random Forest models to provide a comprehensive analysis of the data.

6. **Prediction:**
   - Use the trained models to classify future tweets as either Republican or Democrat, based on the patterns identified during training.

7. **Sentiment Analysis:**
   - Perform sentiment analysis on tweets for each political party to gauge the emotional tone of the conversations.

8. **Further Implementation:**
   - Explore advanced techniques such as Neural Networks or Generative AI for more sophisticated analyses.
   - Consider the application of these techniques to enhance sentiment analysis or discover intricate patterns within the political conversations dataset.

By focusing on Senators' tweets and employing a combination of traditional machine learning and advanced modeling techniques, this project aims to gain insights into the sentiments and political affiliations expressed on Twitter. The comprehensive approach includes data cleaning, feature engineering, and the application of diverse models, setting the foundation for potential future advancements in the analysis of political discourse on social media.

## *Areas of Interest Submission*:

The submitted Area of Interest is dedicated to conducting a comprehensive analysis of Twitter conversations, with a specific focus on the domain of politics. The overarching objective is to systematically process the vast amount of data generated from these conversations through a series of well-defined steps.

To begin with, a rigorous data cleaning process will be employed to enhance the quality of the dataset, ensuring subsequent analyses are built on reliable information. In light of recent information, the data cleaning process will now include tokenization, converting all tweets to lowercase, and removing punctuation, handles, hashtags, stop words, and links to standardize and refine the dataset to faciliate further analysis and modeling.

Following the enhanced data cleaning, the extraction of valuable features from the refined dataset will be undertaken. This step aims to contribute to a more nuanced understanding of political discourse on Twitter, now taking into consideration the removal of noise and irrelevant information.

The analysis strategy encompasses both basic and advanced techniques in text data analysis. This multifaceted approach is designed to uncover patterns, trends, and underlying themes within political tweets, setting the stage for more in-depth investigations. The process includes the application of a Count Vectorizer for feature representation, allowing for a detailed examination of word and hashtags frequencies and their impact on political affiliations.

A pivotal component of this initiative involves the implementation of Sentiment Analysis. This analytical tool will be utilized to discern and categorize prevailing sentiments expressed in political tweets, providing valuable insights into the overall tone and mood within the Twitter political sphere. Furthermore, sentiment analysis will be performed on tweets specific to each political party, enhancing the granularity of the analysis.

Moreover, the project will incorporate a clustering analysis to identify inherent groupings within the dataset. Recent updates include the use of pre-labeled datasets extracted from Senators of both Democrat and Republican parties in the USA to generate features for clustering. The goal is to train robust datasets of political tweets by identifying commonalities, facilitating the creation of distinct clusters. This will enable the categorization of future tweets into relevant clusters, fostering a dynamic understanding of evolving patterns and affiliations within the realm of political discourse on Twitter.

By integrating these methodologies, the ultimate goal remains to provide a comprehensive and insightful exploration of political conversations on Twitter. Leveraging both qualitative and quantitative analyses, the project aims to enhance our understanding of the complex dynamics at play within Twitter.

## *Explaining the Problem Area*:

The vast influence of Twitter on shaping opinions and disseminating news raises concerns about the potential for echo chambers and the polarization of perspectives within the digital space. This project aims to address the challenge of understanding and mitigating the impact of social media on public discourse by analyzing political conversations on Twitter. By deciphering the underlying patterns and sentiments in these discussions, we seek to contribute valuable insights that may aid in fostering a more informed and balanced digital discourse, counteracting potential biases, and promoting a healthier online information ecosystem.

The choice to focus on Twitter in this project makes sense when you consider its huge user base—over 500 million people use it every month around the world. It's like this buzzing hub where people share information and shape opinions. Recent studies found that a whopping 78% of Twitter users use it for news, and 63% feel more connected to the world because of it. These numbers show just how big of an impact Twitter has on our conversations and perspectives.

Our goal with this project is to go beyond just watching what's happening. We want to dig into the interesting discussions that shape our online world. By mapping out what people are talking about and understanding the stories behind it, we hope to shed light on how social media influences what we think, how we consume news, and how we engage with our communities in the digital age.

Here are some extra stats to consider:

Around 550 million people use Twitter on average each month.
About 23% of adults worldwide use Twitter (according to Pew Research Center, 2023).
It's worth noting that the percentage of adults using Twitter can vary a lot depending on things like where you live, your age, and how easy it is for you to get online.

## *Including those affected*:

The project's scope encompasses the entire digital community actively or sporadically participating in Twitter conversations, sharing their views, opinions, and sentiments on specific topics. The analysis holds significant relevance, contingent upon the context and subject matter, for diverse entities such as businesses, brands, individuals, politicians, and various other groups.

Furthermore, this initiative extends its consideration to those directly influenced by or contributing to the discussions, ensuring a comprehensive understanding of the impact and implications for individuals, organizations, and communities engaged in the dynamic discourse on Twitter.

## *Proposed Data Science Solution*:

#### **Web Scraping**:
The method of extracting information from an online source, called Web Scraping, will be the following method for reconstruction the truncated dataset used in this project, which drags several data quality concerns. In this capstone, the analysis is aimed at focusing on political conversations, specifically from Twitter—a social media platform with high costs for extracting tweets. For this reason, the work of this project up to Spint 2, will be outsourced from pre-built datasets found on [Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets). For Sprint 3, the dataset will be scraped. 

Web scraping will be performed using the Twitter API within the Postman web application.

#### **Exploratory Data Analysis*:
*Libraries Used*

- Numpy: To perform array mathematical computations.
- Pandas: A library to process data.
- Matplotlib: Data Viz
- Seaborn: Data Viz

#### **Tokenizing**:

To clean and preprocess text data, specifically tweets various techniques  commonly used in Natural Language Processing (NLP) and text analysis, are employed to enhance the quality and relevance of the text data. Let's break down the steps involved in the clean_tweets function:

**Import Libraries**:

imports necessary libraries, including nltk for natural language processing and re for regular expressions.

**Create a Lemmatizer**:

A lemmatizer from the nltk library is instantiated. Lemmatization involves reducing words to their base or root form, considering the context.

**Define the Cleaning Function**:

The clean_tweets function is defined, taking a tweet as input.

**Text Cleaning Steps**:

**Removing Handles, Hashtags and Mentions**:

Using regular expressions, the function removes Twitter handles (e.g., "@username") from the tweets.
Removing Hashtags and Associated Words:

Another regular expression is used to eliminate hashtags and words that come together with hashtags from the tweets.

**Removing Punctuation and Links**:

Punctuation and special characters, including hashtags, are removed from the tweets. Additionally, hyperlinks (URLs) are eliminated.
Lowercasing:

All characters in the tweet are converted to lowercase to standardize the text.

**Removing Extra Whitespace**:

Extra whitespace is removed by joining the words in the tweet.

**Removing Stopwords**:

Common stopwords (e.g., 'the,' 'a,' 'an') are removed using the stopwords list from the nltk library.

**Lemmatization**:

The lemmatization process is applied to convert words to their base form, enhancing the coherence of the text.

**Handling Ellipsis**:

The function removes three dots at the end of the final word, including the deletion of the truncated word itself.

**Applying the Cleaning Function**:

The clean_tweets function is applied to a column of tweets in the dataframe (df_cleaned), and the cleaned text is stored in a new column called 'Clean_Tweet.'
This function encapsulates a series of preprocessing steps that are crucial for preparing text data for analysis. It aligns with the general principles outlined in the provided explanation of extracting basic and advanced features from text data in the context of Natural Language Processing.

**Sentiment Analysis**:

The analysis we want to implement once all the previous steps are done, and the data has been processed as required.

[Dealing with Text Data](https://www.kaggle.com/code/prashant111/a-beginners-guide-to-dealing-with-text-data)

#### **Clustering**:

There are at least six distinctive structures of social media crowds that form depending on the subject being discussed, the information sources being cited, the social networks of the people talking about the subject, and the leaders of the conversation. Each has a different social structure and shape: divided, unified, fragmented, clustered, and inward and outward hub and spokes.

#### **Logistic Regression**:

The correlation between categorical values is computed to discern whether specific variables or words can serve as reliable indicators of whether a tweet or handle belongs to either a Democrat or a Republican. In the logistic regression model, the target variable is the Is_Democrat column, which has been binarized (1 for Democrat and 0 for Republican).

The logistic regression model is trained using the cleaned tweets and the hashtags column to model and predict the political party affiliation (Is_Democrat). This predictive model leverages the cleaned textual content and the presence of specific hashtags as features to classify tweets as either Democratic or Republican. The target variable (Is_Democrat) serves as the binary outcome for the logistic regression, capturing the political alignment associated with each tweet or handle.

#### **Other Models**:

A pipeline has been implemented to model the classification of tweets or handles as either Democrat or Republican using the Naive Bayes and Random Forest algorithms. In this approach, the target variable for both models is the `Is_Democrat` column, which has been binarized to represent Democrats as 1 and Republicans as 0.

For the Naive Bayes model, the pipeline integrates text processing techniques such as Count Vectorization, a method based on the SciKitLearn library, which captures the unique words and their counts from the cleaned tweets and hashtags. This vectorized representation is then used as input for the Naive Bayes algorithm, aiding in the prediction of political affiliations based on the probabilistic nature of word occurrences.

Similarly, the Random Forest model is incorporated into the pipeline, leveraging the same textual features. Random Forest, implemented via SciKitLearn, is a versatile ensemble learning method that utilizes multiple decision trees to make predictions. The pipeline streamlines the process of feature extraction, vectorization, and model training, enhancing the efficiency of the analysis.

Both pipelines contribute to the comprehensive exploration of political discourse on Twitter by employing distinct machine learning algorithms to predict political affiliations. The binarized `Is_Democrat` column serves as the target variable for these models, facilitating the classification of tweets into either Democratic or Republican categories based on the learned patterns from the text data and hashtags.

## *Impact of your solution*:

The proposed solution holds the potential to significantly impact various sectors by offering a nuanced understanding of public sentiment and discourse on Twitter, particularly in the realm of politics. Through advanced text data analysis and clustering techniques, the project aims to uncover patterns, trends, and sentiment dynamics within the digital community. This insight is invaluable for businesses and brands seeking informed decision-making, politicians refining communication strategies, and individuals or groups aiming for enhanced community engagement. Additionally, the solution may contribute to academic advancements in social media studies, offering a comprehensive exploration of online conversations. By identifying emerging trends and providing a potential foundation for early warning systems, the project stands to empower stakeholders with timely and relevant information, fostering a more informed, targeted, and proactive approach to navigating the dynamic landscape of Twitter discussions on political topics.

## *Description of your dataset*:

[Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets) 

This publicly available dataset on Kaggle provides a comprehensive collection of tweets extracted from Twitter, covering the years 2017-2018. The dataset includes tweets from representatives of both the Democratic and Republican parties in the USA, organized into three essential columns: Political Party, Handle, and Tweet.

However, it's crucial to highlight a significant data quality issue within the dataset. Many tweets, especially those exceeding a certain length, have been truncated, leading to a loss of contextual information. This truncation poses challenges for comprehensive sentiment analysis and may impact the accuracy of interpreting the intended message within each tweet.

In response to these challenges, key modifications have been implemented to enhance the dataset:

1. **Creation of Is_Democrat Column**:

To facilitate predictive modeling, a new column named Is_Democrat was introduced. This binary column binarizes political party affiliations, assigning a label of 1 to tweets associated with the Democratic Party and 0 to those linked to the Republican Party.

2. **Tokenization and Text Cleaning**:

In recognition of the importance of robust text processing, all tweets underwent tokenization and thorough cleaning. This process involved removing handles, hashtags, links, punctuation, and unnecessary whitespace. Additionally, a lemmatization step transformed words into their base form, promoting uniformity in the dataset. The resulting cleaned text was saved in a dedicated column named Cleaned_Tweets.

The decision to scrape additional data in the upcoming sprint is driven by the acknowledgment of limitations imposed by the truncated dataset, particularly concerning sentiment analysis. Truncated tweets may lack the full context and nuances needed for a comprehensive sentiment analysis. Obtaining a more comprehensive and representative dataset through scraping aims to address this limitation, enabling a more accurate exploration of sentiment trends and patterns within political discourse on Twitter. This iterative approach reflects a commitment to refining data quality and enhancing the robustness of subsequent analyses

### Data Dictionary

Some important files, variables and features to take in consideration. 
#### Files

- **1_EDA_Capstone.ipynb**: File with initial EDA on the original dataset.
- **Sprint_2_Capstone.ipynb**: File with further analysis after Sprint 1 Feedback.
- **ExtractedTweets.csv**: Original dataset with 3 columns Party, Handle and Tweet

  #### Variables and Features
  
- **duplicate_tweets**: Shows ALL of the duplicate Tweets.
- **df**: Original DataFrame which is outdated throughout the 1_EDA_Capstone.ipynb file.
- **df_cleaned**: New DataFrame with the updated features and columns.
- **republican_hashtags**: List with all hashtags for republican senators.
- **democrat_hashtags** : List with all hashtags for democrat senators.
- **Retweet column**: Binarized column showing 1 for retweet and 0 for not retweet.
- **Is_Democrat column**: Binarized column showing 1 for democrat and 0 for republican.
- **Hashtags column**: List of hashtags appearing in each tweet.
