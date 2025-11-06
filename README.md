# Current-work-work-work-work-work
StackOverflow Developer Salary Analysis 
Overview

This project is part of a university data analysis course. - So it's partially in Czech

The goal is to analyze developer survey data from StackOverflow and build a predictive model to estimate total compensation (CompTotal) based on various demographic and professional features.

The work presented here corresponds to the intermediate stage of the project. It focuses on data cleaning, feature engineering, encoding, and initial modeling.

Objectives

Explore and clean the dataset

Handle missing and duplicate values

Transform categorical and multi-label features into numeric form

Analyze correlations between features

Build a baseline regression model to predict CompTotal

Interpret feature importance and model behavior

Data Preparation

Selected relevant columns (country, currency, education, dev type, languages, frameworks, databases, experience, etc.)

Removed missing and low-information entries (dropna, unique ratio filtering)

Encoded categorical variables using:

OrdinalEncoder and BinaryEncoder for simple categories

OneHotEncoder for multi-class categories (DevType, EdLevel, RemoteWork)

MultiLabelBinarizer for list-type columns (Languages, Databases, Web frameworks)

Normalized target variable CompTotal using log1p() and RobustScaler

Modeling

Built a Linear Regression model as a baseline

Evaluated with MAE and RMSE metrics:

MAE = 0.69

RMSE = 1.25

Analyzed top 15 influential features impacting salary

Most influential: Currency, Country, and Developer Type

Planned Next Steps

Implement Association Rule Mining to uncover frequent technology patterns

Train Decision Tree models for interpretable prediction

Perform Outlier Detection and Exception Rule Mining to identify unusual salary cases

Compare models and refine features based on interpretability and accuracy

Notes

This repository represents an in-progress version of the project.
Further analyses and improvements will be added in subsequent updates.
