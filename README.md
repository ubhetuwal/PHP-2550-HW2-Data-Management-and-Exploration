# PHP-2550-HW2-Data-Management-and-Exploration
It is important that you learn to write up your results carefully. For each problem assigned for homework, you should carefully describe the analytic methods used and summarize key findings in carefully written English with reference to appropriate tables and figures as needed.

 

The dataset mcalindon_Big.csvPreview the document contains information on individuals who were involved in a clinical trial that measured their pain on 7 different days over the course of several weeks together with local weather information for each person. This is described in the paper by McAlindon et al.Preview the document and in the codebook McAlindon_big.rtfPreview the document.

 

This dataset is in what we call long form meaning that each participant has multiple rows of data each corresponding to a given weather date. Note that the number of rows per participant varies. Variables that are common to a participant on all weather days are the same for each row for each participant. These are participant-level data. Weather variables vary by weather date. These are date-level data that vary within participant.

 

You might simplify the data by creating one set that holds the participant-level data and another that holds the weather-level data linked by the participant ID.

 

    Create these two datasets. How many unique individuals are there in the dataset? Create a graphic that shows the distribution of the number of observations per individual.

Hint: Use the rle function to determine the unique id numbers and the number of rows associated with each id. Then use functions like cumsum to construct the starting and ending row numbers for each individual. This will then allow you to pull off the first row for each person.

    Note that the participant-level data contain 7 variables corresponding to the pain measurements on each of 7 days in the study.

 a. Summarize the average pain score for each of the 7 days of the study.

 b. Regress each of the 7 pain scores on age and use the summary function to create a summary table for each regression. Then find the 95% confidence interval for the regression slopes (e.g. use the confint function) and produce a table with the estimates, standard errors, p-values and confidence intervals of the 7 slopes and put these in a single table. Interpret the findings.

 c. For each individual fit a regression of pain on time. Summarize the slopes and intercepts produced.

 d. Summarize the distributions of the variables age, race, income, BMI, sex, use of NSAIDs and occupation.

 e. Are the slopes or intercepts computed in problem c related to any of the patient characteristics described in problem d?

 

    Now use the weather dataset and the participant level dataset.

    a. Graph and describe the temperatures experienced by each individual over the time in which they were enrolled in the study. Do you see any patterns?

    b. Compute the correlation for each individual between their pain scores and the average temperature on the dates the pain scores were taken and construct a graph to display these correlations. Discuss whether pain is correlated with temperature

    c. Express these correlations as regressions and describe the slopes and intercepts for each individual as in problem 2c.

    d. What do you notice about the distributions of the correlations in 3b and the slopes in 3c?
