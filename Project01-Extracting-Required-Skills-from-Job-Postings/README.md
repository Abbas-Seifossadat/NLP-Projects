# Project: Job Description Analyzer – Extracting Required Skills from Job Postings

## Objective
This project focuses on extracting and categorizing required skills from job descriptions using **spaCy’s Named Entity Recognition (NER)** and **NLTK preprocessing**. The goal is to identify trends in job requirements and analyze the most in-demand skills across various industries.

## ??? Tools & Libraries
- **Python**
- **NLTK** (Natural Language Toolkit) for text preprocessing
- **spaCy** for Named Entity Recognition (NER)
- **Pandas** for data manipulation and analysis

## Dataset
The dataset used in this project is a CSV file containing job descriptions from different industries (e.g., IT, Healthcare, Finance, Marketing). It includes columns such as:
- `company`: Name of the company
- `position`: Job title
- `Job Description`: Detailed job description
- `industry`: Industry category

## Project Steps
1. **Load the Dataset**: The dataset is loaded using Pandas, and basic information about the dataset is displayed.
2. **Preprocessing**: 
   - Text is cleaned by removing stopwords, punctuation, and unnecessary characters.
   - NLTK is used for tokenization and stopword removal.
3. **Extract Skills Using NER**:
   - spaCy’s NER is used to identify and extract skills from job descriptions.
   - A predefined list of common technical skills is used to enhance skill extraction.
4. **Identify Most In-Demand Skills**:
   - A word frequency distribution is created to count the most frequently mentioned skills.
   - The top 10 most in-demand skills are identified.
5. **Categorize Skills by Industry**:
   - Skills are grouped by industry, and the most in-demand skills for each industry are analyzed.

## Results
- **Top 10 Most In-Demand Skills**: The most frequently mentioned skills across all industries are identified and displayed.
- **Skills by Industry**: Skills are categorized by industry, providing insights into the specific requirements for different sectors.

## Key Findings
- The most in-demand skills across industries include **Excel**, **communication**, and **analytical skills**.
- Industries like **Information Technology** emphasize skills such as **cloud computing**, **big data**, and **ERP systems**.
- **Finance** and **Accounting & Legal** industries focus on **Excel**, **SQL**, and **legal compliance**.