# DiverseLens

DiverseLens is a platform aimed at combating bias and misinformation while providing users with personalized recommendations for diverse sources of information. By analyzing users' reading habits, identifying potential biases, and offering curated content from a range of perspectives, DiverseLens encourages critical thinking and helps reduce echo chambers in today's digital landscape.

## Background

The genesis of DiverseLens stems from a confluence of personal experiences and societal observations. In today's digital age, the proliferation of misinformation and biased narratives on social media platforms and news outlets has become ubiquitous. Additionally, a fascination with machine learning and natural language processing further motivated the exploration of innovative solutions in this domain.



## Project Construction Method

ML Model:

Importing Libraries: You begin by importing necessary libraries such as trafilatura for web scraping, textwrap for text formatting,
 requests for making HTTP requests, urllib.parse for URL parsing, IPython.display for displaying Markdown, google.generativeai
 for accessing Generative AI models, sumy for text summarization, and nltk for natural language processing tasks.

Configuration and Setup: We configure the Generative AI model by providing an API key and initializing a GenerativeModel object.

Utility Functions:
to_markdown: Formats text as Markdown.
news_sources: Searches for news articles based on a query and returns a list of URLs.
extract_text_from_url: Extracts text content from a given URL using trafilatura.
textrank_summarize: Generates a summary of the text using TextRank summarization

extract_keywords: Extracts keywords from text using NLTK.
insights: Gathers news articles related to a statement, processes the corpus, and generates insights using a Generative AI model.
llm_response: Constructs a prompt for the Generative AI model and generates a response.

Project Workflow:
The insights function takes a statement as input.
It searches for news articles related to the statement and extracts text content from those articles.
It generates insights on the statement by providing information on bias, factuality, and a summary of key points from the verified information in the corpus.
The insights are generated using a Generative AI model by passing a constructed prompt.
Interaction:
The code  primarily structured for programmatic interaction, where functions can be called with inputs to gather insights on statements.
Using Flask:

This Flask application sets up an API for analyzing statements by gathering news articles related to them and providing insights using a Generative AI model.
 Here's a breakdown of the key components and functionalities:
Flask Setup: You import the necessary modules from Flask to create a web application.
Generative AI Configuration: You configure the Generative AI model by providing an API key and initializing a GenerativeModel object.
Utility Functions:
news_sources: Searches for news articles based on a query and returns a list of URLs.
extract_text_from_url: Extracts text content from a given URL using trafilatura.
textrank_summarize: Generates a summary of the text using TextRank summarization.
extract_keywords: Extracts keywords from text using NLTK.
llm_response: Constructs a prompt for the Generative AI model and generates a response.

API Endpoints:
/insights (POST): Accepts a statement in the request form, gathers news articles related to the statement,
 generates insights using the Generative AI model, and returns the response as JSON.
/status (GET): Returns the status of the process, which can be used for monitoring purposes.
Frontend:
Designed our React components to provide a user-friendly interface for inputting statements and displaying the insights generated by the backend. 





## Conclusion

In conclusion, the development of DiverseLens represents a testament to the power of technology to address pressing societal issues and foster critical thinking in the digital age. By combining machine learning with ethical design principles and user-centered approaches, DiverseLens embodies a holistic solution to the twin challenges of bias detection and fake news prediction.
