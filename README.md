# -Youtube-Video-And-Website-Url-Content-Summarization-GEN-AI-App
LangChain Summarizer: Summarize Text From YouTube or Websites

This Streamlit application uses LangChain and the Groq API to summarize content from YouTube videos or any website. The app processes a URL, fetches its content, and generates a concise summary in 300 words using the Gemma-7b-It model.

Features

Summarize text from YouTube videos or website URLs.

Integrated with LangChain and the Groq API for text generation.

Simple Streamlit interface for user interaction.

Prerequisites

Before running the app, ensure you have the following installed:

Python 3.8 or higher

Required Python packages:

streamlit

langchain

langchain-groq

langchain-community

validators

Installation

Clone the repository or copy the code into a Python file:

git clone <repository-url>
cd <repository-directory>

Install the dependencies:

pip install streamlit langchain langchain-groq langchain-community validators

Usage

Obtain a Groq API Key from your Groq account.

Run the application:

streamlit run app.py

Open the application in your browser (default: http://localhost:8501).

Enter the Groq API key and a valid URL (YouTube video or website).

Click "Summarize the Content from YT or Website" to generate a summary.

Code Explanation

Key Components

Input Fields:

Sidebar text input for the Groq API key.

Main input field for entering a URL.

Validation:

Ensures the API key and URL are provided.

Validates the URL format using the validators library.

Content Loading:

Uses YoutubeLoader for YouTube video content.

Uses UnstructuredURLLoader for website content.

Summarization:

Employs a custom prompt template for summarization.

Uses the Gemma-7b-It model via the Groq API to generate the summary.

Prompt Template

The summarization prompt used:

Provide a summary of the following content in 300 words:
Content:{text}

Error Handling

Displays errors for missing inputs or invalid URLs.

Handles exceptions and displays them to the user.
