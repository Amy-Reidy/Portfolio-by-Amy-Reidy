## Hi, I'm Amy. 

![IMG_20210427_103513 (1)](https://user-images.githubusercontent.com/73396449/123549631-227c2a80-d76a-11eb-8cb7-7395ca88872e.jpg)


Welcome to my portfolio! As a passionate researcher and data enthusiast, my journey is fueled by an unwavering commitment to learning and a drive to find innovative solutions to development and humanitarian challenges. This quest has led me to the fascinating fields of data science and international development, continually broadening my knowledge and honing my skills.

In November 2023, I graduated with first-class honors from Atlantic Technological University, earning a Master's degree in Data Science. This accomplishment was a significant addition to my academic background, which also includes a Master's in Education and International Development. With over ten years of diverse experience across four continents in the non-profit and private sectors, my career has been a testament to my adaptability and broad perspective.

Currently, I'm contributing remotely from Italy as a Data Ingestion and Analytics Consultant for UNICEF's ECARO office. My role revolves around managing and enhancing the ETL processes for the TransMonEE Regional Database for Children, and developing the TransMonEE Dashboard using Dash and Python. This position allows me to blend my technical acumen with a deep-seated desire to impact children's rights monitoring through data.

At the intersection of social impact and data science, my interests are varied but focused. I am especially drawn to addressing issues in poverty alleviation, migration, gender equality, children’s rights, and public health and education equity.

Among the projects in my portfolio are a Convolutional Neural Network for Traffic Sign Classification and an exploration in Natural Language Understanding using Latent Semantic Analysis. These highlight my capability in applying advanced neural networks and my skill in deriving meaningful insights from complex data.

As I continue on this exciting path in data science, I eagerly look forward to enriching my portfolio with projects that demonstrate my technical prowess and contribute significantly to societal betterment. Keep an eye on this space for the latest updates, and please feel free to reach out for potential collaborations or discussions!

-----

### Project 1: [CNN Transfer Learning to Classify Traffic Signs](https://github.com/Amy-Reidy/Portfolio/blob/main/Traffic%20Sign%20Classifier%20with%20Transfer%20Learning%20Project/Poster%20for%20Transfer%20Learning%20Project.pdf)

![image](https://user-images.githubusercontent.com/73396449/157452389-8f33cf8d-4cfe-48ec-9b7b-8495d570ddb4.png)

As vehicles become more autonomous, there is an increasing demand in the automobile industry for driver assistance systems that can identify and **classify road signs quickly and accurately**. The aim of this project was to create a classifier, using a **pre-trained convolutional neural network**, that can effectively classify images from the **German Traffic Sign Recognition Benchmark dataset**. 

The convolutional base of the popular **VGG16 model** was used for feature extraction while the top fully connected layers were retrained with the GTSRB dataset and the **hyperparameters were fine-tuned** to further improve the model. The results show that the best-performing model in this experiment achieved an **accuracy of 82.98%**. As the dataset is quite imbalanced, future work could improve on this result by augmenting the images in the smaller classes to create a more balanced dataset.

A poster accompanying the project can be found [here](https://github.com/Amy-Reidy/Portfolio/blob/main/Traffic%20Sign%20Classifier%20with%20Transfer%20Learning%20Project/Poster%20for%20Transfer%20Learning%20Project.pdf), and [this paper](https://github.com/Amy-Reidy/Portfolio/blob/main/Traffic%20Sign%20Classifier%20with%20Transfer%20Learning%20Project/Paper%20for%20Transfer%20Learning%20Project.pdf) further explains the methodology. The code for the best-performing model can be reviewed [here](https://github.com/Amy-Reidy/Portfolio/blob/main/Traffic%20Sign%20Classifier%20with%20Transfer%20Learning%20Project/ML_Model_E%20(FINAL%20MODEL).ipynb), and the architecture of this model is shown below.


Skills demonstrated: ***Transfer Learning, Convolutional Neural Networks, Model Hyper-tuning, Model Validation***

Libraries used: ***TensorFlow, Keras, Pandas, Numpy, PIL, Google.Colab***

![Architecture of best-performing CNN model](https://user-images.githubusercontent.com/73396449/159645550-836a0dfb-828a-4cbd-8cd6-b9854d8e37bf.jpg "Architecture of best-performing CNN model")


-----
### Project 2: [Dashboard of Global Disparities in Cervical Cancer Rates](https://github.com/Amy-Reidy/Portfolio/blob/main/Global%20Disparities%20in%20Cervical%20Cancer%20Rates/Notebook%20-%20'Global%20Disparities%20in%20Cervical%20Cancer'%20Project.ipynb)

![image](https://user-images.githubusercontent.com/73396449/180845556-4f197fce-6f9e-4060-94b1-9027f2e12b1a.png)

The goal of this project was to **increase awareness of global inequalities in cervical cancer incidence and mortality rates** by exploring and visualizing data related to this disease. 

Cervical cancer (CC) is the **fourth most common cancer affecting women**, but thankfully the number of incidences and the mortality rates of cervical cancer have been slowly decreasing in the past few decades. However, in some countries (such as Lesotho, Zimbabwe, and Bulgaria) the number of new cases is actually increasing, and **women in low-resource settings are still disproportionately affected by cervical cancer** (Zhang et al., 2021). This is partly due to low-income and middle-income countries (LMICs) having less access to preventative services compared to richer countries, as well as less access to treatment for the later stages of the disease (Anaman-Torgbor et al., 2020). As a result, there are much higher mortality rates in these countries, and of the 310,000 women who died of this disease in 2018, **90% were living in LMICs** (Fray et al., 2020). A full literature review for this project can be viewed [here](https://github.com/Amy-Reidy/Portfolio/blob/main/Global%20Disparities%20in%20Cervical%20Cancer%20Rates/Global%20Disparities%20in%20Cervical%20Cancer.pdf).

To visualize the data that I collected and combined together, I created an **interactive dashboard using Plotly and Dash**, and you can see the full data preparation steps and Python code for the project in this **[Jupyter notebook](https://github.com/Amy-Reidy/Portfolio/blob/main/Global%20Disparities%20in%20Cervical%20Cancer%20Rates/Notebook%20-%20'Global%20Disparities%20in%20Cervical%20Cancer'%20Project.ipynb)**. 

The dashboard can be viewed at **[amyreidy.pythonanywhere.com/](https://amyreidy.pythonanywhere.com/)** and it allows the user to explore the data by visualizing either **incidence or mortality rates**, and by **aggregating by either continent or sub-region**. 

The dashboard contains four different visualizations:

1.	**Sunburst chart** – when a user clicks on the continent/sub-region, the chart shows the CC rate for each of the countries in that location when the user hovers over the country. The size and colour of the slice shows how the rate compares to other countries in that geographical area.

2.	**Bar chart** – this graph shows the average CC rates by continent or sub-region. Evidently, Africa has the highest average rates of both mortality and incidence rates. However, when the data is disaggregated by sub-region, we see that there is a lot of disparity within the continent as North Africa has relatively low CC rates, whereas Sub-Saharan Africa has the highest rates in the world. Similarly, we can see extreme disparity in Oceania with Australia and New Zealand having some of the lowest rates while Melanesia has the second highest incidence and mortality rates. This suggests that a weighted average could be more suitable for this type of visualization in the future.

3.	**World map** – this chart shows a geographical visualization of the CC rates for each country, with the value of CC rates being represented by the color scale and the marker size. When the user hovers over each country, more information is displayed in the text box. It is very clear from the map that the highest CC rates are found in Sub-Saharan African countries.

4.	**Scatter plot** - this chart shows the relationship between CC rates and other social indicators, and the user can change the indicator being displayed by clicking on the x-axis. The size of the markers is based on the CC rate (higher rates have bigger markers), and the markers are coloured purple or red based on if the country had a national HPV vaccination program as of 17th August 2021. Two regression lines have been added to the plot, one for the countries with a national vaccination program and one for the countries without a program. The regression lines show that CC rates are generally more negatively correlated with the social indicators when there is a vaccination program in place - e.g., the higher the Human Development Index (HDI) of a country, the lower the CC rates. However, when there is not a program, these social indicators are less correlated with CC rates. 


![Screenshot](https://user-images.githubusercontent.com/73396449/180840916-f2cdfd03-bcda-43ed-8f59-5b345ed602e2.JPG)

Skills demonstrated: ***Data Visualisation, Data Mining, Data Wrangling, Dashboard Creation, App Deployment***

Libraries used: ***Plotly, Dash, Flask, Pandas, Numpy***

-----
### Project 3: [Latent Semantic Analysis: Applied Linear Algebra in Natural Language Understanding](https://github.com/Amy-Reidy/Portfolio/blob/main/Latent%20Semantic%20Analysis%20Project/Linear%20Algebra%20Project%20Code%20-%20LSA.ipynb)                                                                                                                          

![image](https://user-images.githubusercontent.com/73396449/159176567-92ee61b6-9233-4385-b957-ad8e0cfe9a87.png)

                 
The aim of this project was to describe how **linear algebra can be applied to topic modelling in Natural Language Understanding (NLU)**. NLU is a subfield of Natural Language Processing (NLP), and the goal of NLU is to use computer algorithms to not just process text data, but to make sense of natural language data as it is spoken and written like a human would. 

Topic modelling is a NLU text-mining technique for extracting topics from text, and it can be used for **information retrieval, categorizing documents and exploratory analysis of text datasets**. It assumes that documents contain different topics, and these topics are made up of a collection of words. A foundational method of topic modelling is **Latent Semantic Analysis (LSA)** which is an unsupervised machine learning technique of analysing a text corpus (a large collection of texts) to **discover the hidden or latent topics** in it. This method differs from traditional NLP as it uses **statistical techniques and linear algebra** to analyse text, rather than relying on any specification of rules or dictionaries, and it is based on the principle of distributional hypothesis - words that have similar meanings occur in analogous segments of text.

There are two main steps in conducting LSA:

1. Construction of a term-document matrix.
2. Dimensionality reduction of this matrix using **Singular Value Decomposition (SVD)**. This process produces a topic-document matrix and a topic-term matrix.

To illustrate each of the steps involved in using LSA to quickly uncover themes across documents, text from the **titles and abstracts from ten recent research papers** were analyzed in this project. The papers are all related to **‘anticipatory action’** - an emerging approach to disaster risk reduction). Below are word clouds showing the **10 most prominent words** related to the top 2 topics that were uncovered from the text. 

You can review the code and read more about the theory, process and results in this  [notebook](https://github.com/Amy-Reidy/Portfolio/blob/main/Latent%20Semantic%20Analysis%20Project/Linear%20Algebra%20Project%20Code%20-%20LSA.ipynb).


Skills demonstrated: ***Natural Language Processing (NLP),  Text-Mining, Text Preprocessing, Latent Semantic Analysis***

Libraries used: ***Natural Language Toolkit (NLTK), TfidfVectorizer, CountVectorizer, TruncatedSVD, Pandas, Numpy, Matplotlib***

![topic_1](https://user-images.githubusercontent.com/73396449/159646507-6a66cfce-8b3b-403d-826f-077acd7069c3.jpg)      ![topic_2](https://user-images.githubusercontent.com/73396449/159647139-05bcd907-4934-4c65-a554-4ed2ff636d1b.jpg) 




-----
### Project 4: [Exploring Factors Related to Global Rates of COVID-19](https://github.com/Amy-Reidy/Portfolio/blob/main/Exploring%20Factors%20Related%20to%20Global%20Rates%20of%20COVID-19/Exploring%20Factors%20Related%20to%20Global%20Rates%20of%20COVID-19..ipynb)

![Alarming gap in global response to COVID-19](https://user-images.githubusercontent.com/73396449/123540825-3bbcb100-d741-11eb-84f9-0d0b61a7fda3.jpg)

I created this project as my final assignment for the 'Programming for Data Science' module of my master's program.

There were two goals of the project:\
**1. Test the claim that female-led countries have lower rates of COVID-19.**\
   I used the non-parametric Mann-Whitney U test to test the null hypothesis that the distributions of two samples are equal; first, I compared all countries in the sample and then just the OECD countries, as some critics say that this claim focuses too much on OECD countries.

**2. Create a linear regression model to predict rates of COVID-19 in countries around the world.**\
   I created multiple linear regression models using TensorFlow and Scikit-learn and compared the results. Note: these are quite simple models, as the course’s main objective was to introduce Python programming and there was only a very brief introduction to machine learning.
   
The data for COVID-19 rates around the world was retrieved by sending an API request to 'https://api.covid19api.com/summary'. Data for population and global rates of smoking, obesity, and life expectancy was sourced from csv files on [ourworldindata.org](https://ourworldindata.org/). Information about which countries are part of the OECD was retrieved from [https://www.oecd.org/](https://www.oecd.org/newsroom/global-oecd-welcomes-colombia-as-its-37th-member.htm#:~:text=The%20OECD's%2037%20members%20are,Poland%2C%20Portugal%2C%20Slovak%20Republic%2C). And to get a list of countries that have had a female leader for the COVID-19 outbreak, I used BeautifulSoup to web scrape a table with female heads of state and government from [Wikipedia](https://en.wikipedia.org/wiki/List_of_elected_and_appointed_female_heads_of_state_and_government).  

After the data was pre-processed, it was merged into a SQL database which was queried to extract information into dataframes 

Skills demonstrated: ***Hypothesis Testing, Advanced Statistics, Linear Regression, Web Scraping, SQL, Data Visualisation, Data Wrangling***

Tools used: ***Pandas, Numpy, Scikit-learn, TensorFlow, SQLite3, Scipy.stats,  Matplotlib, Seaborn, Requests, BeautifulSoup, Geopy, Folium***

-----
### Project 5: ["Has COVID-19 affected the world's happiness and wellbeing?"](https://github.com/Amy-Reidy/Portfolio-by-Amy-Reidy/blob/main/World%20Happiness%20and%20Wellbeing%20-%20Stats%20Project/World%20Happiness%20and%20Wellbeing%20Project.ipynb)
![Beyond-Catastrophe](https://user-images.githubusercontent.com/73396449/123085318-6269a780-d422-11eb-85a9-babc7d78552b.jpg)

This is a project I undertook for a module on 'Statistics and Applied Probability' and I used data from the World Happiness Report 2021 to test the following hypotheses:
 1.	Global happiness scores decreased from 2019 to 2020. 
 2.	Positive emotions decreased globally from 2019 to 2020. 
 3.	Negative emotions increased globally from 2019 to 2020.

As the differences between the samples were not normally distributed and had significant outliers, I decided to use a non-parametric test (Wilcoxon signed-rank test), rather than the paired T-test which is usually used for comparing paired samples. 

Skills demonstrated: ***Hypothesis Testing, Advanced Statistics, Data Wrangling, Data Visualisation*** 

Libraries used: ***Pandas, Numpy, SciPy, Matplotlib, Seaborn***



### Project 6: [“Exploring Toronto Neighborhoods to Identify a Suitable Location for a New Indian Restaurant”](https://github.com/Amy-Reidy/Portfolio/blob/main/IBM%20Capstone%20Project%20-%20Exploring%20Indian%20Restaurants%20in%20Toronto.ipynb)

![image](https://user-images.githubusercontent.com/73396449/160131823-895a8c41-faa0-44d6-b1cd-920b531ccc7b.png)


This was my first ever data science project, which I did as a capstone project for [IBM's Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science?utm_source=gg&utm_medium=sem&campaignid=2087860785&utm_campaign=10-IBM-Data-Science-ROW&utm_content=10-IBM-Data-Science-ROW&adgroupid=116274867101&device=c&keyword=&matchtype=b&network=g&devicemodel=&adpostion=&creativeid=506892807488&hide_mobile_promo&gclid=Cj0KCQjw5auGBhDEARIsAFyNm9H3qhF5Sg8y6oWRoxM86ZqMkHP_gaTK_Y1x9O8FKXRNscBTeqVRav8aAttWEALw_wcB) in November 2020.

The aim of the project was to investigate where would be a suitable location for a new Indian restaurant in Toronto, based on the density of existing Indian restaurants and the number of Indian residents in each neighborhood.

Data was sourced by web scraping Wikipedia, extracting information about various venues in Toronto and their geospatial information using Foursquare’s API, and obtaining geospatial for Toronto from “https://cocl.us/Geospatial_data”.

The K-means machine learning model was used to group the neighborhoods into clusters based on the density of Indian restaurants in each neighborhood.

Skills demonstrated: ***Unsupervised Machine Learning, Clustering, K-Means, Web Scraping, Data Wrangling, Data Cleansing** 

Tools used: ***Pandas, Numpy, Scikit-learn, Matplotlib, Seaborn, Requests, Geopy, Folium, Wikipedia, Yellowbrick***


