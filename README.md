# Module-End-Assignment-Python-Customer-Support-Ticket-Analyzer
A Python-based project to clean, analyze, and manage customer support ticket data using string manipulation and data structures. Provides insights into ticket priorities, keyword frequency, longest issue descriptions, and unique words to support better customer service analysis.

🎫 Customer Support Ticket Analyzer using Python

🐍 A beginner-friendly Python project to clean customer support ticket data, analyze keywords, and generate useful insights into customer feedback and ticket priorities.

📑 Table of Contents

🌟 Project Overview

🎯 Problem Statement

🚀 Project Objectives

🛠️ Technologies Used

📊 Dataset Information

🔄 Project Workflow

📝 Step 1: Preloaded Ticket Data

➕ Step 2: Adding New Tickets

🧹 Step 3: Text Cleaning

🔎 Step 4: Keyword-Based Analysis

📌 Step 5: Priority Analysis

🏆 Step 6: Longest Issue Description

🔤 Step 7: Unique Word Extraction

💡 Key Insights

📈 Recommendations

🧠 Skills Learned

🔮 Future Enhancements

🏁 Conclusion

🌟 Project Overview

🎫 Project Name: Customer Support Ticket Analyzer

🐍 Programming Language: Python

📂 Project Type: Data Cleaning and Analysis

🏢 Domain: Customer Support Analytics

🎯 Main Goal: Analyze customer support tickets to identify common issues, feedback keywords, and ticket priorities.

✨ What Does This Project Do?

📥 Stores customer support ticket information.

➕ Allows users to add new tickets.

🔢 Generates ticket numbers automatically.

🧹 Cleans and standardizes issue descriptions.

🔎 Counts tickets containing specific keywords.

📊 Analyzes High, Medium, and Low priorities.

🏆 Finds the ticket with the longest issue description.

🔤 Extracts unique words from all ticket descriptions.

🎯 Problem Statement

Customer support teams receive many service tickets every day.

Analyzing these tickets helps to:

🔴 Identify common customer complaints.

🟢 Recognize positive customer feedback.

🟡 Understand ticket priority distribution.

⏱️ Identify descriptions mentioning slow service.

📊 Improve data organization and reporting.

💡 Discover opportunities to improve customer satisfaction.

💻 Solution: Build a Python-based system that cleans, processes, and analyzes customer support tickets to generate meaningful insights.

🚀 Project Objectives

✅ Store ticket information using a dictionary of lists.

✅ Allow users to add new tickets dynamically.

✅ Validate ticket priorities.

✅ Assign ticket numbers automatically.

✅ Clean issue descriptions using Python string methods.

✅ Count tickets containing selected keywords.

✅ Calculate the number of tickets by priority.

✅ Find the longest issue description based on word count.

✅ Extract and sort unique words.

✅ Display the final cleaned dataset and analysis results.

🛠️ Technologies Used

Technology / Concept

Purpose

🐍 Python

Main programming language

📚 Dictionary

Store ticket information

📋 Lists

Maintain ticket records

🔁 Loops

Process tickets and user inputs

🔀 Conditional Statements

Validate priorities and compare values

⚙️ Functions

Perform reusable keyword analysis

✂️ String Methods

Clean and standardize text

🔢 count()

Count occurrences of priority values

🧩 Sets

Extract unique words

🔤 sorted()

Sort unique words alphabetically

📊 Dataset Information

📌 Initial Records: 10 customer support tickets

🔢 Ticket Numbers: 1–10

➕ New Ticket Numbers: Starting from 11

👥 Customers: Ravi, Meera, Sam, Anu, Rakesh, Divya, Arjun, Kiran, Leela, and Nisha

🎯 Priority Categories: High, Medium, Low

📋 Dataset Columns

Column Name

Description

Ticket_No

Unique ticket identification number

Customer_Name

Name of the customer

Issue_Description

Description of the customer's issue

Priority

Priority assigned to the ticket

🗂️ Sample Dataset

Ticket_No

Customer_Name

Issue_Description

Priority

1

Ravi

Internet not working!!!

🔴 High

2

Meera

Slow response, very poor service

🟢 Low

3

Sam

GREAT support! issue resolved.

🔴 High

4

Anu

okay... need help

🟡 Medium

5

Rakesh

not BAD but slow

🟢 Low

6

Divya

Excellent guidance, Very Helpful!

🔴 High

7

Arjun

good support and good behaviour!

🟡 Medium

8

Kiran

Poor handling of technical issue

🔴 High

9

Leela

Satisfied. Could be better.

🟢 Low

10

Nisha

Good service... quick response.

🟡 Medium

🔄 Project Workflow

<details>
<summary>🔽 Click to view the complete workflow</summary>

📥 Load the initial ticket data.

🖨️ Display the original ticket records.

➕ Ask the user how many tickets to add.

