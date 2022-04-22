# sentiment-analysis
Sentiment Analysis in Excel with Azure Machine Learning
Sebastian Obeta
Sebastian Obeta
Jun 16 · 5 min read

sebastian-obeta




There is an important difference between language and most other kinds of things people think of when they do signal processing, data mining, etc. Most things are sort of random data gotten and someone trying to make sense out of it. Fundamentally, human language is not like massive data, exhaustive that someone is trying to process something useful. It is a system design specifically to convey the speaker’s or writer’s meaning. It is not just an environmental signal, but a deliberate form of communication. An amazing side of human language is that it is a complex system with an encoding format that a kid can quickly learn.


Sentimental analysis is a field that could be called motion mining. Companies and businesses have exploited in discovering people’s opinions, emotions, and feelings about a certain product or service. It could be through review sites, blogs, forums, or social media. Application of NLP helps a business to gain more insights on consumers, create a competitive edge necessary for business decisions and growth.

For example, some survey generates feedbacks from and in turns gives insight to the providers on how to meet the need of the customer. They are polarized, could base on sentiment (feelings and emotions) as good or bad, positive or negative.

If I want to download a new app, my first point of call is to check the rating on those apps and comments. There are different types of sentiment analysis and you can read it up below.

https://monkeylearn.com/sentiment-analysis/

With sentiment analysis, you will get a real-time analysis. For example, during the COVID 19 lock-down, you can do a sentiment analysis of what people say on social media to know the impact of the spread, how people are faring, where government palliative was palliative enough to the masses?. You can imagine if you go to tweeter to checking the trending topics with your area, you will be overwhelmed with the streams of data that come in per second, and processing those data manually will be hectic. Sentiment analysis can inform an individual, business, mitigate the crisis, etc.
It can be used for customer service purposes, Market research, Social media monitoring, etc.

How does Sentiment analysis works?

There are different algorithms in sentiment analysis but the popular once are rule-based, Hybrid, and automated systems.
Image for post
Image for post
Architecture of Sentiment Analysis (Monkey Learn)

All of the above explains how it works but you read the full details below. https://monkeylearn.com/sentiment-analysis/.

Classification algorithms are the part of the machine learning stage and classifier model however, all of this embedded in its azure machine learning.

The first point of call will be to get your datasets and populate it in excel. How to get to generate and excel will be shared in the next episode of Text classification. We will use Twitter data available on Kaggle for this demonstration. The link to the dataset is https://www.kaggle.com/jl18pg052/tweets-for-georgefloydfuneral/tasks?taskId=1132

Description of the dataset: We want to do sentiment analysis on what people are saying and how they felt during George Floyd’s funeral about 200 tweets not much but to show how sentiment analysis can be done on Excel.
Image for post
Image for post
George Floyds Funeral tweets (Kaggle)

Next, you need to add a Text sentiment analysis add-on on excel. On Home Tab, click on Insert Tab, and click on the store as shown in the colored below.

A dialogue box pops up as shown below, you search for Azure Machine learning.
Image for post
Image for post
Azure Machine Learning Add- on

You click on Add, accept the license terms and privacy policy,

It is added to your excel workbook at the left-hand side, you select, sentiment analysis
Image for post
Image for post
Text Sentiment add-on

The sentiment analysis is added as shown below with two categories.

1. View schema

2. Predict

3. Errors.

If you collapse the view schema, you will Input, Output, and Global Parameter.
Select the Inputs and select input 1, you will see “tweet text”. Please change the header on your excel sheet to “tweet text”
Next is to click on the Predict, under input 1, select cell number 1, and drag into the last cell. You can type it and it is as follows.
Name of the sheet! First cell and last cell. In this work, it is as follows

George!A1:A201

Please leave at least two columns after the “tweet_text” Colum where the result will be populated.
On the Output tab under Predict, select where column where the wanted the result to be populated. For this project, I have column B empty. The output will take the form of the input but the cell will change.

George!B1.
Image for post
Image for post
Parameter Setting for Azure Machine Learning

Click predict and your result is out. With a sentiment and its score.

You have your score. You will have over view of the score in percentage by formatting the column. You can know the count of positive by using pivot and manipulating it. You can check for the average, check for word count. Watch out for the next article on word cloud with excel.
Image for post
Image for post

Conclusion

If you have survey data with multiple choice entry, you can use pivot table, but for free form text like tweets, chats it is hard to process. You will need a machine learning system which is provided by Azure. Click and follow to get the next update on how to do word cloud on Excel. Next time you have a large amount of data to analyze, consider Azure Machine Learning.
