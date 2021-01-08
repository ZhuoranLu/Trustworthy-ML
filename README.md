<p align="center">

# Trustworthy-ML

This is a repository for the data and analysis code for the paper "Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks".

## Repository Structure

* `rawData` contains the profiles of the speed dating tasks used in the experiments, and raw data dumped from the experiment procedure.

* `data` contains the cleaned data including the predictions of tasks and answers to the questionnaire given by subjects.

* `analysis` contains the analysis code implemented by python and R via jupyter notebook and R markdown.

Each file in `data` and `analysis` starting with "experimentOne","experimentTwo", "experimentThree", are each corresponding to the Experiment 1, 2, 3 in the paper.

## Data Sample

| workerID| idpAgreement   | taskId | profile  | globalId  | decision | selfPrediction |finalPrediction|selfCorrect|finalCorrect|agreement|time|prediction|finalAgreement|mlCorrect|switch|
| ---------------------------------- | ---------------------------------------------- | -------- | ------------------------------------------------------------ | ---------- | ---------- | ------------------------------- |
| Vibrating mesh transducer (VMT)    | 16 mm diameter; ~110±5 kHz operating frequency | 1        | [Comidox](https://www.amazon.com/Comidox-Ultrasonic-Transducer-Humidifier-Replacement/dp/B07P8C5V7W/) | $3.00      | $6.00      | Supplier sells in pairs.        |
| Transducer Driver Board            | Grove Water Atomization v1.0                   | 1        | [Seeed Studio](https://www.seeedstudio.com/Grove-Water-Atomization-v1-0.html) | $10.00     | $10.00     | 

## Licensing & Citing
When using or building upon the data in an academic publication, please consider citing as follows:

Lu, Z., & Yin M. (2021, May). Human Reliance on Machine Learning Models When Performance Feedback is Limited: Heuristics and Risks. In *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems* 
 
 [DOI:10.1145/3411764.3445562]


