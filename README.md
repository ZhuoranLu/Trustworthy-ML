<p align="center">

# Trustworthy-ML

This is a repository for the data and analysis code for the paper "Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks".

## Repository Structure

* `rawData` contains the profiles of the speed dating tasks used in the experiments, and raw data dumped from the experiment procedure.

* `data` contains the cleaned data including the predictions of tasks and answers to the questionnaire given by subjects.

* `analysis` contains the analysis code implemented by python and R via jupyter notebook and R markdown.

Each file in `data` and `analysis` starting with "experimentOne","experimentTwo", "experimentThree", are each corresponding to the Experiment 1, 2, 3 in the paper.

## Data Sample


| workerID | idpAgreement | taskId | profile | globalId | decision | selfPrediction| finalPrediction| selfCorrect| finalCorrect | agreement | time                    | prediction | finalAgreement | mlCorrect | switch |
| -------- | ------------ | -------| ------- | -------- | -------- | ------------- | -------------- | ---------- | ------------ | --------- | --------------------------- | ---------- | -------------- |------------- |------------- |
| 1 | 40 | 4 | 26 | 734 | 1 | 1| 0| FALSE| FALSE | 0 | Mon Feb 10 2020 171422 GMT-0500 (Eastern Standard Time) | 1 | TRUE | TRUE | TRUE |

## Licensing & Citing
When using or building upon the data in an academic publication, please consider citing as follows:

Lu, Z., & Yin M. (2021, May). Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks. In *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems* 
 
 [DOI:10.1145/3411764.3445562]


