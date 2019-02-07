# Projects

## 1. Web programming - data scraping, pipelining, visualisation

### 1.1. [Pubmed's top authors](https://github.com/gknam/pubmed-top-authors)

Try the [demo](https://pubmed-top-authors-gknam.c9users.io/).

#### Description

User submits an author name or a keyword with other parameters (number of articles, number of authors to plot, date range from the day of search). Pubmed database is queried, and interactive plots are drawn using returned data.


<a href="https://www.youtube.com/watch?v=jXctQUTaPcY" target="_blank"><img src="pubmed_top_authors.png" alt="pubmed_authors" style="float:left" /></a>


#### Languages, packages and framework used
* Backend
   * Python
       * [Flask](http://flask.pocoo.org/)
   * SQLite3 (via Python's [SQLAlchemy](https://www.sqlalchemy.org/))
   * [xml.etree.ElementTree](https://docs.python.org/3/library/xml.etree.elementtree.html)
* Frontend
   * HTML
   * CSS
   * JavaScript
       * [D3.js](https://d3js.org/)
       * [jQuery](https://jquery.com/)
       * [jQueryUI](https://jqueryui.com/)
       * [Bootstrap](https://getbootstrap.com/)
       * [typeahead.js](https://twitter.github.io/typeahead.js/)
       * [Handlebars.js](https://handlebarsjs.com)

#### Technical notes

* Back-end
    * Auto-update database at regular interval (not fully tested)
        * Fetch data from Pubmed
        * [ETL](https://en.wikipedia.org/wiki/Extract,_transform,_load) data
            * E: Relevant elements (i.e. information) are  **_extracted_** using [**xml.etree.ElementTree**](https://docs.python.org/3/library/xml.etree.elementtree.html), 
            * T: **_transformed_**  into a Python data type (e.g. [set](https://docs.python.org/2/library/sets.html))
            * L: **_loaded_** into the DB using  **SQLite**  and [SQLAlchemy](https://www.sqlalchemy.org/)
    * Upon receipt of search request from front-end, query either SQLite3 database or [Pubmed API](https://www.ncbi.nlm.nih.gov/books/NBK25501/).
    * Send data to front-end in JSON format
* Front-end
    * Reorganise data
    * Draw interactive plots using D3.js


## 2. Data science projects

###  2.1. [Guided projects at DataQuest](https://github.com/gknam/projects/tree/master/DataScience/DataQuest)

* Step 1: Python Introduction
    * Python Programming: Beginner
        * [Using Jupyter notebook](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step1_PythonIntro/1_PythonBeginner/project1/UsingJupyterNotebook.ipynb) - Open CSV file
        * [Explore U.S. Births](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step1_PythonIntro/1_PythonBeginner/project2/ExploreUsBirths.ipynb) - Data visualisation, Descriptive statistics
    * Python Programming: Intermediate
        * [Exploring Gun Deaths in the US](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step1_PythonIntro/2_PythonIntermediate/project1/ExploringGunDeathsInTheUS.ipynb) - Data visualisation
* Step 2: Data Analysis and Visualization
    * Pandas and NumPy Fundamentals
        * [Analyzing Thanksgiving Dinner](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/1_PandasAndNumPyFundamentals/Old_Before20180921/project1/AnalyzingThanksgivingDinner.ipynb) - Data visualisation, Descriptive statistics
        * [Exploring Ebay Car Sales Data](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/1_PandasAndNumPyFundamentals/New_20180921/project1/ExploringEbayCarSalesData.ipynb) - Feature processing, data cleaning, data visualisation, descriptive statistics
    * Exploratory Data Visualization
        * [Visualizing Earnings Based On College Majors](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/2_dataAnalVis/project1/Visualizing_Earnings_Based_On_College_Majors.ipynb) - Data cleaning, data visualisation, descriptive statistics
    * Storytelling Through Data Visualization
        * [Visualizing The Gender Gap In College Degrees](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/3_StorytellingThroughDataVisualization/project1/VisualizingTheGenderGapInCollegeDegrees.ipynb) - Data visualisation
    * Data Cleaning
        * [Analyzing NYC High School Data](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/4_DataCleaning/project1/AnalyzingNYCHighSchoolData.ipynb) - Feature processing, statistics, data visualisation, data analysis
        * [Star Wars Survey](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step2_DataAnalVis/4_DataCleaning/project2/StarWarsSurvey.ipynb) - Data cleaning, feature processing, data visualisation, data analysis
* Step 3: The Command Line
    * Command Line: Beginner
        * [Working With Data Downloads](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step3_TheCommandLine/1_CommandLine-Beginner/project1/WorkingWithDataDownloads.ipynb) - Data visualisation, data analysis (?)
    * Command Line: Intermediate
        * [Transforming data with Python](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step3_TheCommandLine/2_CommandLine-Intermediate/project1/TransformingDataWithPython.ipynb) - Descriptive statistics
* Step 4: Working with Data Sources
    * SQL Fundamentals
        * [Analyzing CIA Factbook Data Using SQLite and Python](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step4_WorkingWithDataSources/1_SQLfundamentals/project1/AnalyzingCIAfactbookDataUsingSQLiteAndPython.ipynb) - Database (query), data visualisation, descriptive statistics
    * SQL and Databases: Intermediate (old)
        * [Preparing data for SQLite](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step4_WorkingWithDataSources/Old_2_SQLAndDatabases-Intermediate/project1/PreparingDataForSQLite.ipynb) - Database (query), data cleaning, feature processing
        * [Creating relations in SQLite](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step4_WorkingWithDataSources/Old_2_SQLAndDatabases-Intermediate/project2/CreatingRelationsInSQLite.ipynb) - Database (creation, query)
    * SQL and Databases: Intermediate (new)
        * [Answering Business Questions using SQL](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step4_WorkingWithDataSources/2_SQLIntermediate-TableRelationsAndJoins/project1/AnsweringBusinessQuestionsUsingSQL.ipynb) - Database (query), data visualisation (interactive), data analysis
        * [Designing and Creating a Database](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step4_WorkingWithDataSources/2_SQLIntermediate-TableRelationsAndJoins/project2/DesigningAndCreatingDatabase.ipynb) - Database (design, creation)
* Step 5: Probability and Statistics
    * Statistics Fundamentals
        * [Investigating Fandango Movie Ratings](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step5_ProbabilityAndStatistics/1_StatisticsFundamentals/project1/InvestigatingFandangoMovieRatings.ipynb) - Descriptive statistics, probability, data visualisation, data analysis
    * Statistics Intermediate: Averages and Variability
        * [Finding the Best Markets to Advertise In](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step5_ProbabilityAndStatistics/2_StatisticsIntermediate-AveragesAndVariability/project1/FindingTheBestMarketsToAdvertiseIn.ipynb) - Data visualisation, data cleaning, data analysis, feature processing
    * Probability and Statistics in Python: Beginner
        * [Analyzing Movie Reviews](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step5_ProbabilityAndStatistics/Old_1_ProbabilityAndStatisticsInPython-Beginner/project1/AnalyzingMovieReviews.ipynb) - Statistics, data visualisation, data analysis
    * Probability and Statistics in Python: Intermediate
        * [Winning Jeopardy](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step5_ProbabilityAndStatistics/3_ProbabilityAndStatisticsInPython-Intermediate/project1/WinningJeopardy.ipynb) - Statistics, data cleaning, data analysis, feature processing
* Step 6: Machine Learning
    * Machine Learning Fundamentals
        * [Predicting Car Prices](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step6_MachineLearning/1_MachineLearningFundamentals/project1/PredictingCarPrices.ipynb) - Machine learning, data visualisation, data cleaning, feature processing
    * Linear Regression For Machine Learning
        * [Predicting House Sale Prices](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step6_MachineLearning/4_LinearRegressionForMachineLearning/project1/PredictingHouseSalePrices.ipynb) - Machine learning, data cleaning, feature processing, feature engineering
    * Machine Learning in Python: Intermediate
        * [Predicting the stock market](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step6_MachineLearning/5_MachineLearningInPython-Intermediate/project1/PredictingTheStockMarket.ipynb) - Machine learning, data cleaning, feature processing, 
    * Decision Trees
        * [Predicting Bike Rentals](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step6_MachineLearning/6_DecisionTrees/project1/PredictingBikeRentals.ipynb) - Machine learning, data cleaning, feature processing
* Step 7: Advanced Python and Computer Science
    * Data Structures and Algorithms
        * [Efficiencies of matrix search strategies](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step7_AdvancedPythonAndComputerScience/1_DataStructuresAndAlgorithms/project1/EfficienciesOfMatrixSearchStrategies.ipynb) - Data visualisation
* Step 8: Advanced Topics in Data Science
    * Kaggle Fundamentals
        * [Creating a Kaggle Workflow](https://github.com/gknam/projects/blob/master/DataScience/DataQuest/Step8_AdvancedTopicsInDataScience/1_KaggleFundamentals/project1/CreatingAkaggleWorkflow.ipynb) - Machine learning, data visualisation, feature processing, feature engineering