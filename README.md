<p align="center">

# Trustworthy-ML

This is a repository for the data and analysis code for the paper "Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks".

## Repository Structure

* `rawData` contains the profiles of the speed dating tasks used in the experiments, and raw data dumped from the experiment procedure.

* `data` contains the cleaned data including the predictions of tasks and answers to the questionnaire given by subjects.

* `analysis` contains the analysis code implemented by python and R via jupyter notebook and R markdown.

Each file in `data` and `analysis` starting with "experimentOne","experimentTwo", "experimentThree", are each corresponding to the Experiment 1, 2, 3 in the paper.

## Data Sample

Here attached a data sample of predictions made by subjects in Experiment 1. Each row is a piece of record on a subject making predictions on one task.

`1` indicates "The dating participant wants to see the date again." `0` indicates "The dating participant wants to see the date again."


| workerID | idpAgreement | taskId | profile | globalId | decision | selfPrediction| finalPrediction| selfCorrect| finalCorrect | agreement | time                    | prediction | finalAgreement | mlCorrect | switch |
| -------- | ------------ | -------| ------- | -------- | -------- | ------------- | -------------- | ---------- | ------------ | --------- | --------------------------- | ---------- | -------------- |------------- |------------- |
| 94 | 100 | 4 | 26 | 734 | 0 | 1| 1| FALSE| FALSE | 1 | Mon Feb 10 2020 171422 GMT-0500 (Eastern Standard Time) | 1 | TRUE | FALSE | FALSE |

* `workerId` Int. The unique for each subject assigned in each experiment.
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

Subjects' predictions in Experiment 2 and 3 are similar to those in Experiment 1. Due to the different experiment designs, there can be additional columns in the data as follow:
In Experiment 2: * `acc` Int. The designed accuracy of the ML model's predictions in Phase 1 of the experiment.
In Experiment 3: * `treatment` Int. The designed experimental group of the subject. `0` indicates high confidence agreement - high confidence disagreement group, `1` indicates high confidence agreement - low confidence disagreement group, `2` indicates low confidence agreement - high confidence disagreement group, `0` indicates low confidence agreement - low confidence disagreement group.

Here attached a sample of the data of answers made by subjects to the questionnaire during the Experiment 3. Each row is a piece of record on a subject answering questionnairs.

`1` indicates "The dating participant wants to see the date again." `0` indicates "The dating participant wants to see the date again."


| workerID | idpAgreement | humanPredictAccuracy | humanPredictSelfAccuracy | reliability | faith | competence | understandability | surveyTrust| 
| -------- | ------------ | ---------------------| -----------------------  | ------------| ----- | ---------- | ----------------- | ---------- | 
| 94 | 100 | 80 | 5 | 3 | 5 | 7| 5| 

* `workerId` Int. The unique ID for each subject assigned in each experiment.
* `idpAgreement` Int. The three different agreement levels of each experimental group, indicating the ML model in this group was designed to agree with the majority of people on idpAgreement percent (e.g., 40%).
* `humanPredictAccuracy` Int. How accurate did the subject think the model was between 0 to 100.
* `humanPredictSelfAccuracy` Int. How accurate did the subject think she was between 0 to 100.
* `reliability` Int. The subject's rating on the ML model's reliability between 1 to 7.
* `faith` Int. The subject's faith in the ML model between 1 to 7.
* `competence` Int. The subject's rating on the ML model's competence between 1 to 7. 
* `understandability` Int. The subject's rating on the ML model's understandability between 1 to 7. 
* `surveyTrust` Int. The subject's rating on her overall trust in the ML model between 1 to 7.

For questionnaires in Experiment 1 and 2, they are also similar to those in experiment 3 and have fewer columns since some perceptions are not measured due to the experiment design. Except that on a 7-point Likert scale, we considered subjects who provided a rating of 1–3 asdisagreeing with the statement and encode them as 1. For subjects who provided a rating of 5–7 as agreeing with the statement and encoded them to 1. Due to a mistake in Experiments 1 and 2, for subject’s evaluationson the competence, reliability, understandability, and faith statements, ratings of 6 and 7 were all recorded as 5.





## Licensing & Citing
When using or building upon the data in an academic publication, please consider citing as follows:

Lu, Z., & Yin M. (2021, May). Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks. In *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems* 
 
 [DOI:10.1145/3411764.3445562]


