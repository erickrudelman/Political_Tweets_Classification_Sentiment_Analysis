# Tweet_Sentiment_Analysis_Capstone

## **Project Overview**
Social Listening is a powerful method for understanding public sentiment. In the past, surveys were the primary means of gauging public opinion on specific topics. However, today, a more organic approach involves monitoring online conversations to glean real-time insights. Social Listening, achieved through the extraction and analysis of thousands, and ideally millions, of comments on social media platforms, has emerged as an effective way to gather data and empower businesses, individuals, and brands.

When engaging in Social Listening, both quantitative and qualitative information can be delivered to comprehensively grasp the dynamics of the digital world. By tracking online discussions, one can decipher what people are saying, when, and why. These insights are invaluable for tailoring strategies to target audiences effectively.

### **Project Scope**

In this project, I undertake a comprehensive analysis of political discourse on Twitter, guiding the exploration through various key stages. The initial phase involves independent collection of a dataset of political tweets using the Twitter API V2. Following this, my focus turns to effective tokenization and preprocessing techniques, leveraging natural language processing to enhance the granularity and cleanliness of the data.

Moving forward, my efforts center around developing a Logistic Regression model for tweet classification, with the primary goal of categorizing tweets into Democrat or Republican affiliations. Notably, I prioritize interpretability in the model to glean insights into feature importance.

Simultaneously, I delve into sentiment analysis using the TextBlob library, offering nuanced perspectives on the emotional tone embedded in political tweets. Feature engineering takes center stage as well, where I extract and categorize hashtags to not only enhance model performance but also understand their significance in the context of the analysis.

Statistical rigor is applied through hypothesis testing to discern any significant differences in sentiment between tweets from Democrats and Republicans. Model evaluation becomes pivotal, involving metrics such as accuracy, precision, recall, and F1-score.

Concluding the project is the development of a real-time tweet analysis function, enabling users to input a tweet, tokenize it, classify its political affiliation, and conduct sentiment analysis. This dynamic functionality adds practical utility to the exploration of online political discourse.

In summary, this project synthesizes data scraping, tokenization, machine learning models, statistical analyses, and real-time tweet analysis to offer nuanced insights into the dynamics of political conversations on Twitter.

### **Objectives**
This project focuses on analyzing political conversations on Twitter, specifically targeting members of the House of Representatives from both the Democrat and Republican parties in the USA. The primary objectives are outlined as follows:

**1. Data Collection with Twitter API V2:**
   - Independently collect a dataset by leveraging the Twitter API V2 to gather political tweets from members of the house of representatives of both the Democrat and Republican parties.

**2. Feature Engineering:**
   - Implement feature engineering techniques to enhance model performance, including the extraction and categorization of hashtags.
   - Explore the significance of hashtags in predicting party affiliation and sentiment.

**3. Tokenization and Preprocessing:**
   - Implement tokenization techniques to break down tweets into individual words, enhancing the granularity of the analysis.
   - Employ natural language processing for efficient handling of textual data.
   - Clean and preprocess the collected tweets to remove noise and irrelevant information.

**4. Tweet Classification:**
   - Develop and train a tweet classification model to predict the party affiliation (Democrat or Republican) based on the content of the tweets.
   - Utilize natural language processing techniques for tokenization, cleaning, and vectorization of tweets.
   - Employ a Logistic Regression, TF-IDF, Word Embedding, Random Forest and SVM to test for the best classification model, and enhance interpretability based on the best performaning model.

**5. Sentiment Analysis:**
   - Conduct sentiment analysis on the tweets to discern the overall sentiment of the online speech from Democrats and Republicans.
   - Utilize the TextBlob library for sentiment analysis, considering both polarity and subjectivity of the tweet content.

**6. Hypothesis Testing:**
   - Perform hypothesis testing to assess whether there are statistically significant differences in sentiment between tweets from Democrats and Republicans.
   - Utilize statistical tests to validate the observed differences and provide a robust foundation for interpreting sentiment variations.

**7. Model Evaluation and Interpretability:**
   - Evaluate the classification model's performance using metrics such as accuracy, precision, recall, and F1-score.
   - Emphasize model interpretability to derive insights into the features contributing to predictions.

**8. Real-time Tweet Analysis:**
   - Develop a function to classify and analyze individual tweets in real-time.
   - Allow users to input a tweet, tokenize it, classify the political affiliation, and perform sentiment analysis.

