# Module-End-Assignment-Python-Customer-Support-Ticket-Analyzer
A Python-based project to clean, analyze, and manage customer support ticket data using string manipulation and data structures. Provides insights into ticket priorities, keyword frequency, longest issue descriptions, and unique words to support better customer service analysis.

🎫 Customer Support Ticket Analyzer using Python

📌 Table of Contents

Project Overview

Problem Statement

Project Objectives

Technologies Used

Dataset Information

Project Workflow

1. Preloaded Ticket Data

2. Adding New Tickets

3. Text Cleaning

4. Keyword-Based Analysis

5. Priority Analysis

6. Longest Issue Description

7. Unique Word Extraction

Key Insights

Skills Demonstrated

Conclusion

📖 Project Overview

Project Name: Customer Support Ticket Analyzer

Domain: Customer Service Analytics

Programming Language: Python

Project Type: Data Cleaning and Exploratory Data Analysis

Objective: Analyze customer support tickets to identify common issues, understand service-related feedback, and summarize ticket priorities.

🔍 Project Highlights

Store customer support tickets using a dictionary of lists.

Add new tickets dynamically through user input.

Clean issue descriptions using Python string methods.

Count tickets containing specific keywords.

Analyze ticket distribution by priority.

Identify the ticket with the longest issue description.

Extract unique words from all ticket descriptions.

🎯 Problem Statement

Customer support teams receive numerous service tickets every day.

Analyzing these tickets helps organizations:

Identify common customer complaints.

Understand positive and negative service feedback.

Monitor high-, medium-, and low-priority issues.

Evaluate customer experiences through issue descriptions.

Identify areas that require improvements in support quality.

Solution: Develop a Python-based Ticket Analysis System that stores, cleans, and analyzes customer support ticket data to generate meaningful insights.

🎯 Project Objectives

Organize customer support ticket information.

Allow users to add new tickets without manually assigning ticket numbers.

Validate ticket priorities to maintain consistent data.

Standardize issue descriptions through text cleaning.

Count keyword occurrences at the ticket level.

Calculate the distribution of ticket priorities.

Find the longest issue description based on word count.

Identify and sort unique words across all tickets.

🛠️ Technologies Used

Python: Core programming language.

Dictionary: Stores ticket information using key-value pairs.

Lists: Maintain ticket numbers, customer names, issue descriptions, and priorities.

Functions: Perform reusable keyword-counting operations.

Loops: Process tickets and collect user input.

Conditional Statements: Validate priorities and compare ticket information.

String Methods: Clean and standardize text.

Sets: Extract unique words.

Sorting: Display unique words alphabetically.

📊 Dataset Information

Dataset Structure

The project begins with 10 preloaded customer support tickets.

Column Name

Description

Ticket_No

Unique identification number for each ticket

Customer_Name

Name of the customer who raised the ticket

Issue_Description

Text describing the customer's issue or feedback

Priority

Priority assigned to the ticket: High, Medium, or Low

Sample Dataset

Ticket_No

Customer_Name

Issue_Description

Priority

1

Ravi

Internet not working!!!

High

2

Meera

Slow response, very poor service

Low

3

Sam

GREAT support! issue resolved.

High

4

Anu

okay... need help

Medium

5

Rakesh

not BAD but slow

Low

6

Divya

Excellent guidance, Very Helpful!

High

7

Arjun

good support and good behaviour!

Medium

8

Kiran

Poor handling of technical issue

High

9

Leela

Satisfied. Could be better.

Low

10

Nisha

Good service... quick response.

Medium

Dataset Characteristics

Initial number of tickets: 10

Ticket numbering starts at: 1

New ticket numbering starts at: 11

Priority categories: High, Medium, Low

Issue descriptions contain inconsistent capitalization, punctuation, and spacing.

🔄 Project Workflow

Load the initial ticket data.

Display the original data in a readable format.

Ask the user how many new tickets to add.

Collect customer names, issue descriptions, and priorities.

