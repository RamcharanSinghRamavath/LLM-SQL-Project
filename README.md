
# 🧠 LLM-Powered SQL Assistant (End-to-End)

An end-to-end Generative AI project that enables users to interact with a MySQL database using natural language.
The system leverages Large Language Models (LLMs) and LangChain to automatically convert user questions into accurate SQL queries, execute them on a live database, and return meaningful insights through an interactive UI.

## 🚀 Overview

In real-world businesses, non-technical users often struggle to extract insights from databases.
This project solves that problem by allowing users to “talk to a database” using plain English.

A store manager can ask questions such as:

How many white Adidas T-shirts are currently in stock?

What will be the total sales if all extra-small T-shirts are sold after discounts?

The system intelligently:

Understands the natural language query

Converts it into an optimized SQL query

Executes it on a MySQL database

Displays real-time results via a Streamlit interface

## ✨ Key Features

Natural Language → SQL conversion using LLMs

Real-time execution on a MySQL relational database

Interactive Streamlit-based web interface

Few-shot prompting to improve SQL accuracy

Vector-based semantic understanding using embeddings

Modular and scalable architecture

## 🧩 How It Works

User enters a question in natural language

LangChain uses few-shot prompts to guide the LLM

The LLM generates a valid SQL query

SQL query is executed on the MySQL database

Results are returned and displayed in the UI

## 🛠️ Tech Stack

Programming Language: Python

Database: MySQL

LLM Framework: LangChain

Model: Google PaLM

Embeddings: Hugging Face

Vector Store: ChromaDB

UI: Streamlit

AI Concepts: Prompt Engineering, Few-Shot Learning, NLP

## ⚙️ Installation & Setup

1.Clone this repository to your local machine using:

```bash
git clone https://github.com/RamcharanSinghRamavath/LLM-SQL-Project.git
cd LLM-SQL-Project
```
2.Navigate to the project directory:

```bash
  cd 4_sqldb_tshirts
```
3. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Acquire an api key through makersuite.google.com and put it in .env file

```bash
  GOOGLE_API_KEY="your_api_key_here"
```
5. For database setup, run database/db_creation_atliq_t_shirts.sql in your MySQL workbench

## Usage

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

2.The web app will open in your browser where you can ask questions

## Sample Questions
  - How many total t shirts are left in total in stock?
  - How many t-shirts do we have left for Nike in XS size and white color?
  - How much is the total price of the inventory for all S-size t-shirts?
  - How much sales amount will be generated if we sell all small size adidas shirts today after discounts?
  
## Project Structure

- main.py: The main Streamlit application script.
- langchain_helper.py: This has all the langchain code
- requirements.txt: A list of required Python packages for the project.
- few_shots.py: Contains few shot prompts
- .env: Configuration file for storing your Google API key.

 ## 📈 Use Cases

Business analytics for non-technical users

Conversational BI systems

AI-powered database querying tools

Data analyst and GenAI portfolio project

## 🔮 Future Enhancements

Support for multiple databases (PostgreSQL, SQLite)

Role-based authentication

Query result visualizations (charts & dashboards)

Power BI / Tableau integration

Deployment on cloud platforms