👤 Collect customer name and issue description.

🎯 Validate ticket priority.

🔢 Assign ticket numbers automatically.

🧹 Clean all issue descriptions.

🔎 Count selected keywords.

📊 Analyze ticket priorities.

🏆 Identify the longest issue description.

🔤 Extract unique words.

📋 Display the final cleaned dataset and insights.

</details>

📝 Step 1: Preloaded Ticket Data

🎯 Objective

Create a dictionary containing 10 customer support tickets.

Store ticket details in separate lists.

Display the initial dataset in a readable format.

🐍 Python Concepts

📌 Dictionary creation

📋 Lists

🖨️ print()

✅ Expected Result

All 10 initial tickets are displayed.

Each ticket contains a ticket number, customer name, issue description, and priority.

➕ Step 2: Adding New Tickets

🎯 Objective

Allow users to add new customer support tickets through input.

📝 Information Collected

👤 Customer Name

💬 Issue Description

🎯 Priority

📌 Rules

🔢 Ticket numbers automatically start from 11.

🔴 Accept High as a valid priority.

🟡 Accept Medium as a valid priority.

🟢 Accept Low as a valid priority.

⚠️ Reject invalid priority values.

➕ Append new ticket details to the existing lists.

🐍 Python Concepts

input()

append()

range()

while loop

if-else statements

💡 Example

How many new tickets do you want to add? 2

Enter customer name: John
Enter issue description: Internet connection is slow
Enter priority: High

Enter customer name: Priya
Enter issue description: Good customer service
Enter priority: Medium

✅ Expected Result

Two new tickets are added.

Their ticket numbers are 11 and 12.

Invalid priorities are rejected until a valid priority is entered.

🧹 Step 3: Text Cleaning

🎯 Objective

Clean issue descriptions to make the text consistent and easier to analyze.

🧽 Cleaning Operations

✂️ Punctuation Removal

Remove ., ,, !, ?, and -.

🔡 Lowercase Conversion

Convert uppercase letters to lowercase.

🧹 Whitespace Removal

Remove unnecessary spaces at the beginning and end.

📏 Space Standardization

Replace multiple spaces with a single space.

🔄 Shorthand Replacement

Replace ok with okay when it appears as a standalone word.

🐍 Python Methods Used

.replace()

.split()

' '.join()

.strip()

.lower()

📋 Before and After Cleaning

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

Excellent guidance, Very Helpful!

excellent guidance very helpful

✅ Expected Result

Clean and standardized descriptions.

Consistent capitalization.

Removal of unwanted punctuation and extra spaces.

🔎 Step 4: Keyword-Based Analysis

🎯 Objective

Count how many ticket descriptions contain specific keywords.

🔑 Keywords Analyzed

🔴 poor

🟢 good

🟡 slow

🔵 excellent

⚙️ Function Created

def count_tickets_with_word(word):
    count = 0

    for description in ticket_data['Issue_Description']:
        words = description.lower().split()

        if word.lower() in words:
            count += 1

    return count

📊 Display Keyword Counts

keywords = ['poor', 'good', 'slow', 'excellent']

for word in keywords:
    print(word, ':', count_tickets_with_word(word))

🐍 Python Concepts

⚙️ Function definition

🔁 Loops

🔡 String methods

📋 Lists

🔍 Conditional statements

↩️ Return values

💡 What Can We Learn?

🔴 Poor: Helps identify tickets containing negative service-related language.

🟢 Good: Helps identify tickets containing positive language.

🟡 Slow: Highlights feedback mentioning slow service or response.

🔵 Excellent: Identifies tickets containing strongly positive language.

📌 The function counts tickets containing a complete word, not the total number of times that word appears. A keyword count alone does not determine the overall sentiment of a ticket.

📌 Step 5: Priority Analysis

🎯 Objective

Calculate the number of tickets in each priority category.

🚦 Priority Categories

🔴 High Priority

Tickets requiring urgent attention according to support rules.

🟡 Medium Priority

Tickets requiring attention at a moderate level.

🟢 Low Priority

Tickets that can be handled according to normal support procedures.

📊 Analysis Performed

🔴 Count High-priority tickets.

🟡 Count Medium-priority tickets.

🟢 Count Low-priority tickets.

🐍 Python Example

print("High Priority:",
      ticket_data['Priority'].count('High'))

print("Medium Priority:",
      ticket_data['Priority'].count('Medium'))

print("Low Priority:",
      ticket_data['Priority'].count('Low'))

💼 Business Benefits

📍 Understand the support team's workload.

⏱️ Identify the number of tickets requiring urgent attention.

👥 Help allocate support resources.

📊 Monitor the distribution of ticket priorities.

🏆 Step 6: Longest Issue Description

🎯 Objective

Find the ticket containing the highest number of words.

🔍 Analysis Steps