By focusing on Senators' tweets and employing a combination of traditional machine learning and advanced modeling techniques, this project aims to gain insights into the sentiments and political affiliations expressed on Twitter. The comprehensive approach includes data cleaning, feature engineering, and the application of diverse models, setting the foundation for potential future advancements in the analysis of political discourse on social media.

## *Areas of Interest Submission*:

The submitted Area of Interest is dedicated to conducting a comprehensive analysis of Twitter conversations, with a specific focus on the domain of politics. The overarching objective is to systematically process the vast amount of data generated from these conversations through a series of well-defined steps.

The first stop is data scraping and cleaning, where tweets are transformed into a standardized format. I begin by tokenizing, breaking them down into individual words and hashtags. This is followed by converting everything to lowercase and removing unnecessary elements like punctuation, user handles, and stop words. Finally, I eliminate distracting links to streamline the data and focus on the core content.

Once the data is clean, I extract valuable features that will aid in our analysis. This step, known as feature engineering, involves techniques like Count Vectorizer, which identifies the frequency of words and hashtags. This frequency data paints a picture of the most prominent vocabulary used within different political factions, revealing insights into their communication styles and potential alignments.

Armed with these meaningful features, I delve into the heart of the analysis: classification. Utilizing a range of powerful models tested throughout the project, I aim to categorize each tweet based on its political leaning. This classification paints a vivid picture of the prevailing discourse, highlighting dominant narratives and potential shifts in public opinion. By analyzing the distribution of tweets across different categories, I uncover valuable insights into the evolving landscape of political thought on Twitter.

Having classified the tweets, the project delves deeper into the emotional undercurrents by performing sentiment analysis. This allows us to gauge the prevailing sentiment within each political group and across the entire Twittersphere. Are discussions generally hopeful, anxious, or angry? How do these sentiments differ across groups? By understanding the emotional landscape, we gain a richer understanding of the motivations and reactions embedded within political discourse.

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

For data acquisition, I independently conducted scraping using the Twitter API V2, focusing on retrieving political tweets. The Twitter API V2 allowed for efficient and targeted collection, enabling the extraction of valuable information from the platform. This approach facilitated the creation of a diverse and comprehensive dataset, essential for subsequent analyses. The use of the Twitter API V2 provided real-time access to tweets, ensuring the inclusion of the latest and most relevant data in the project.

#### **Exploratory Data Analysis**:
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


#### **Modelling for Classification**:

In the pursuit of optimal tweet classification, I employed various models in my analysis, including Logistic Regression, TF-IDF, Word Embedding, Random Forest, and Support Vector Machine (SVM). These models underwent extensive testing and evaluation to identify the best performer for categorizing tweets into Democrat or Republican affiliations. The evaluation process involved assessing accuracy, precision, recall, and F1-score metrics on both training and testing datasets. Through meticulous parameter tuning and feature scaling, the Logistic Regression model emerged as the top performer, achieving a balanced accuracy rate and demonstrating its effectiveness in capturing intricate patterns within the political tweet dataset.

**Sentiment Analysis**:

In the realm of sentiment analysis, I utilized TextBlob sentiment analysis to gauge the emotional tone of political tweets. This approach involved assigning sentiment scores to tweets, providing insights into their positivity or negativity. 

**Hypothesis Tesing**:

Hypothesis test was conducted to determine statistically significant differences in sentiment between Democrats and Republicans. The t-statistic and p-value derived from the test indicated that, on average, tweets from Democrats exhibited slightly higher sentiment compared to those from Republicans. This statistical analysis enriched our understanding of the nuanced emotional dynamics within political discourse on Twitter.

## *Impact of your solution*:

The proposed solution holds the potential to significantly impact various sectors by offering a nuanced understanding of public sentiment and discourse on Twitter, particularly in the realm of politics. Through advanced text data analysis and clustering techniques, the project aims to uncover patterns, trends, and sentiment dynamics within the digital community. This insight is invaluable for businesses and brands seeking informed decision-making, politicians refining communication strategies, and individuals or groups aiming for enhanced community engagement. Additionally, the solution may contribute to academic advancements in social media studies, offering a comprehensive exploration of online conversations. By identifying emerging trends and providing a potential foundation for early warning systems, the project stands to empower stakeholders with timely and relevant information, fostering a more informed, targeted, and proactive approach to navigating the dynamic landscape of Twitter discussions on political topics.

