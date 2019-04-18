# Parkinson's diagnosis

For the Dartmouth class COSC 89.20, Data Science for Health. Project members are Srishti Bagchi, Rachael Chacko, and Cara Van Uden.

## Objective

Here, we will replicate the PLOS ONE study. We will extend their work by seeing which behavioral markers of PD are first present in early-stage (non-severe) PD and see how these behavioral markers change with increased severity of the disease. Through this analysis, we hope to identify early markers of PD for improved early-stage PD diagnosis. We will also potentially extend the previous ML models to implement PD classification with a deep neural network (DNN).

## Innovation

## Dataset

We're using the open-source Kaggle dataset [Tappy Keystroke Data with Parkinson's Patients](https://www.kaggle.com/valkling/tappy-keystroke-data-with-parkinsons-patients). This is the keystroke dataset for the study titled 'High-accuracy detection of early Parkinson's Disease using multiple characteristics of finger movement while typing'. This research paper is [published](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0188226#sec008) in PLOS ONE.

The dataset contains keystroke logs collected from over 200 subjects (103 PD subjects (32 with mild PD severity) and the remainder non-PD controls), with and without Parkinson's Disease (PD), as they typed normally on their own computer (without any supervision) over a period of weeks or months (having initially installed a custom keystroke recording app, Tappy). This dataset has been collected and analyzed in order to indicate that the routine interaction with computer keyboards can be used to detect changes in the characteristics of finger movement in the early stages of PD.

For the user metadata, for each user we have BirthYear, Gender, Parkinsons (PD or control), DiagnosisYear, Sided (left or right), Impact (of the PD, severe or less severe), Tremors, Unified Parkinson's Disease Scale (UPDRS) score, and whether the patient is being treated with Levadopa, DA, MOA-B inhibitors, or

For the keystroke data, each file contains comma separated keystroke data for one month for a particular user. The filename comprises the 10 character code (matching the user details file) and the YYMM of the data. The fields are:

- UserKey: 10 character code for that user
- Date: YYMMDD
- Timestamp: HH:MM:SS.SSS
- Hand: L or R key pressed
- Hold time: Time between press and release for current key mmmm.m (milliseconds)
- Direction: Previous to current LL, LR, RL, RR (and S for a space key)
- Latency time: Time between pressing the previous key and pressing current key (milliseconds)
- Flight time: Time between release of previous key and press of current key (milliseconds)

## References

- [High-Accuracy Detection of Early Parkinson's Disease Using Multiple Characteristics of Finger Movement While Typing](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0188226#sec008)
- [Predicting Severity of Parkinson's Disease with Typing Behavior: A Machine Learning Approach](https://dspace.library.uu.nl/handle/1874/373466)
- [Less is More: Univariate Modelling to Detect Early Parkinson’s Disease from Keystroke Dynamics](https://link.springer.com/chapter/10.1007/978-3-030-01771-2_28)