🧹 Use the cleaned issue descriptions.

✂️ Split each description into words.

🔢 Calculate the word count.

🔎 Compare the word counts.

🏆 Identify the ticket with the highest count.

📋 Information Displayed

🎫 Ticket Number

👤 Customer Name

💬 Cleaned Issue Description

🔢 Word Count

🐍 Python Example

word_counts = [
    len(description.split())
    for description in ticket_data['Issue_Description']
]

max_index = word_counts.index(max(word_counts))

print("Ticket Number:",
      ticket_data['Ticket_No'][max_index])

print("Customer Name:",
      ticket_data['Customer_Name'][max_index])

print("Issue Description:",
      ticket_data['Issue_Description'][max_index])

print("Word Count:", word_counts[max_index])

💡 Business Benefit

📝 Identifies the most detailed ticket description.

🔍 Helps locate tickets containing more written information.

📊 Demonstrates the use of word counts for text analysis.

🔤 Step 7: Unique Word Extraction

🎯 Objective

Extract all unique words used across the cleaned issue descriptions.

🔍 Analysis Steps

📋 Collect all cleaned issue descriptions.

✂️ Split descriptions into individual words.

🧩 Store the words in a set.

🔄 Remove duplicate words automatically.

🔤 Sort the words alphabetically.

🔢 Calculate the number of unique words.

🐍 Python Example

unique_words = set()

for description in ticket_data['Issue_Description']:
    unique_words.update(description.split())

print("Number of Unique Words:", len(unique_words))
print("Sorted Unique Words:", sorted(unique_words))

🧠 Python Concepts

Sets

Loops

.split()

.update()

len()

sorted()

💡 Business Benefit

🔎 Understand the vocabulary used by customers.

📊 Identify recurring terms.

🧠 Build a foundation for future text-mining projects.

💡 Key Insights

The program can generate the following insights from the final output:

🔴 Service Complaints

Analyze tickets containing words such as poor and slow.

🟢 Positive Feedback

Identify descriptions containing good and excellent.

📊 Priority Distribution

Compare the numbers of High-, Medium-, and Low-priority tickets.

🏆 Longest Description

Identify the ticket with the highest word count.

🔤 Unique Vocabulary

Discover the different words used across all ticket descriptions.

🧹 Data Quality

Standardize text before performing analysis.

📌 Actual counts and conclusions should be taken from the program output after all new tickets have been added.

📈 Recommendations

🚨 Improve Ticket Prioritization

Review high-priority tickets regularly.

⏱️ Monitor Response Time

Investigate complaints mentioning slow responses.

💬 Improve Customer Experience

Review negative feedback to understand the underlying issues.

🧹 Maintain Data Quality

Standardize descriptions and validate priority values.

📊 Track Performance

Monitor ticket volume and priority distribution over time.

🧠 Extend Text Analysis

Add sentiment analysis to classify positive, negative, and neutral feedback.

🧠 Skills Learned

🐍 Python Programming

Variables and data types

Lists and dictionaries

Loops and conditional statements

Functions and return values

User input and validation

🧹 Data Cleaning

Lowercase conversion

Punctuation removal

Whitespace standardization

Text replacement

Data consistency

📊 Data Analysis

Keyword counting

Priority analysis

Word-count comparison

Unique-word extraction

Sorting and summarization

💼 Problem-Solving

Automatic ticket numbering

Input validation

Organizing text data

Generating meaningful insights

🔮 Future Enhancements

📂 Import ticket data from CSV and Excel files.

💾 Export cleaned data into CSV format.

📊 Create charts using Matplotlib.

🧠 Implement sentiment analysis using Python libraries.

🔎 Identify frequently reported issues.

🌐 Build an interactive dashboard using Streamlit.

🗄️ Store tickets in a MySQL database.

📈 Track response time and resolution time.

📁 Suggested GitHub Repository Structure

Customer-Support-Ticket-Analyzer/
│
├── Customer_Support_Ticket_Analyzer.ipynb
├── README.md
└── screenshots/
    └── analysis_output.png

📂 File Description

🐍 Customer_Support_Ticket_Analyzer.ipynb

Contains the Python code, cleaning process, and analysis.

📘 README.md

Explains the project, objectives, methods, and insights.

🖼️ screenshots/

Stores screenshots showing the program output.

🏁 Conclusion

🎉 Project Outcomes

✅ Created a system to manage customer support ticket data.

✅ Added new tickets with automatic numbering.

✅ Validated ticket priorities.

✅ Cleaned issue descriptions using Python.

✅ Analyzed keywords in customer feedback.

✅ Calculated ticket priority counts.

✅ Identified the longest issue description.

✅ Extracted and sorted unique words.

🌟 Final Takeaway

This project demonstrates how Python can transform raw customer support text into clean, organized, and meaningful information that supports better ticket analysis and customer service improvement.
