# -Youtube-Video-And-Website-Url-Content-Summarization-GEN-AI-App


This Streamlit application uses LangChain and the Groq API to summarize content from YouTube videos or any website. The app processes a URL, fetches its content, and generates a concise summary in 300 words using the Gemma-7b-It model.

### Features

Summarize text from YouTube videos or website URLs.

Integrated with LangChain and the Groq API for text generation.

Simple Streamlit interface for user interaction.

### Prerequisites

Before running the app, ensure you have the following installed:

Python 3.8 or higher

Required Python packages:

streamlit

langchain

langchain-groq

langchain-community

validators

### Installation

Clone the repository or copy the code into a Python file:

git clone <repository-url>
cd <repository-directory>

### Install the dependencies:

pip install streamlit langchain langchain-groq langchain-community validators

Usage

Obtain a Groq API Key from your Groq account.

### Run the application:

streamlit run app.py


### Key Components

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



Error Handling

Displays errors for missing inputs or invalid URLs.

Handles exceptions and displays them to the user.
