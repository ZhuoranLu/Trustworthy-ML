<p align="center">

# Trustworthy-ML

This is a repository for the data and analysis code for the paper "Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks".

## Repository Structure

* `rawData` contains the profiles of the speed dating tasks used in the experiments, and raw data dumped from the experiment procedure.

* `data` contains the cleaned data including the predictions of tasks and answers to the questionnaire given by subjects.

* `analysis` contains the analysis code implemented by python and R via jupyter notebook and R markdown.

Each file in `data` and `analysis` starting with "experimentOne","experimentTwo", "experimentThree", are each corresponding to the Experiment 1, 2, 3 in the paper.

## Data Sample

Here attached a sample of the data of predictions made by subjects. Each row is a piece of record on a subject making predictions on one task.

`1` indicates "The dating participant wants to see the date again." `0` indicates "The dating participant wants to see the date again."


| workerID | idpAgreement | taskId | profile | globalId | decision | selfPrediction| finalPrediction| selfCorrect| finalCorrect | agreement | time                    | prediction | finalAgreement | mlCorrect | switch |
| -------- | ------------ | -------| ------- | -------- | -------- | ------------- | -------------- | ---------- | ------------ | --------- | --------------------------- | ---------- | -------------- |------------- |------------- |
| 1 | 40 | 4 | 26 | 734 | 1 | 1| 0| FALSE| FALSE | 0 | Mon Feb 10 2020 171422 GMT-0500 (Eastern Standard Time) | 1 | TRUE | TRUE | TRUE |

* `workerId` Int. The unique for each subject
* `idpAgreement` Int. The three different agreement levels of each experimental group, indicating the ML model in this group was designed to agree with the majority of people on idpAgreement percent (e.g., 40%).
* `taskId` Int. The 
* `profile` Int. The unique profile ID of the dating profile observed by the subject in each task, corresponding to each dating profile.
* `globalId` Int. Another unique profile ID of the dating profile.
* `decision` Int. The ground truth of the dating profile used in the task. 
* `selfPrediction` Int. The prediction given by the subject before she observe the ML model's prediction.
* `finalPrediction` Int. The prediction given by the subject after she observe the ML model's prediction.
* `finalCorrect` Bool. Whether the final prediction given by the subject is correct or not.
* `agreement` Bool. Whether the initial prediction given by the subject is the same as the ML model's prediction.
* `time` Str. The time that the subject submitted on the task.
* `prediction` Int. The prediction given by the ML model in this task.
* `finalAgreement` Bool. Whether the final prediction given by the subject is the same as the ML model's prediction.
* `mlCorrect` Bool. Whether the ML model's prediction is correct on this task.
* `switch` Bool. Whether the subject switched her prediction after observing the ML model's prediction.




## Licensing & Citing
When using or building upon the data in an academic publication, please consider citing as follows:

Lu, Z., & Yin M. (2021, May). Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks. In *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems* 
 
 [DOI:10.1145/3411764.3445562]


