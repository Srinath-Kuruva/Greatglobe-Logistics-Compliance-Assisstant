# Greatglobe-Logistics-Compliance-Assisstant

## Copyright and Licensing
© 2026 Srinath Kuruva. All rights reserved.

This project is provided for demonstration purposes only and is not intended for commercial use, modification, or redistribution without explicit written consent from the author. All intellectual property rights remain with the author

## Prerequisites
* googlecolab
* Jupyter

## Overview
Global logistics involves navigating a maze of international regulations, HS codes, and varied tariff obligations. For Greatglobe Logistics, which manages over 500 products for dozens of clients, manual compliance is a major operational bottleneck. This project introduces an Agentic AI Assistant that automates the identification of trade requirements and customs guidance, ensuring that shipments meet regulatory standards efficiently.

## Objective
To build a sophisticated, data-connected AI agent that:

Automates the extraction of logistics and compliance information.

Queries internal databases using natural language via an SQL Agent.

Identifies specific trade obligations (taxes, documents, HS codes) for different product domains.

Reduces regulatory risk and scales support for a growing global client base.

## Technical Stack
Framework: LangChain (Agentic AI Workflows)

LLM: OpenAI gpt-4o-mini

Database Interaction: LangChain SQL Agent

Data Handling: SQLite / Pandas

Language: Python

Environment: Jupyter Notebook

## System Architecture
1. Agentic Workflow
Unlike a simple chatbot, this assistant uses an agentic approach to "think" through a query. It determines which tool is required to find information, executes the search, and verifies the findings against the user's specific request.

2. SQL Database Integration
The assistant is equipped with an SQL Agent tool. When a user asks about a specific product ID, the agent:

Translates the request into a valid SQL query.

Fetches the data from the Greatglobe product database.

Interprets the data to provide context-aware compliance advice.

3. Compliance & Tariff Identification
The system automates the mapping of products to HS codes and identifies applicable tariffs, which is critical for accurate customs declarations and payment calculations.

## Business Impact
Accuracy: Minimizes human oversight in complex international trade documentation.

Operational Efficiency: Drastically reduces the time spent manually researching customs requirements for new product categories.

Scalability: Allows the logistics team to manage a high volume of products across different trade routes with consistent accuracy.

## Setup and Usage
Open ACS_Greatglobe_Logistics_Assistant.ipynb in Jupyter or Google Colab.

Ensure you have an OpenAI API key configured.

Install dependencies:

Bash

pip install langchain openai pysqlite3 pandas
Run the notebook to initialize the database and interact with the Logistics Assistant.
