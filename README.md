# xtapod - Database Developer Exercise

## Objectives

The goal of this exercise is to examine your ability to query data efficiently and build effective data models.  You will be asked in this exercise to demonstrate two things:

- Query a large data set to return facts on the dataset
- Model the data in a way that would allow for an analyst to extract key facts from the data without a complete understanding of the dataset as a whole.

## Exercise Completion

Please download the zip file of this repository, modify locally, zip, and return to Maria.  **Forks of this repository will not be accepted.**

## Background

The United States Department of Education keeps a significant amount of data about the performance of colleges and universities in the U.S.  This data set includes information about tuition, grants, completion rate, faculty salary, transfer rates, etc. and is also presented broken down by a number of demographic factors.  The raw data for this from December 2019 can be found in this repository along with a complete data dictionary.

# Task 1: Load the data

The first task you will have is loading this dataset into a database.  We do not expect you to normalize the data - only to load it so that it can be queried.  Success for this task will be based on documentation you provide so that a reviewer could load the data and eventually test your queries against it.  Please provide the documentation in a markdown file or other document in your submission.

# Task 2: Write analytical queries

For the next task, we will ask you to provide queries that answer the following questions.  Note that we are providing the data fields required in the query.  You must provide the query and the result you received for each query in a document with your submission.

1.  What was the average in-state tuition (TUITIONFEE_IN) for families with an average family income (FAMINC_IND) of < $100,000 USD?
1.  How many schools awarded a Percentage of Degrees in Engineering (PCIP14) of > 10% where there was a minimum enrollment of undergraduate students (UG) of 5,000?
1.  Of all of the schools in the 25 percentile of SAT math scores (SATMT25) how many students were ultimately awarded a Bachelor's Degree in Legal Professions and Studies (CIP22BACHL)?

| Note: It is possible that even a correct query will return a result that is 0.

# Task 3: Data modeling for analytics

For the final task, we will ask you to design a data model that allows for simplified analysis by people with limited database knowledge.  A user is looking to build a report that will allow them to track the following information:

- Admission Rate (ADM_RATE)
- Average Faculty Salary (AVGFACSAL)
- Undergradate Enrollment Rate (UG)
- Percent that died within 2 years at original institution (DEATH_YR2_RT)

We would like to be able to slice this data up by:

- Region (REGION)
- Women-only colleges (WOMENONLY)
- Commercial Status (CONTROL)
- Accreditor (ACCREDAGENCY)

Please provide any and all instructions on how you would make this data available for use by a report generation tool.