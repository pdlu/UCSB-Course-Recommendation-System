# UCSB Course Recommendation Project

*Built a course recommendation system for UCSB students using the Academic Curriculum API and the BM25 algorithm to rank courses by relevance.*

## Overview

UCSB offers a wide range of courses across disciplines, yet students often struggle to discover classes that align with their personal interests—especially outside their major. This project aims to streamline the course discovery process by developing a course recommendation system that suggests UCSB classes tailored to student interests.

Using the UCSB Academic Curriculum API, we collect real-time course data. To simulate student profiles, we incorporate an extracurricular dataset from Kaggle, ensuring privacy while modeling diverse interests. Courses are ranked for relevance using the BM25 algorithm, a popular method in information retrieval. The result is a tool that helps students efficiently explore the UCSB curriculum in a more personalized and engaging way.

## Tools and Libraries

-   Academic Curriculum v3.0 API
-   R (tidyverse, tidytext, ggplot2, jsonlite, httr)
-   Python (pandas, BM250kapi, re)
-   Jupyter Notebook
-   Git/Github
-   OpenAi (Chatgpt)

## Methodology

### Data Processing
-   Utilized with UCSB Academic Curriculum v3.0 API to gather real-time and relevant UCSB course information.
-   Collected anonymized student dataset from Kaggle (Students Extracurricular Info Dataset).
-   Conducted exploratory data analysis (EDA) on student extracurricular and course data to identify missing values and better understand the structure and content of the datasets.
-   Applied feature engineering such as text tokenization, fine-grained weighting, and data merging to both datasets for modeling.

### Recommendation System Generation

-   the **BM25 (Okapi BM25)** model:

1.  better handling of term frequency,

2.  strong performance in retrieving the most relevant documents given a query,

3.  document length normalization which gives a more consistent results than TF-IDF,

4.  robustness to varying text lengths, particularly for matching short queries (student interests) to richer documents (course descriptions).

## Result/Discussion

-   Every student's top 5 recommended courses (including course IDs, titles, and BM25 scores) was saved to a separate CSV file for easy verification and allow for quick access to the suggested courses for each student without extensive console output. This file is called "**recommendations.csv**" and can be found in the repository.

-   The recommendation system effectively matches students to broad course interests but struggles with niche topics due to limited student data. Incorporating previous coursework could improve personalization, prevent redundant suggestions, and capture interdisciplinary interests. However, due to privacy concerns, student input would need to be voluntary and securely handled, with no data retention to maintain ethical standards.

## Key Learnings

-   Collected and processed real-time UCSB course data via API integration.
-   Worked with multi-source datasets and applied EDA to assess data quality.
-   Implemented BM25 for relevance-based course recommendations.
-   Gained experience switching between Python and R for analysis.
-   Strengthened team collaboration, task delegation, and project planning.
-   Practiced responsible data use with an emphasis on privacy and ethical handling.

------------------------------------------------------------------------

## Contact

Created by Phuc Lu - feel free to reach out!

[www.linkedin.com/in/phuclu](www.linkedin.com/in/phuclu)