Validate priority values and assign ticket numbers automatically.

Clean all issue descriptions.

Count tickets containing selected keywords.

Calculate ticket counts by priority.

Find the longest issue description by word count.

Extract and sort all unique words.

Display the final cleaned dataset and analysis results.

1. Preloaded Ticket Data

Objective

Create a dictionary containing the initial 10 tickets.

Store each column as a separate list.

Display the original data before processing.

Python Concepts Used

Dictionary creation

Lists

print()

Expected Outcome

The initial ticket records are displayed.

Each ticket contains a ticket number, customer name, issue description, and priority.

2. Adding New Tickets

Objective

Allow users to add tickets dynamically.

Collect the following information:

Customer name

Issue description

Priority

Business Rules

Ticket numbers must increment automatically from 11.

Priority must be one of the following:

High

Medium

Low

Invalid priorities must be rejected.

New records must be appended to the existing lists.

Python Concepts Used

input()

append()

range()

while loops

if-else statements

Input validation

Expected Outcome

New tickets are added without replacing the existing data.

Every ticket receives a unique, sequential ticket number.

Invalid priority entries are not accepted.

3. Text Cleaning

Objective

Standardize issue descriptions before performing keyword analysis.

Data Cleaning Operations

Remove punctuation: Remove characters such as ., ,, !, ?, and -.

Normalize spaces: Replace multiple spaces with a single space.

Trim spaces: Remove unnecessary spaces from the beginning and end.

Convert to lowercase: Standardize capitalization.

Replace shorthand: Convert ok to okay.

Example of Text Cleaning

Original Text

Cleaned Text

Internet not working!!!

internet not working

slow response, very poor service

slow response very poor service

GREAT support! issue resolved.

great support issue resolved

okay... need help

okay need help

not BAD but slow

not bad but slow

Python Methods Used

.replace()

.split()

' '.join()

.strip()

.lower()

Expected Outcome

Issue descriptions follow a consistent text format.

Unnecessary punctuation and spaces are removed.

Keyword searching becomes more reliable.

4. Keyword-Based Analysis

Objective

Identify how many ticket descriptions contain specific keywords.

Keywords Analyzed

poor

good

slow

excellent

Function Used

count_tickets_with_word(word)

Function Requirements

Accept a keyword as input.

Search ticket descriptions without considering capitalization.

Count the number of ticket descriptions containing the complete word.

Return the total count.

Python Concepts Used

Function definition

Parameters and return values

Loops

String comparison

Conditional statements

Expected Outcome

Number of tickets containing poor.

Number of tickets containing good.

Number of tickets containing slow.

Number of tickets containing excellent.

Business Value

Identify recurring service complaints.

Recognize positive feedback.

Detect possible service-quality concerns.

Understand common themes in customer feedback.

Note: Keyword counts indicate the presence of words, not the overall sentiment of a ticket. For example, a ticket containing good may also include negative feedback.

5. Priority Analysis

Objective

Calculate the number of tickets in each priority category.

Priority Categories

High Priority

Tickets requiring greater attention.

May represent urgent or important customer issues.

Medium Priority

Tickets requiring attention without the highest urgency.

Low Priority

Tickets that may be handled according to normal support procedures.

Analysis Performed

Count tickets with High priority.

Count tickets with Medium priority.

Count tickets with Low priority.

Python Concepts Used

count()

Loops

Conditional statements

Expected Outcome

Total number of high-priority tickets.

Total number of medium-priority tickets.

Total number of low-priority tickets.

Business Value

Helps allocate support resources.

Supports workload planning.

Makes it easier to identify the number of high-priority cases requiring attention.

6. Longest Issue Description

Objective

Identify the ticket with the longest cleaned issue description based on word count.

Information Displayed

Ticket number

Customer name

Cleaned issue description

Total word count

Methodology

Split each cleaned issue description into individual words.

Count the words in each description.

Compare the word counts.

Identify the ticket with the highest word count.

Display the corresponding ticket details.

Python Concepts Used

