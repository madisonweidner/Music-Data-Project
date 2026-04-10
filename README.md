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
* What time of day do they listen to music the most?
* What tracks are played most frequently? 
* What tracks do they skip the most?
* What factors increase the probability that a track will be skipped?

## **SELECTION OF DATA**
The source of the dataset are Spotify users who requested their extended listening history from Spotify. The dataset had approximately 800000 records dating back to 2019.

Data Preview:\
<img width="422" height="299" alt="Screenshot 2026-03-25 at 2 59 23 PM" src="https://github.com/user-attachments/assets/5da29408-d03d-4e3a-bf70-476c7437b6cd" />

We did a small amount of data munging by converting the time stamp column ('ts') from a string to a EST datetime value. Many of the columns were dropped such as the audiobook and episode related columns due to irrelevance to answering our questions.

For the track skipping question, we excluded songs with less than 10 listens from the dataset so songs that the spotify algorithm persistently tries to include would appear in the top 30 skipped songs over songs with a singular play and immediate skip.  

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
What artists are most listened to?
<img width="1255" height="615" alt="TopArtists" src="https://github.com/user-attachments/assets/66641e09-e68d-4e4f-89eb-4815dc95bf5d" />


What time of day do they listen to music the most? 

The listening data follows a workday curve where listening rises in the late morning and peaks in the early afternoon (1-2pm). 

<img width="594" height="455" alt="SongsByDay" src="https://github.com/user-attachments/assets/7083731b-f8d1-4242-a056-9d914195d30b" />

\
What tracks are played most frequently?

<img width="571" height="563" alt="TopFreqPlays" src="https://github.com/user-attachments/assets/0c5755aa-9775-4c22-96de-85eda2d75e67" />

Multiple of the tracks that share a similar listening frequency come from the same album which could suggest that the user listened to the entire album in one sitting. 

What tracks do they skip the most?

<img width="567" height="566" alt="TopSkipped" src="https://github.com/user-attachments/assets/b9506fee-0581-46cd-9b8a-d470fb87c74e" />


What factors increase the probability that a track will be skipped?


## **DISCUSSION**
What might the answer imply and why does it matter?

Our data is highly biased to specific genres which makes it difficult to abstract our findings for the artists and songs to a larger sample. However, our answer to which times of day have the most listening time could be important in determining appropriate times for maintenance across various music platforms, not just Spotify.

How does it fit in with what other researchers have found?

Future research would delve more into invididually searching a person's history and comparing trends from their early listening to their most current data rather than looking across everyone's history as an entire dataset. 

## **SUMMARY**
This project implements a supervised machine learning approach to determine the likelihood of a song being skipped.  
