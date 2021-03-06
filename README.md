## Introduction
You have reached my project portfolio page which continues to grow. I was very recently working in General Insurance (claims) as a Loss Adjuster - we go by other names like "adjuster", "surveyor" or "assessor". If you ever filed an insurance claim for your house, building, shop unit, warehouse, office, power plant, construction site, oil refinery, ship or aircraft, you would likely have met one of us. I have prior experience in consulting, software development and product development.

#### <a style="font-weight:bold" href="https://www.linkedin.com/in/irwinwei" target="_blank">Learn more about me or get in touch via LinkedIn</a>

The following are my projects to date, in **reverse chronological order** (most recent at the top).
<br><br>

### 2020

#### *Visualization of data used for the 2019 Capstone Project*
##### *Tableau |<a href="https://public.tableau.com/profile/irwinwei#!/vizhome/general-insurance-singapore-viz/Story1" target="_blank">> Link to visualization on Tableau Public </a>*
Visualization of the data that was downloaded from the Monetary Authority of Singapore to train the machine learning model in the capstone project. The purpose of the visualization is to obtain insights regarding the General Insurance market in Singapore.
<br><br>
*More projects to come.*
<br><br>

### 2019

#### *Capstone Project: Predicting Whether Insurance Underwriting Gain will be Negative*
##### *Regression | Classification | Unsupervised |<a href="https://www.github.com/irwinwei/GA-DSI-Capstone" target="_blank">> Link to project repository (see README file)</a>*
As my capstone project for the Data Science Immersive program at General Assembly, I took a deep dive into the annual returns submitted by Singapore-registered General Insurers to the Monetary Authority of Singapore (MAS). The returns for year 2005 and after are publicly available <a href="https://www.mas.gov.sg/statistics/insurance-statistics/insurance-company-returns" target="_blank">here</a>. Submission of these returns is mandatory and captures the financial data as at 31 December of the reporting year. At the time of the project, the latest data available was for 31 December 2018. <br><br>
For each General Insurer and for every year that they are active, their underwriting and investment performance (for Singapore-based risks) is summarized in a table named "Form 6 (SIF)" in the report, organized by insurance class (e.g. Fire, Motor, Health, Engineering etc). For each insurance class, a breakdown of financial components is provided i.e. premiums earned, claims paid, liabilities booked, management expenses, distribution expenses etc. The underwriting gain/loss and net investment income for each class are thus derived accordingly. <br><br>
The data was extracted from the PDF documents downloaded from MAS and processed for use by models for regression, classification and unsupervised learning (clustering).<br><br>
The main challenge faced was the coarse-granularity of this publicly available data, since this was just a 'snap shot' of the net result of the previous 12 months' activities. As such, it was difficult to cluster (unsupervised learning) the data in an interpretable/explainable way, and to apply a regression to predict the underwriting gain/loss.  A major factor was likely the disparity between the premiums collection schedule (typically on an annual basis) and claims paid/reserved schedule (which could span between weeks to years to resolve i.e. different time-scale from the corresponding premiums). <br><br>
However, the classification models (Logistic Regression, Extra Trees performed best) were able to perform better than the baseline accuracy of 68% with optimal tuning.<br><br>
As such, I am confident that far better results can be obtained (including regression) with finer-granularity data that General Insurers have on-hand, such as detailed claim statistics and other policy-specific data.<br><br>

#### *Project 4: Predicting the Presence of West Nile Virus*
##### *Classification |<a href="https://www.github.com/irwinwei/GA-DSI-Project-04" target="_blank">> Link to project repository (see README file)</a>*
We were required to study known cases of West Nile Virus presence in Chicago and to predict, based on weather and pesticide usage information, when the virus would be present i.e. the positive case being that the virus was present, and the negative case being that the virus was not present. The data used for this project was downloaded from this <a href="https://www.kaggle.com/c/predict-west-nile-virus/" target="_blank">Kaggle competition web page</a> and submitted to Kaggle web page for scoring. The score for classification was based on the area under the "ROC" curve (AUC).<br><br>
Based on the results from the model, a cost-benefit analysis was conducted to determine what mitigation measures ought to be taken to minimize the presence of the virus and its impact to the public.<br><br>
Apart from cleaning the data, a detailed analysis helped to establish which were the factors that most strongly influenced the presence of the virus. We carried out research regarding the relevant species of mosquitoes and the methodology/processes used to detect the presence of the virus. From the foregoing, we were also able to relate the data with the 'real world situation' to identify limitations in the data, and to inform what assumptions would be best employed in dealing with the matter.<br><br>
Of the classification models evaluated (Logistic Regression, K-Nearest Neighbors, Decision Tree, Random Forest, Extra Trees, Gradient Boost, Ada Boost), the best result (Kaggle score of 0.75) was obtained by using the Ada Boost Classifier with 100 estimators and a 0.73 learning rate.<br><br>