.split()

len()

Loops

Comparison operators

Dictionary indexing

Expected Outcome

The ticket containing the most words is identified.

Its ticket number, customer name, cleaned description, and word count are displayed.

Business Value

Helps identify tickets containing more detailed descriptions.

May assist support teams in identifying complex or information-rich cases.

Note: A longer description does not necessarily indicate a more complicated issue.

7. Unique Word Extraction

Objective

Extract all distinct words used across the cleaned ticket descriptions.

Steps Performed

Process every cleaned issue description.

Split the text into individual words.

Add the words to a Python set.

Remove duplicate words automatically.

Sort the unique words alphabetically.

Display the total number of unique words and the sorted word list.

Python Concepts Used

Sets

.split()

len()

sorted()

Loops

Expected Outcome

Total count of unique words.

Alphabetically sorted list of unique words.

Business Value

Helps identify the vocabulary commonly used in support tickets.

Provides a foundation for identifying recurring topics.

Supports future text-mining and natural language processing projects.

📈 Key Insights

The following insights can be generated after executing the Python program:

Customer Feedback: Keyword counts help identify descriptions containing positive or negative service-related terms.

Service Quality: Frequent occurrences of words such as poor and slow may indicate areas requiring investigation.

Positive Feedback: Occurrences of good and excellent help identify positive language in ticket descriptions.

Priority Distribution: High-, medium-, and low-priority counts show how support tickets are distributed.

Detailed Tickets: The longest description identifies the ticket containing the most words.

Vocabulary Analysis: Unique-word extraction reveals the range of words customers use to describe their experiences.

Data Quality: Text cleaning makes ticket descriptions more consistent and easier to analyze.

Note: Actual counts and conclusions should be reported using the program's final output.

💡 Recommendations

Prioritize Urgent Tickets

Review high-priority tickets regularly.

Allocate support resources according to urgency and business impact.

Improve Response Time

Investigate tickets containing words such as slow.

Review response-time and resolution-time records before drawing conclusions.

Improve Support Quality

Review tickets containing negative terms such as poor.

Investigate the underlying causes of customer dissatisfaction.

Maintain Data Quality

Standardize issue descriptions.

Validate priority values.

Assign unique ticket numbers consistently.

Extend the Analysis

Add ticket status and resolution time.

Track customer satisfaction ratings.

Introduce sentiment analysis using Python libraries.

Visualize priority distribution and keyword frequency using charts.

🧠 Skills Demonstrated

Python Programming

Variables and data types

Dictionaries and lists

Loops and conditional statements

Functions and return values

User input and validation

Data Cleaning

Text normalization

Punctuation removal

Whitespace handling

Lowercase conversion

Shorthand replacement

Data Analysis

Keyword-based analysis

Frequency counting

Priority distribution

Word-count comparison

Unique-word extraction

Sorting and summarization

Problem-Solving

Automating ticket numbering

Handling invalid inputs

Organizing unstructured text

Generating useful analytical summaries

🚀 Future Enhancements

Import ticket data from CSV or Excel files.

Export cleaned ticket records to CSV.

Create visualizations using Matplotlib or Seaborn.

Add sentiment analysis to classify positive, negative, and neutral feedback.

Identify frequently reported issues using keyword frequency.

Build an interactive dashboard using Streamlit.

Integrate a database to store and manage larger ticket datasets.


Customer_Support_Ticket_Analyzer.ipynb — Contains the Python implementation and analysis.

README.md — Documents the project objectives, workflow, methods, and insights.



🏁 Conclusion

Developed a Python-based system for managing and analyzing customer support tickets.

Implemented dynamic ticket entry and priority validation.

Standardized issue descriptions through text cleaning.

Analyzed selected keywords to identify common feedback terms.

Summarized ticket priorities and identified the longest issue description.

Extracted unique words to support further text analysis.

Overall Outcome: This project demonstrates how Python can be used to transform raw customer support ticket descriptions into structured data and meaningful analytical summaries.
