# UK Biobank Female Cancer Study

This repository contains code related to a comprehensive study on the risk factors associated with female cancers, with a specific focus on breast, ovarian, and uterine cancers. The study utilizes data from the UK Biobank, a prospective cohort study consisting of over half a million participants. The goal of this research is to identify a sparse set of variables that can jointly predict multiple cancers and contribute to the development of effective early detection and prevention strategies.


## Study Overview

The study involves the following steps:

* Data Preprocessing: This step includes cleaning the UK Biobank data, dealing with missing data, transforming variables, and downsampling due to imbalance between cases and controls.
* Test Train Split: This step involves splitting the data set, into variable selection, train and test. 
* Exploratory Data Analysis: This step involves univariate analysis on each exposure to four outcomes (all female cancers, breast cancer, uterus cancer, and ovary cancer), with adjustment for age.
* Variable Selection: A stability selection lasso is fitted to identify a sparse set of variables that can jointly predict multiple cancers.
* Model Building and Evaluation: Two predictive models, a logistic regression and a ridge regression, are built for each outcome using the selected variables. The models are trained and tested on separate data splits, and their performance is compared using AUC.


## Running the Scripts
Clone this repository to your local machine.
Ensure you have R version 4.2.2 installed along with the necessary packages (glm, SHAP, glmnet, MatchIt, MICE).
Navigate to the scripts/ directory and run the scripts in the following order:
00_preprocessing.rmd
01_test_train_split.rmd
02_preanalysis.rmd
03_univariate_analysis.rmd
04_stability_selection.rmd
05_prediction.Rmd

## Results
This research contributes to a deeper understanding of the risk factors implicated in the development of female cancers. The predictive models built in this study have practical implications for early detection and prevention initiatives, leading to more focused and efficacious screening and prevention strategies.

## Contact

For any questions or feedback, please feel free to contact us:

* seth.howes22@imperial.ac.uk
* constance.bicanic-popovic22@imperial.ac.uk
* siwei.wu22@imperial.ac.uk
* fiona.rice22@imperial.ac.uk





