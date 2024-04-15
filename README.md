# Cloud Run Template for Tavily Search Assistant API

A template repository for a Cloud Run for a Tavily Search API, written in Python

**Tavily Search Assistant**
This repository contains a Flask web application that integrates with the Tavily Search API and OpenAI's language model to provide a conversational search assistant. The application allows users to interact with the assistant through a chat interface, where the assistant can perform web searches using the Tavily Search tool and provide relevant responses based on the user's queries.

**Features**
Integration with Tavily Search API for web searching capabilities
Utilization of OpenAI's language model for generating assistant responses
Chat history management to maintain context across multiple user interactions
Flask web server for handling API requests and serving the user interface
Modularized HTML templates for a clean and maintainable frontend structure

**Prerequisites**
Before running the application, ensure that you have the following dependencies installed:
Python (version X.X.X)
Flask (version 3.0.1)
gunicorn (version 21.2.0)
requests (version 2.31.0)
structlog (version 24.1.0)
google-auth (version 2.3.2)
langchain
tiktoken
tavily-python
langchain-openai
langchain_openai
langchain-community
openai
langchainhub

You can install the required Python packages by running the following command:
bash
pip install -r requirements.txt

Getting Started

Clone the repository:
bash
git clone https://github.com/your-username/tavily-search-assistant.git
cd tavily-search-assistant

Set up the necessary environment variables:

OPENAI_API_KEY: Your OpenAI API key
TAVILY_API_KEY: Your Tavily Search API key

Run the Flask application:

bash
python app.py

Access the application in your web browser at http://localhost:8080.

**Usage**
Enter your query or message in the chat interface.
The assistant will process your input and generate a response using the Tavily Search tool and OpenAI's language model.
The chat history will be maintained, allowing the assistant to provide context-aware responses.

**API Endpoints**
POST /api/chat: Accepts a JSON payload with the user's message and returns the assistant's response.

**File Structure**
app.py: The main Flask application file containing the server-side logic.
templates/: Directory containing HTML templates for the user interface.
index.html: The main page template.
main_content.html: The modularized template for the main content section.
utils/: Directory containing utility modules.
logging.py: Logging utility functions.
requirements.txt: File listing the required Python dependencies.

**Contributing**
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
**License**
This project is licensed under the MIT License.

