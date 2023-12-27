# Tweet_Sentiment_Analysis_Capstone

## **Project Overview**
Social Listening is a powerful method for understanding public sentiments. In the past, surveys were the primary means of gauging public opinion on specific topics. However, today, a more organic approach involves monitoring online conversations to glean real-time insights. Social Listening, achieved through the extraction and analysis of thousands, and ideally millions, of comments on social media platforms, has emerged as an effective way to gather data and empower businesses, individuals, and brands.

When engaging in Social Listening, both quantitative and qualitative information can be delivered to comprehensively grasp the dynamics of the digital world. By tracking online discussions, one can decipher what people are saying, when, and why. These insights are invaluable for tailoring strategies to target audiences effectively.

### **Scope**
The scope of this project extends beyond Social Listening and initiates with the acquisition of a robust dataset of Twitter conversations. Ideally, these conversations would be directly scraped from Twitter using the Twitter API. However, due to high associated costs, an alternative dataset has been obtained from [Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets).

Following an analysis of the dataset to identify data quality issues, feature engineering opportunities, and other notable observations related to data processing, the data will undergo preprocessing for further analysis. The initial analysis will involve Sentiment Analysis to categorize conversations into positive, negative, or neutral tones. Additionally, features such as counts of the most positive and negative words, word cloud representations, and other descriptive visualizations will be extracted.

Furthermore, a clustering analysis will be conducted to develop a functional algorithm trained on pre-existing datasets. This algorithm will later identify new topic-related comments and assess the sentiment's alignment with the existing clusters. Can it accurately predict the cluster to which a new tweet belongs?

For the clustering algorithm, pre-labeled datasets have been extracted to generate features for either Democrats or Republicans. The goal is to identify words indicative of political alignment, commonly used by each group (e.g., "pro-life" or "pro-choice").

Additionally, a Logistic Regression, implemented in the form of a CountVectorizer, will convert political labels into binary forms. The input for the Logistic Regression will be vectorized text. Can the model accurately determine if a tweet is Democratic or Republican based on word counts?

### **Objectives**
This project focuses on a dataset containing political conversations on Twitter with the following objectives:

Extract Democrat vs. Republican Twitter conversations from a pre-built dataset.
Implement Sentiment Analysis on the tweets in the dataset.
Develop and apply a Clustering Algorithm to classify tweets as Democrat, Republican, or Neutral.

## *Areas of Interest Submission*:

The submitted Area of Interest centers around the comprehensive analysis of Twitter conversations, particularly within the domain of politics. The primary objective is to process the voluminous data generated from these conversations through a series of methodical steps.

Firstly, the data will undergo a meticulous cleaning process, aimed at refining its quality and ensuring that subsequent analyses are based on reliable information. Following this, the extraction of valuable features from the cleaned dataset will be undertaken, contributing to a more nuanced understanding of the political discourse on Twitter.

The analysis will encompass both basic and advanced techniques in text data analysis. This multifaceted approach seeks to uncover patterns, trends, and underlying themes within political tweets, providing a rich foundation for subsequent investigations.

A pivotal aspect of this endeavor involves the implementation of Sentiment Analysis. This analytical tool will be employed to discern and categorize the prevailing sentiments expressed in political tweets, thereby shedding light on the overall tone and mood within the Twitter political sphere.

Moreover, a clustering analysis will be conducted to discern inherent groupings within the dataset. The objective is to train robust datasets of political tweets through the identification of commonalities, allowing for the creation of distinct clusters. This, in turn, will enable the categorization of future tweets into relevant clusters, facilitating a dynamic understanding of evolving patterns and affiliations within the realm of political discourse on Twitter.

By integrating these methodologies, the ultimate goal is to offer a comprehensive and insightful exploration of political conversations on Twitter, leveraging both qualitative and quantitative analyses to enhance our understanding of the complex dynamics at play within this digital space.

## *Explaining the Problem Area*:

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
The method of extracting information from an online source, called Web Scraping, would have been the preferred method for building the dataset used in this project. In this capstone, the analysis is aimed at focusing on political conversations, specifically from Twitter—a social media platform with high costs for extracting tweets. For this reason, this critical part of the project will be outsourced from pre-built datasets found on [Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets).

#### **Exploratory Data Analysis*:
*Libraries Used*

- Numpy: To perform array mathematical computations.
- Pandas: A library to process data.

#### **Natural Language Processing**:

*Extracting basic features from text data*

Designing and building an algorithm with pre-built libraries to understand the meaning of words and translate their meaning into other valuable interpretations, such as Sentiment Analysis of the words.

In the process of working with text, a **count of words** is a crucial step in determining the number of words in each tweet. This is a useful first step in establishing whether the tone of the tweet is positive or negative. Just like words, characters can be counted for the same purpose.

**Removing stopwords** is also a commonly used practice before processing text. These include words such as 'the,' 'a,' 'an,' 'in,' etc. The *nltk* library is used for these instances. It allows the text to be processed in the desired language.

Another practice in NLP is **extracting the number of special characters** in the text, such as hashtags, which provide valuable information about the text being analyzed.

**Identifying uppercase words** is also a valuable practice since uppercase words are often associated with expressions of anger and rage. Implementing this practice adds value to the text analysis.

*Pre-processing steps to clean the data and obtain valuable features*

The following Data Science techniques are included in the Natural Language Processing of this project.

**CountVectorization** Method based on the *SciKitLearn* library, implemented to obtain each unique word from the text data and the count for each word. When counting words, a common practice is to group them by amount, either 2 or 3, so instead of the CountVectorizer returning each word separately, it can return a sequence of words that only make sense together.

**Hashing Vectorization** is the practice of converting the text to a matrix, counting the number of token occurrences (count of unique words in the text data).

**Stemming** is the method of removing suffixes that change the tense of the word but not its meaning. When analyzing text in NLP, we aim for the base form of it, so removing suffixes helps group words of the same root into one.

**Lemmatization** is a method similar to stemming, in which words are processed to their base form. However, in lemmatization, words are converted to their root depending on the context of the word, as opposed to stemming, where it only cuts off the suffixes of the words.

*Advanced text processing*

**N-grams** is an advanced text processing technique where algorithms are used to predict which word(s) are most likely to follow a given word. It is implemented using the *textblob* library.

**Term Frequency** is the method of obtaining the ratio of the count of words in a specific frame of text to the length of that text.

**Sentiment Analysis** is the analysis we want to implement once all the previous steps are done, and the data has been processed as required.

[Dealing with Text Data](https://www.kaggle.com/code/prashant111/a-beginners-guide-to-dealing-with-text-data)

#### **Clustering**:

There are at least six distinctive structures of social media crowds that form depending on the subject being discussed, the information sources being cited, the social networks of the people talking about the subject, and the leaders of the conversation. Each has a different social structure and shape: divided, unified, fragmented, clustered, and inward and outward hub and spokes.

#### **Logistic Regression**:

Correlation between categorical values is calculated to predict if any given variable or word can be a good indicator if the tweet or handle is either from a Democrat or a Republican.

## *Impact of your solution*:

The proposed solution holds the potential to significantly impact various sectors by offering a nuanced understanding of public sentiment and discourse on Twitter, particularly in the realm of politics. Through advanced text data analysis and clustering techniques, the project aims to uncover patterns, trends, and sentiment dynamics within the digital community. This insight is invaluable for businesses and brands seeking informed decision-making, politicians refining communication strategies, and individuals or groups aiming for enhanced community engagement. Additionally, the solution may contribute to academic advancements in social media studies, offering a comprehensive exploration of online conversations. By identifying emerging trends and providing a potential foundation for early warning systems, the project stands to empower stakeholders with timely and relevant information, fostering a more informed, targeted, and proactive approach to navigating the dynamic landscape of Twitter discussions on political topics.

## *Description of your dataset*:

[Republican vs Democrat Tweets](https://www.kaggle.com/datasets/kapastor/democratvsrepublicantweets) 

The dataset is publicly available on Kaggle and comprises data extracted from Twitter. It includes tweets from 2017-2018 from representatives of both the Democratic and Republican parties in the USA, organized into three columns:

- Political Party
- Handle
- Tweet

The dataset, once cleansed and transformed, contains 44,362 tweets associated to the Republican party and 42,041 tweets associated with the Democratic Party.
 
As indicated in the data source:

- Some tweets in ExtractedTweets.csv are not (as far as I can tell) associated with a representative's individual account. For instance, @RepublicanStudy represents a committee, not a specific representative.
- Tweets above a certain length were truncated to a length much shorter than what Twitter itself enforces.
  
Originally, the dataset contained 86,460 rows of data. However, it was cleaned and processed, resulting in 86,403 rows of data. The dataset initially included several duplicate tweets. Only those with repeated handles were removed, while duplicate tweets (mainly retweets) from different handles were treated as distinct tweets and retained in the dataset.

The following changes were implemented in the dataset:

- Checked for null values.
- Removed duplicate tweets where the handle was also duplicated.
- Created an "RT" binary column to mark all tweets that are retweets: 1 if it is a retweet, otherwise 0.
- Created a "Hashtags" column that displays all hashtags, if any, for every tweet.
- Created a list called "hashtag_list" containing all the hashtags that appear in the dataset.

### Data Dictionary

On the Repository you will find the "ExtractedTweets.csv" file. This is the original data set. After some Exploratory Data Analysis, new features were extracted and new columns were created, to transform the dataset into a new table saved into a file named "PoliticalTweets.csv". This analysis was performed in the file "1_EDA_Capstone.ipynb".

Some important files, variables and features to take in consideration 
#### Files

- **1_EDA_Capstone.ipynb**: File with initial EDA on the original dataset.
- **ExtractedTweets.csv**: Original dataset with 3 columns Party, Handle and Tweet
- **PoliticalTweets.csv**: New dataset created after initial EDA. This dataset will be the one used throughout the rest of the capstone project.

  #### Variables and Features
  
- **duplicate_tweets**: Shows ALL of the duplicate Tweets.
- **duplicates_with_different_handle**: Shows ALL of the duplicate Tweets which are coming from different handles.
- **df**: Original DataFrame which is outdated throughout the 1_EDA_Capstone.ipynb file.
- **df_cleaned**: New DataFrame with the updated features and columns.
- **hashtag_list**: A list with all of the hashtags that appear in the DataSet.
 