#### *Project 3: Classifying Text according to their SubReddits*
##### *Web Scraping | Natural Language Processing | Classification |<a href="https://www.github.com/irwinwei/GA-DSI-Project-03" target="_blank">> Link to project repository (see README file)</a>*
The objective was to build an NLP model to analyze the posts from 2 subreddits and determine which one a post belonged to. The subreddits selected for the project were:

- <a href="https://www.reddit.com/r/TalesFromTheCustomer" target="_blank">r/TalesFromTheCustomer</a> (accounts of poor customer service encountered by contributors)
- <a href="https://www.reddit.com/r/TalesFromYourServer" target="_blank">r/TalesFromYourServer</a> (accounts from people who work(ed) as waiters or waitresses about unreasonable customers)

The lexicon/vocabulary in both types of posts are very similar. Hence, the challenge was to create a model that relied not only individual words, but also multi-word sequences (bi-grams, tri-grams etc) to distinguish between the posts. About 1,000 posts from each subreddit were scraped from the web, resulting in approximately 2,000 rows of data to work with.<br><br>
The text was first pre-processed by removing stop-words and single-characters (if not a stop-word). Although lemmatization and stemming where subsequently applied, these steps appear to have a detrimental effect on the classification accuracy for this corpus. Count and TF-IDF vectorizers were also used to transform the data prior to input into the classifiers. The classification models used were Logistic Regression and Naive Bayes (Multinomial).<br><br>
The best results (accuracy, area under ROC curve) were achieved using TF-IDF vectorization and Naive Bayes (Multinomial) classifier.<br><br>

#### *Project 2: Predicting Housing Sale Prices in Ames, Iowa, USA*
##### *Regression |<a href="https://www.github.com/irwinwei/GA-DSI-Project-02" target="_blank">> Link to project repository (see README file)</a>*
The objective was to develop a machine learning model to predict the prices of houses based on history data (which described that attributes of each house), in the town of Ames in Iowa, USA. The data was downloaded from this <a href="https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/overview" target="_blank">project web page</a> and submitted to the Kaggle web page for scoring.<br><br>
The training data comprised 2,015 rows and 81 columns (which included the target "Sale Price"). The test data comprised 879 rows. The columns were a mixture of continuous, discrete ordered (ordinal) and discrete unordered (nominal) data. Preparing the data for training required thoughtful normalization and imputation. An iterative process of feature engineering using Lasso and Ridge regressions was also employed to determine those feature that had the most effect on the Sale Price.<br><br>
The final prediction model was submitted to Kaggle and returned a decent score of 31,996 which is based on the root mean-squared error (RMSE) between the predicted and actual values.<br><br>

#### *Project 1: Analysing SAT and ACT Participation Rates*
##### *Exploratory Data Analysis |<a href="https://www.github.com/irwinwei/GA-DSI-Project-01" target="_blank">> Link to project repository (see README file)</a>*
The objective was analyze the 2017 and 2018 participation rates and the component scores for the Scholastic Aptitude Test (SAT) and American College Test (ACT) by college students in the US. The analysis first required the data to be cleaned, visualized and explored with specific questions in mind. The normality of the distributions of the component scores were also explored.<br><br>
Based on external research as to what may have caused the differences in participation rates of the test in 2017 and 2018, we produced recommendations to increase the SAT participation rate in specific states.<br><br>
The group presentation is for the state of Iowa, whereas my personal analysis was for the state of Missouri.
