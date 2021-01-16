#!/usr/bin/env python
# coding: utf-8

# # 1. Pick a dataset: I chose tthe 2017 Stack Overflow results in my project.

# In[6]:


import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
get_ipython().run_line_magic('matplotlib', 'inline')


# In[7]:


pd.set_option('display.max_columns', None)
df = pd.read_csv('/Users/ruba/Downloads/udacity/P4/P4-B/survey_results_public.csv')
schema = pd.read_csv('/Users/ruba/Downloads/udacity/P4/P4-B/survey_results_schema.csv')
df.head()


# # 2. Pose at least three questions related to business or real-world applications of how the data could be used.

# 1.The most frequent languages, technologies, methodologies and technologies used by professionals
# 
# 2.Average salary for each programming language
# 
# 3.Which programming language has the highest job satisfaction

# # 3. Create a Jupyter Notebook, using any associated packages you'd like, to:
# 3-A Prepare data
# 
# 3-B Analyze 
# 
# 3-C Model 
# 
# 3-D Visualize 

# In[8]:


q1 = df[['Professional', 'HaveWorkedLanguage', 'HaveWorkedFramework', 'HaveWorkedDatabase', 'Methodology']]
q1 = q1[q1.Professional == "Professional developer"]
q1.head()


# In[9]:


# 1.The most frequent languages, technologies, methodologies and technologies used by professionals
# 1.A: The most commonly used languages
languages = q1['HaveWorkedLanguage'].str.split('; ', expand=True).stack().value_counts()
plt.figure(figsize=(10,10))
languages.plot(kind="bar")
plt.savefig('languages')


# In[10]:


# 1.B: The most commonly used frameworks
frameworks = q1['HaveWorkedFramework'].str.split('; ', expand=True).stack().value_counts()
plt.figure(figsize=(10,10))
frameworks.plot(kind="bar")
plt.savefig('frameworks')


# In[11]:


# 1.C: The most commonly used databases
databases = q1['HaveWorkedDatabase'].str.split('; ', expand=True).stack().value_counts()
plt.figure(figsize=(10,10))
databases.plot(kind="bar")
plt.savefig('databses')


# In[12]:


# 1.D: The most commonly used methodologies
methodologies = q1['Methodology'].str.split('; ', expand=True).stack().value_counts()
plt.figure(figsize=(10,10))
methodologies.plot(kind="bar")
plt.savefig('methodologies')


# # Evaluatation:
# 1.A: JavaScript, C#, Java and SQL and Python are the most 5 used languages by professional developers.
# 
# 2.B: From the most used frameworks you can see that most of them is JavaScript based; as AngularJS, Node.js and React.
# 
# 3.C: MySQL and SQL server are the most commonly used databases
# 
# 4.D: Agile is the most popular methodology used by professional developers.

# In[13]:


# 2.Average salary for each programming language


# The data will be prepared here by selecting the desired columns and only using the rows where a professional devloper was taking the survey. All rows were dropped where the Professional column did not equal "Professional Developer" as I was only interested in Professional Developers.If the row had Salary or HaveWorkedLanguage as Nan then the row would be dropped. This is becase I was trying to find a correlation between the two and therefore they needed to exist.  This was the only way in which I needed to handle Nan values and categorical values.

# In[14]:


q2 = df[['Professional', 'HaveWorkedLanguage', 'Salary']]
q2 = q2[q2.Professional == "Professional developer"]
q2 = q2.drop('Professional', 1)
q2 = q2.dropna(subset=['Salary', 'HaveWorkedLanguage'], axis=0)
q2.head()


# In[15]:


def split_column(column_to_split, delimeter, column_to_store, df):
    """
    Method to split a columns values by a provided delimeter while
    retaining the associated value of another column.
    
    :param str column_to_split: column whose values are to be split
    :param str delimeter: delimeter to split by
    :param str columns_to_store: column who's data must be stored along split rows
    :param DataFrame df: dataframe to use
    """
    split_col = pd.DataFrame(columns = [column_to_split, column_to_store])
    for index, row in df.iterrows():
        columns = row[column_to_split].split(delimeter)
        for c in columns:
            split_col.loc[len(split_col)] = [c, row[column_to_store]]
    return split_col


# In[16]:


split_languages = split_column("HaveWorkedLanguage", "; ", "Salary", q2)
split_languages.head()


# In[17]:


q2_answer = split_languages.groupby(['HaveWorkedLanguage']).mean()['Salary'].sort_values()
plt.figure(figsize=(10,10))
q2_answer.plot(kind = 'bar')
plt.savefig('q2')


# # Evaluatation:
# 1.From the chart the average salaries range is between ~40K to ~80K. 
# 
# 2.Most popular languages as JavaScript, C#, Java, SQL and Python we found in the first question seem to be in the middle of the range, and that's expected! because the more people who knows that language mean less rareness.
# 
# 3. At the same time, if the language is less popular like Hack it will be from the highest salaries range. 

# In[18]:


# 3.Which programming language has the highest job satisfaction


# The data will be prepared here by selecting the desired columns and only using the rows where a professional devloper was taking the survey All rows were dropped where the Professional column did not equal "Professional Developer" as I was only interested in Professional Developers.If the row had JobSatisfaction or HaveWorkedLanguage as Nan then the row would be dropped. This is becase I was trying to find a correlation between the two and therefore they needed to exist. This was the only way in which I needed to handle Nan values and categorical values.

# In[19]:


q3 = df[['Professional', 'HaveWorkedLanguage', 'JobSatisfaction']]
q3 = q3[q3.Professional == "Professional developer"]
q3 = q3.drop('Professional', 1)
q3 = q3.dropna(subset=['JobSatisfaction', 'HaveWorkedLanguage'], axis=0)
q3.head()


# In[20]:


split_languages_q3 = split_column("HaveWorkedLanguage", "; ", "JobSatisfaction", q3)
q3_answer = split_languages_q3.groupby(['HaveWorkedLanguage']).mean()['JobSatisfaction'].sort_values()
q3_answer.head(50)


# In[21]:


plt.figure(figsize=(10,10))
q3_answer.plot(kind = 'bar')
plt.savefig('q3')


# # Evaluatation:
# If we take the highest job satisfaction "Smalltalk" and the lowest "Visual Basic 6", and compare them with the average salaries chart at the second question, then we will find that "Smalltalk" came in the 2nd place as the highest average salaries, and "Visual Basic 6" is the 2nd lowest; and thats give us the effect of the salaries range on job satisfaction. 

# In[ ]:




