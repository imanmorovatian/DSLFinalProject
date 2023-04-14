# Intention Detection Using SVM 

This repository contains the final project of the Data Science Lab course at Politecnico di Torino, in January 2023. In this project, we work on an intention detection problem. Intent detection is a crucial task in the field of natural language processing (NLP) and speech recognition. It involves identifying the underlying intention or purpose of a spoken or written statement. In the context of audio intent detection, the system must be able to accurately interpret the user’s spoken words and determine their intended meaning. The dataset consists of a collection of audio files in a WAV format. Several attributes characterize each record. The following is a short description of each of them.

* path: the path of the audio file.
* speakerId: the id of the speaker.
* action: the type of action required through the intent.
* object: the device involved by intent.
* Self-reported fluency level: the speaking fluency of the speaker.
* First Language spoken: the first language spoken by the speaker.
* Current language used for work/school: the main language spoken by the speaker during daily activities.
* gender: the gender of the speaker.
* ageRange: the age range of the speaker

An intent is given by the combination of an action with an object, therefore the information in the two respective columns must be combined to obtain the label to be used to address this task. The way this information should be combined is a simple string concatenation (e.g., if the action is “increase” and the object is “volume”, the corresponding intent will be “increasevolume”).

The dataset is located at this [Link](https://drive.google.com/file/d/1gUPpqPTlgfzIyDU4eG6t5HoTlK5inLO4/view?usp=sharing). Within the archive, there are the following elements:
* audio: a folder containing all the audio files in WAV format.
* development.csv: a comma-separated values file containing the records from the development set. This portion does have the action and object columns, which you should use
to obtain the labels to train and validate your models.
* evaluation.csv: a comma-separated values file containing the records corresponding
to the evaluation set. This portion does not have the action and object columns.
* sample_submission.csv: a sample submission file.
