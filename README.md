# **PROJECT REPORT**

## **INTRODUCTION**
Why was the project undertaken?\
This project was undertaken to explore and build an understanding of the different methods of interpreting listening data music platforms implement to better understand its users and predict user interaction.
Research Questions:
* What artists are most listened to by the person? 
* When do they listen to music the most? (Time of day, time of year, time of month, etc.) 
* What tracks are played most frequently? 
* What track do they skip the most?
* What factors increase the probability that a track will be skipped?

## **SELECTION OF DATA**
The source of the dataset are Spotify users who requested their extended listening history from Spotify. We did a small amount of data munging by converting the time stamp column ('ts') from a string to a datetime value as well as converting it to EST. Many of the columns were dropped such as the audiobook and episode related columns due to irrelevance to answering our questions.\
Data Preview:\
<img width="422" height="299" alt="Screenshot 2026-03-25 at 2 59 23 PM" src="https://github.com/user-attachments/assets/5da29408-d03d-4e3a-bf70-476c7437b6cd" />

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
Was the tested hypothesis true?
## **DISCUSSION**
What might the answer imply and why does it matter?\
Our data is highly biased to specific genres which makes it difficult to abstract our findings for the artists and songs to a larger sample. However, our answer to which times of day have the most listening time could be important in determining appropriate times for maintenance across various music platforms, not just Spotify. \
How does it fit in with what other researchers have found?\
What are the perspectives for future research?

## **SUMMARY**
