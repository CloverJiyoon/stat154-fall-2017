Stat 154 - Fall 2017, Final Project
================
Due date: December 10, 2017

Submission Instructions
-----------------------

The final project is a practical project to be done individually or in a team of 2 members max (no teams with more than 2 members allowed).

You will receive a link to a google sheet to be filled in with your team's name, the member names, and the corresponding email addresses.

Each team will be invited to a BOX folder (via bConnected): <https://berkeley.account.box.com/login>. You should be able to log in using the email that appears on CalCentral (e.g. typically your `berkeley.edu` email).

Each team must submit all the materials of their final project to the shared BOX folder.

Each team's folder must contain a `README` file explaining the structure of the project. Here's a sample file structure of how your BOX folder may look like:

      team01/
         README.md
         data/
            ... # all the data files
         R/
            ... # all you R files here
         report/
            ... # mainly the pdf file
            ... # (you could use an Rmd file)

You can add more folders to the previous file structure.

You must produce a single PDF file for the report.

Data
----

The data set for this project is the [Census Income Data Set](https://archive.ics.uci.edu/ml/datasets/Census+Income) donated by Ronny Kohavi and Barry Becker to the UCI Machine Learning Repository.

The data set describes 15 variables on a sample of individuals from the US Census database. The prediction task is to determine whether a person makes over 50K a year.

Preprocessing and Exploratory Data Analysis
-------------------------------------------

Start your analysis cycle with an exploratory phase so you get to know and understand the data set. Below is a (non-comprehensive) list of (optional) considerations to keep in mind:

-   Handling missing values
-   Handling outliers
-   Changing scales
-   Binning (i.e. discretizing)
-   Converting to (dummy) indicators
-   Summary statistics
-   Visualizing distributions
-   Association between each predictor and the response

### Build a Classification Tree

-   Fit a classification tree (see examples in ISL chapter 8, and APM chapter 14).
-   Make plots and describe the steps you took to justify choosing optimal tuning parameters.
-   Report your 5 (or 6 or 7) important features (could be either just 5, or 6 or 7), with their variable importance statistics.
-   Report the training accuracy rate.
-   Plot the ROC curve, and report its area under the curve (AUC) statistic.

### Build a Bagged Tree

-   Train a Random Forest classifier (see examples in ISL chapter 8, and APM chapter 14)
-   Make plots and describe the steps you took to justify choosing optimal tuning parameters.
-   Report your 5 (or 6 or 7) important features (could be either just 5, or 6 or 7), with their variable importance statistics.
-   Report the training accuracy rate.
-   Plot the ROC curve, and report its area under the curve (AUC) statistic.

### Build a Random Forest

-   Train a Random Forest classifier (see examples in ISL chapter 8, and APM chapter 14)
-   Make plots and describe the steps you took to justify choosing optimal tuning parameters.
-   Report your 5 (or 6 or 7) important features (could be either just 5, or 6 or 7), with their variable importance statistics.
-   Report the training accuracy rate.
-   Plot the ROC curve, and report its area under the curve (AUC) statistic.

### Model Selection

-   Validate your best supervised classifier on the test set.
-   Compute the confusion matrix.
-   Using the class "over 50K a year" as the positive event, calculate the *Sensitivity* or *True Positive Rate* (TPR), and the *Specificity* or *True Negative Rate* (TNR).
-   Plot the ROC curves of all the classifiers.