## *Description of your dataset*:

In the first step of dataset creation, the Twitter handles of all U.S. Senators were gathered from (Official Twitter Handles from Members)[https://pressgallery.house.gov/member-data/members-official-twitter-handles], converted into a dataframe, and then used to fetch corresponding user_ids. This process involved multiple steps documented in the 'twitter_hacking.ipynb' notebook, including querying usernames with the Twitter API v2 via Postman and merging the obtained information into a comprehensive CSV file named 'PoliticalUsernamesAndIds.csv'. The resulting CSV included user_ids, names, and usernames, with party affiliations mapped based on the initial list extracted from the HTML. This file served as the foundation for the subsequent scraping of tweets.

In the second step, the 'Tweet_extractor.ipynb' notebook was employed to extract up to 23 tweets from each user_id's timeline using the Twitter API v2. This resulted in multiple JSON files, including 'tweets.json', 'tweets1_2.json', and 'RepAdamas.json'.

The third step involved compiling the extracted tweets into a consolidated dataset. The 'json_files_compiler.ipynb' notebook orchestrated the merging of individual JSON files into the final dataset labeled '3.RepublicanVsDemocratNew.json'. This was converted to CSV afterwards.

The dataset, initially comprising user_ids and tweets, underwent enhancements. Additional columns were introduced, such as usernames, party affiliations ('Party'), hashtags, and an 'is_retweet' indicator. This comprehensive dataset captures a diverse range of political tweets from U.S. Senators, providing a rich resource for subsequent analyses.

### Data Dictionary and Documents

Some important files, variables and features to take in consideration. 
##### *Modelling Notebooks*:
- **1_EDA_Capstone.ipynb**: File with initial EDA on the original dataset.
- **Sprint_2_Capstone.ipynb**: File with further analysis after Sprint 1 Feedback.
- **Sprint_3.ipynb**: Final capstone project

###### *Twitter Scraping Notebooks* 
- **twitter_hacking.ipynb**: Notebook with code to extract all US Senator's Twitter username's and use this results to scrape the user_id from each username.
- **Tweet_extractor.ipynb**: Python robot that loops over all user_ids and extracts tweets.
- **json_files_compiler.ipynb**: Code that compiles all json files.

###### *JSON Files*
- **RepAdamas.json**: Tweets extracted only for user RepAdams. It was done separately in postman for result testing.
- **tweets1_2.json**: Tweets extracted from the following 2 usernames, following RepAdams, using the *Tweet_extractor.ipynb* code. Code was ran on only these 2 users for testing purpose. Execution was successfull.
- **tweets.json**: Tweets extracted from all of the other 423 user's using the *Tweet_extractor.ipynb* code.
- **RepublicanVsDemocratNew.json**: file compiling the tweets from tweets1_2.json and tweets.json. The ones from RepAdamas.json came in a different format so they were compiled separately.
- **3.RepublicanVsDemocratNew.json**: file compiling the RepublicanVsDemocratNew.json with the RepAdamas.json. This is the **final** file compiling all tweets in the dataset.

###### *CSV Files*
- **ExtractedTweets.csv**: Original dataset extracted from Kaggle with 3 columns Party, Handle and Tweet. 
- **PoliticalUsernamesAndIds.csv**: Dataset with all usernames, user_ids and party affiliation. Used as main source to scrape tweets and build the dataset.
- **RepublicanVsDemocrat.csv**: **Final** dataset scraped from scratch. This is the dataset used for the project, containing roughly 10,000 tweets.

#### Variables and Features
  
- **duplicate_tweets**: Shows ALL of the duplicate Tweets.
- **df**: Original DataFrame which is outdated throughout the 1_EDA_Capstone.ipynb file.
- **df_cleaned**: New DataFrame with the updated features and columns.
- **republican_hashtags**: List with all hashtags for republican senators.
- **democrat_hashtags** : List with all hashtags for democrat senators.
- **is_retweet column**: Binarized column showing 1 for retweet and 0 for not retweet.
- **Is_Democrat column**: Binarized column showing 1 for democrat and 0 for republican.
- **Hashtags column**: List of hashtags appearing in each tweet.

