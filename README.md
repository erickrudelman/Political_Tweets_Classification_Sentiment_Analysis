# tweet_sentiment_analysis_capstone
Scrape conversation on Twitter based on Keywords or Hashtags and perform Sentiment Analysis

Just checking if I could commit the changes in this file to the remote repo.

The Capstone Repo contains a README file with pre-existing **headers and bullet points** to help guide your thoughts. You are required to fill this file in with a **Project Overview**. The overview should reflect the structure of your:

- *Areas of Interest Submission*:
- *explaining the Problem Area*:
- *including those affected*:
- *proposed Data Science solution*:
- *impact of your solution*:
- *description of your dataset*:

Any changes or refinements to your Area of Interest should be reflected in the README, and it is expected that your description of the data will be more granular (including a Data Dictionary if feasible) compared to the Area of Interest submission.

Thursday 21 of Dicember:
- Finish text data notebook
- Read all articles
- Scrape twitter conversations

Sunday 24th of December:

Cover the scope of the project, define the objectives, framework and methodology. 
- Finish the README file and start defining the dataset

Monday 25th of December:
Download the dataset, pre-process the data and perform some EDA to determine data issues, feature engineering opportunited and other observations.
- Prepare the Jupyter Notebook

Tuesday 26h of December
- Presentation 

-------------------------------------------
## **Project Overview**
Social Listening is a powerful method for understanding public sentiments. In the past, surveys were the primary means of gauging public opinion on specific topics. However, today, a more organic approach involves monitoring online conversations to glean real-time insights. Social Listening, achieved through the extraction and analysis of thousands, and ideally millions, of comments on social media platforms, has emerged as an effective way to gather data and empower businesses, individuals, and brands.

When engaging in Social Listening, both quantitative and qualitative information can be delivered to comprehensively grasp the dynamics of the digital world. By tracking online discussions, one can decipher what people are saying, when, and why. These insights are invaluable for tailoring strategies to target audiences effectively.

### **Scope**
The scope of this project extends beyond Social Listening and initiates with the acquisition of a robust dataset of Twitter conversations. Ideally, these conversations would be directly scraped from Twitter using the Twitter API. However, due to high associated costs, an alternative dataset has been obtained from _______.

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

Around 550 million people use Twitter on average each month (that's our best estimate).
About 23% of adults worldwide use Twitter (according to Pew Research Center, 2023).
It's worth noting that the percentage of adults using Twitter can vary a lot depending on things like where you live, your age, and how easy it is for you to get online.

## *Including those affected*:

The project's scope encompasses the entire digital community actively or sporadically participating in Twitter conversations, sharing their views, opinions, and sentiments on specific topics. The analysis holds significant relevance, contingent upon the context and subject matter, for diverse entities such as businesses, brands, individuals, politicians, and various other groups.

Furthermore, this initiative extends its consideration to those directly influenced by or contributing to the discussions, ensuring a comprehensive understanding of the impact and implications for individuals, organizations, and communities engaged in the dynamic discourse on Twitter.

## *Proposed Data Science solution*:

#### **Web Scraping**: 
The method of extracting information from online source called Web Scraping would've been the preffered method of building the dataset used for this project. In this capstone, the analysis is aimed to be directed to political conversation specifically from Twitter, social media platform that has very high costs for extracting tweets. For this reason, this critical part of the project will be outsourced from pre-built  datasets found on ______.

#### **Exploratory Data Analysis**:
*Libraries used*
    - Numpy: Perform array mathematical computations
    - PandasL Library to process data

  
#### **Natural Language Processing**: 

*Extracting basic features from text data*
Designing and building an algorithm with pre-built libraries in order to understand the meaning of words and translate their meaning into other valuable interpretations such as a Sentiment Analysis of the words.

In the process of working with text, a **count of words** is a very important step, to determine the amount of words in each tweet. This is a very useful fisrt step in determining if the tone of the teet is either positive or negative. Just as the words, the characters can be counted with the same purpose.

**Removing the stopwords** is also a common used practice before processing text. These inclued words such as 'the', 'a', 'an', 'in', etc. The *nltk* library is used for this instances. It allows for the text to be processed in the desired language.

Another practice used in NPL is **extracting the amount of special characters** in the text, such as hashtags, which bring valuable information about the text we are dealing with. 

**Identifying uppercase** words is also a valuable practice since uppercase words are often associated with expresions of anger and rage. Implementing this practice helps bring value to the analysis of the text.

*Pre-processing steps to clean the data and obtain valuable features*
The following Data Science techniques are included in the Natural Language Processing of this project.
   
**CountVectorization** Method based on a *SciKitLearn* library implemented to obtain each unique word from the text-data and the count for each words. When counting words, a common practice is to group them by amount, either 2 or 3, so instead of the CountVectorizar return each word separately, it can return a sequence of words that only make sense together.

**Hashing Vectorization** is the practice of converting the text to a matrix counting the amount of token occurrences (count of unique words in the text data).

**Stemming** is the method of removing suffices which change the tense of the word but not its meaning. When analyzing text in NLP, we aim for the base form of it, so removing suffices helps group words of the same root into one. 

**Lemmatization** is a method similar to stemming, in which words are processed to its base form, however, in a lemmatization process words are converted to its root depending on the context of the word, as opossed to stemming where it only cuts off the suffix of thw rods. 

*Advanced text processing*

**N-grams** is an dvanced text processing technique where algorithsm are used to predict which word/s are most likely to follow a given word. It is implemented using the *textblob* library 

**Term Frequency** is the method of obtaining the ratio of the count of words in a specific frame of text, to the length of the that text.

**Sentiment Analysis** is the analysis we want to implement once all of the previous steps are done and data has been processed as requiered. 

#### **Clustering**:

There are at least six distinctive structures of social media crowds which form depending on the subject being discussed, the information sources being cited, the social networks of the people talking about the subject, and the leaders of the conversation. Each has a different social structure and shape: divided, unified, fragmented, clustered, and inward and outward hub and spokes.

## *Impact of your solution*:

The proposed solution holds the potential to significantly impact various sectors by offering a nuanced understanding of public sentiment and discourse on Twitter, particularly in the realm of politics. Through advanced text data analysis and clustering techniques, the project aims to uncover patterns, trends, and sentiment dynamics within the digital community. This insight is invaluable for businesses and brands seeking informed decision-making, politicians refining communication strategies, and individuals or groups aiming for enhanced community engagement. Additionally, the solution may contribute to academic advancements in social media studies, offering a comprehensive exploration of online conversations. By identifying emerging trends and providing a potential foundation for early warning systems, the project stands to empower stakeholders with timely and relevant information, fostering a more informed, targeted, and proactive approach to navigating the dynamic landscape of Twitter discussions on political topics.

## *Description of your dataset*:
