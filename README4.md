# Project4

This project is titled 'P4'.

The [Stack Overflow 2017 survey] https://www.kaggle.com/stackoverflow/so-survey-2017 data was used here in order to glean some information on professional developers and what to focus on to have the best career.

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Description](#files)
4. [Results](#results)
5. [Acknowledgements](#acknowledgements)

## Installation <a name="installation"></a>
This project uses a Jupyter Notebook running Python 3 with the libraries numpy, pandas and matplotlib. These can be installed using pip but should be included in the Anaconda distribution of Python.

## Project Motivation <a name="motivation"></a>
This project was written as part of the Udacity Data Scientist course. I used the Stack Overflow survey data due to my interest in professional software developers.

## File Descriptions <a name="files"></a>
P4.ipynb contains the Python code for this project.
It assumes that the survey data is in the same directory.
This can be found at https://www.kaggle.com/stackoverflow/so-survey-2017

## Results <a name="results"></a>
Throughout the notebook, I posed three questions related to business or real-world applications:
1. The most frequent languages, technologies, methodologies and technologies used by professionals
2. Average salary for each programming language 
3. Which programming language has the highest job satisfaction

We found out the following:
* JavaScript, C#, Java and SQL and Python are the most 5 used languages by professional developers. From the most used frameworks you can see that most of them is JavaScript based; as AngularJS, Node.js and React. MySQL and SQL server are the most commonly used databases. Agile is the most popular methodology used by professional developers. 
* FThe average salaries range is between ~40K to ~80K. Most popular languages as JavaScript, C#, Java, SQL and Python we found in the first question seem to be in the middle of the range, and that's expected! because the more people who knows that language mean less rareness. At the same time, if the language is less popular like Hack it will be from the highest salaries range
* After taking the highest job satisfaction "Smalltalk" and the lowest "Visual Basic 6", and compare them with the average salaries chart at the second question, I found that "Smalltalk" came in the 2nd place as the highest average salaries, and "Visual Basic 6" is the 2nd lowest; and thats give us the effect and relationship between the salaries range and job satisfaction.

## Acknowledgements <a name="acknowledgements"></a>
Must acknowledge Stack Overflow and Kaggle for the data, whose licensing can be found [here](https://www.kaggle.com/stackoverflow/so-survey-2017). 
Guidance on implementing the notebook and README were taken from learnings in the Udacity course. 
