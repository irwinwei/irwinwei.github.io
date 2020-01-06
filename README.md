## Thank you for dropping by. My name is Irwin Wei.
You have reached my project portfolio page which continues to grow. I was most recently working in General Insurance (claims) as a Loss Adjuster - we go by other names like "adjuster", "surveyor" or "assessor". If you ever filed an insurance claim for your house, building, shop unit, warehouse, office, power plant, construction site, oil refinery, ship or aircraft, you would likely have met one of us. I have prior experience in consulting, software development and product development.

#### <a style="font-weight:bold" href="https://www.linkedin.com/in/irwinwei" target="_blank">Learn more about me or get in touch via LinkedIn</a>

The following are projects to date, in **reverse chronological order** (most recent at the top).
<br><br>

### 2019 Projects

#### *Capstone Project: Predicting Whether Insurance Underwriting Gain will be Negative*
##### *Regression | Classification | Unsupervised |<a href="https://www.github.com/irwinwei/GA-DSI-Capstone" target="_blank">> Link to project repository (see README file)</a>*
Project write-up to be added shortly.
<br><br>

#### *Project 4: Predicting the Presence of West Nile Virus*
##### *Classification |<a href="https://www.github.com/irwinwei/GA-DSI-Project-04" target="_blank">> Link to project repository (see README file)</a>*
We were required to study known cases of West Nile Virus presence in Chicago and to predict, based on weather and pesticide usage information, when the virus would be present i.e. the positive case being that the virus was present, and the negative case being that the virus was not present. The data used for this project was downloaded from this <a href="https://www.kaggle.com/c/predict-west-nile-virus/" target="_blank">Kaggle competition web page</a> and submitted to Kaggle web page for scoring. The score for classification was based on the area under the "ROC" curve (AUC).<br><br>
Based on the results from the model, a cost-benefit analysis was conducted to determine what mitigation measures ought to be taken to minimize the presence of the virus and its impact to the public.<br><br>
Apart from cleaning the data, a detailed analysis helped to establish which were the factors that most strongly influenced the presence of the virus. We carried out research regarding the relevant species of mosquitoes and the methodology/processes used to detect the presence of the virus. From the foregoing, we were also able to relate the data with the 'real world situation' to identify limitations in the data, and to inform what assumptions would be best employed in dealing with the matter.<br><br>
Of the classification models evaluated (Logistic Regression, K-Nearest Neighbors, Decision Tree, Random Forest, Extra Trees, Gradient Boost, Ada Boost), the best result (Kaggle score of 0.75) was obtained by using the Ada Boost Classifier with 100 estimators and a 0.73 learning rate.<br><br>

#### *Project 3: Classifying Text according to their SubReddits*
##### *Web Scraping | Natural Language Processing | Classification |<a href="https://www.github.com/irwinwei/GA-DSI-Project-03" target="_blank">> Link to project repository (see README file)</a>*
The objective was to build an NLP model to analyze the posts from 2 subreddits and determine which one a post belonged to. The subreddits selected for the project were:

- <a href="https://www.reddit.com/r/TalesFromTheCustomer" target="_blank">r/TalesFromTheCustomer</a> (comprises accounts of poor customer service encountered by contributors)
- <a href="https://www.reddit.com/r/TalesFromYourServer" target="_blank">r/TalesFromYourServer</a> (comprises contributions from people who work(ed) as waiters/waitresses regarding unreasonable customers they encountered)

The lexicon/vocabulary in both types of posts are very similar. Hence, the challenge was to create a model that relied not only individual words, but also multi-word sequences (bi-grams, tri-grams etc) to distinguish between the posts. About 1,000 posts from each subreddit were scraped from the web, resulting in approximately 2,000 rows of data to work with.<br><br>
The text was first pre-processed by removing stop-words and single-characters (if not a stop-word). Although lemmatization and stemming where subsequently applied, these steps appear to have a detrimental effect on the classification accuracy for this corpus. Count and TF-IDF vectorizers were also used to transform the data prior to input into the classifiers. The classification models used were Logistic Regression and Naive Bayes (Multinomial).<br><br>
The best results (accuracy, area under ROC curve) were achieved using TF-IDF vectorization and Naive Bayes (Multinomial) classifier.<br><br>

#### *Project 2: Predicting Housing Sale Prices in Ames, Iowa, USA*
##### *Regression |<a href="https://www.github.com/irwinwei/GA-DSI-Project-02" target="_blank">> Link to project repository (see README file)</a>*
The objective was to develop a machine learning to predict the prices of houses based on data concerning attributes of each house, in the town of Ames in Iowa, USA. The data was downloaded from this <a href="https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/overview" target="_blank">project web page</a> and submitted to the Kaggle web page for scoring.<br><br>
The training data comprised 2,015 rows and 81 columns (which included the target "Sale Price"). The test data comprised 879 rows. The columns were a mixture of continuous, discrete ordered (ordinal) and discrete unordered (nominal) data. Preparing the data for training required thoughtful normalization and imputation. An iterative process of feature engineering using Lasso and Ridge regressions was also employed to determine those feature that had the most effect on the Sale Price.<br><br>
The final prediction model was submitted to Kaggle and returned a decent score of 31,996 which is based on the root mean-squared error (RMSE) between the predicted and actual values.<br><br>

#### *Project 1: Analysing SAT and ACT Participation Rates*
##### *Exploratory Data Analysis |<a href="https://www.github.com/irwinwei/GA-DSI-Project-01" target="_blank">> Link to project repository (see README file)</a>*
The objective was to carry out an analysis of the 2017 and 2018 participation rates and the component scores for the Scholastic Aptitude Test (SAT) and American College Test (ACT) by college students in the US. The analysis first required the data to be cleaned, visualized and explored with specific questions in mind. The normality of the distributions of the component scores were also explored.<br><br>
Lastly, based on external research as to what may have caused the differences in participation rates of the test in 2017 and 2018, we produced recommendations to increase the SAT participation rate in specific states.<br><br>
The group presentation is for the state of Iowa, whereas my personal analysis was for the state of Missouri.
