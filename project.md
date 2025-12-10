# Semester Project

## Introduction

In many ways, this assignment is intentionally open-ended – there are several parts that ask you to decide what to do, and there is not necessarily a single right or wrong answer to the question. As a group, you will decide things like which variables to use for your models, and which to ignore. The outcome matters, but you should focus more on the process. 

__There is not necessarily a single right or wrong answer__ is not the same as saying all answers are equally wonderful. A rubric for this assignment will be posted on our class Blackboard page. You may get results that are not nice or neat – remember, this is real-world data, and not based on a canned textbook example. If your model does not predict the outcome variable well, that doesn’t necessarily mean that you did something wrong, or that the assignment prompt is wrong; On the contrary, it means that you explored something, you found results, and you’re reporting the results. Sometimes, it doesn’t get more real world than that! 

A data dictionary has also been provided. Some of these variable descriptions may not be totally clear, but that will not impede your ability to perform any steps on this prompt. The cities available for the project are either:

1. Geneva
2. Vaud
3. Zurich

Your teams have already been assigned. Each team will choose one city (the project can be completed with any city, so one is not better than any other for this project). The instructor will be glad to clarify any questions you have about the project or about the rubric, which can also be found in the Semester Project folder. However, the assignment itself belongs to you and your team. I want to stay as far away from your code, and your decisions,
as possible.


If you have a question along the lines of Why doesn’t this code work?, the instructor will assume that you have already run this question by all of your other team members. As you proceed, just remember this quote from Hadley Wickham: Every good data analysis starts as a bad data analysis. So get started, do it badly, and then do it better! Start by downloading your city’s dataset from our class Blackboard page. It can be found in the semester project folder.

## Steps

### Data Preparation & Exploration (20 points)

Read your data into your local environment.

1. Missing Values

• Does your data contain any missing values and/or blank cells? If so, what can you do about this?
• Write one paragraph describing what you did, and why you did it. (Note: You may wish to deal with missing values differently for different tasks. You are not locked in to a decision regarding missing values). Throughout the various steps, you may also wish to consider the way you’ll handle outliers.

2. Summary Statistics

• Take a peek at your data, and look at some of the ways that it’s organized by area. To do this, you may wish to use neighbourhood, or neighbourhood_cleansed variables (note the UK spelling of these words). If one of these groups has many levels, you could try a top_n filter or find a way to combine some of them together. Alternatively, you could use the lat/long variables to divide your city however you wish to. Next, generate at least 5 different summary stats that reveal things about the differences (or lack thereof) among the areas in your city. 
• Show your results. Describe your findings in 1-2 paragraphs. For each stat you found, what is your team’s takeaway?

3. Data Visualization

• Now generate five visualizations that help you to better understand the various neighborhoods, or regions, in your city. Be creative! This is intentionally very open-ended. The only requirement is that each one of your plots offers information about your city and its regions. Make five different types of plots for this.
• Write a two-paragraph description that explains the choices that you made, and what the resulting plots teach you about your data.

4. Mapping

• Generate a map of the Airbnb rentals in your city. Do any key features here seem to stand out? What are a few of the things your map shows you about your region? No citations are needed here but this can be a chance to orient the reader to your city and some of its key features.

5. Word Cloud

• Using the neighborhood overview column in your dataset, generate a wordcloud. What are some terms that seem to be emphasized here?

## Prediction (20 points)

1. Create a multiple regression model with the outcome variable price. The dataset description implies that the units are Swiss francs. Swiss francs are nearly equivalent to US dollars.
2. Describe your process. How did you wind up including the independent variables that you kept, and discarding the ones that you didn’t keep? In a narrative of at least two paragraphs, discuss your process and your reasoning. In the write-up, be sure to talk about how you evaluated the quality of your model.
3. Show a screenshot of your regression summary, and explain the regression equation that it generated.
4. Analyze any other metrics that are relevant for linear regression models. Based on these, what can you say about your model’s performance in 1-2 paragraphs? When performing this step, you may wish to consider a log transformation on the response variable. 

## Classification (40 points)

1. **Classification, Part I. k-nn** Using k-nearest neighbors, predict whether a rental in your neighborhood will have some particular amenity, or combination of amenities. Use any set of numerical predictors in order to build this model. You can decide which amenity, or set of amenities, to use as your outcome variable.

• Show the code you used to run your model, and the code you used to assess your model.
• Write a two-paragraph narrative that describes how you did this. In your narrative, be sure to describe your amenity choice(s), your predictor choices, and the process that you used to arrive at the particular k value that you used. When assessing your model, you may also wish to consider its performance against a naive benchmark.

2. **Classification, Part II. Classification Tree**

• Build a classification tree that predicts the host_response_time variable.
• Determine the ideal size of your tree using cross-validation.
• Show your tree model here.
• In a 1-2 paragraph write-up, describe your process. Mention anything that you found interesting as you explored various possible models, the process you used to arrive at the model you finished with, and any findings that you can draw from the model results.

3. **Classification, Part III. Transformer**

• We will now use a transformer model as a classification tool.
• Create a new variable called price_quartile. Divide the price variable into four quartiles. The new variable should be a categorical variable with 4 classes.
• There are three descriptive text columns, description, host_about and amenities.
• Use a transformer model of your choosing to build a classification model which predicts the price quartile for a data record based on these 3 input variables.
• You have to test your model using the training and test data sets. 
• Describe a fictional rental record which creates the above three input variables, and use your model to predict which bin it will fall into.
• Write a two-paragraph narrative that describes how you did this. In your narrative, be sure to talk about things like assessing performance using your training and validation data.

## Clustering (15 points)

• Perform either a k-means analysis or a hierarchical clustering analysis in order to place rental units within your city into clusters (each observation in your dataframe is one rental unit). 

Of any section of the project, this one offers the most opportunity to be creative and take risks. 

Think about feature engineering, too – how/when/where can you create new variables based on existing ones?
• Show your code and results. Name and describe each of your clusters. In 1-2 paragraphs, describe the process that you used for variable selection and model building.
• Include at least three simple visualizations that describe your clustering model. A simple visualization can be a scatterplot, histogram, barplot, boxplot, violin plot, etc. Write 1-2 sentences for each visualization to explain what it shows. Do not include any visualization that your team is unable to fully explain. Including an unexplained visualization will cost your team points on both the write-up and the presentation.

## Conclusions (5 points)

• Write a 3-5 paragraph summary that describes your overall process and experience with this assignment. How could these findings be useful? Who could benefit from the data mining that you have performed here? You already summarized your specific steps in some other parts of the write-up, so focus
on the big picture here (do not not use the conclusion to simply describe everything you did in the other parts). Try to deliver some specific insights or takeaways here, and avoid copy-pasted AI output for your answer.
• Submit your final report as a PDF to Blackboard before the deadline listed on the assignment. Your PDF should generally have a similar look and feel to a homework submission.
• Please be sure to take out the trash prior to submission in other words, don’t include hundreds of pages of code printout, notes that don’t pertain to your answers, etc.
• Also: Upload the Python Script(s) that you used to generate your results