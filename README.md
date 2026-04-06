# **PROJECT REPORT**

## Authors: 
- Madison Weidner
- Luna DesRoches
- Nesh Fuertes 

## **INTRODUCTION**
Why was the project undertaken?\
This project was undertaken to explore and build an understanding of the different methods of interpreting listening data music platforms implement to better understand its users and improve user satisfaction with their music recommendation algorithm.

Research Questions:
* What artists are most listened to? 
* When do they listen to music the most? (Time of day, time of year, time of month, etc.) 
* What tracks are played most frequently? 
* What track do they skip the most?
* What factors increase the probability that a track will be skipped?

## **SELECTION OF DATA**
The source of the dataset are Spotify users who requested their extended listening history from Spotify. The dataset had approximately 800000 records dating back to 2019.

Data Preview:\
<img width="422" height="299" alt="Screenshot 2026-03-25 at 2 59 23 PM" src="https://github.com/user-attachments/assets/5da29408-d03d-4e3a-bf70-476c7437b6cd" />

We did a small amount of data munging by converting the time stamp column ('ts') from a string to a EST datetime value. Many of the columns were dropped such as the audiobook and episode related columns due to irrelevance to answering our questions.

Cleaned Data:\
<img width="1207" height="714" alt="Screenshot 2026-03-31 at 3 44 59 PM" src="https://github.com/user-attachments/assets/ee5b7c11-22a6-48ed-be1c-30c6850e630f" />


## **METHODS**
Analysis Tools:
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn

Inference Tools:
* RandomForestClassifier

## **RESULTS**
What answer was found to the research questions; what did the study find?\
What time of day do people listen to music the most? \
<img width="640" height="480" alt="SongsByDay" src="https://github.com/user-attachments/assets/fb1acc22-5c21-4345-8990-7e630fa72493" />
\
<img width="1255" height="615" alt="TopArtists" src="https://github.com/user-attachments/assets/1d65c005-3202-40f7-90f1-aff955d2e8ec" />


Was the tested hypothesis true?
## **DISCUSSION**
What might the answer imply and why does it matter?\
Our data is highly biased to specific genres which makes it difficult to abstract our findings for the artists and songs to a larger sample. However, our answer to which times of day have the most listening time could be important in determining appropriate times for maintenance across various music platforms, not just Spotify. \
How does it fit in with what other researchers have found?\
What are the perspectives for future research?

## **SUMMARY**
This project implements a supervised machine learning approach to determine the likelihood of a song being skipped.  
