
# News Research ChatBot 

This is a user-friendly news research tool designed for news information retrieval system. Users can input article URLs and ask questions to receive relevant insights from the stock market and financial domain.

## Features >>
- Load URLs or upload text files containing URLs to fetch article content.
- Process article content through LangChain's Unstructured URL Loader.
- Construct an embedding vector using OpenAI's embeddings and leverage FAISS.
- Interact with the LLM's by input queries and receiving answers.

## Installation >>
01. Clone this repository to your local machine using by this given command:
        git clone https://github.com/mflix24/NewsResearchChatBot.git

02. Install the required dependencies using pip:
        pip install -r requirements.txt

03. Setup OpenAI-API-key into .env fileand load API-KEY
        OPENAI_API_KEY=MY_API_KEY

## Usage/Examples
This web-app will open in your browser. On the sidebar, we can input URLs directly.
Initiate the data loading and processing by clicking "Process URLs." button.Observe 
the system as it performs text splitting, generates embedding vectors and efficiently indexes them using FAISS. The embeddings will be stored and indexed by using FAISS.
The FAISS index will be saved in a local file path at pickle format.We are going to 
use the following given web address :
  - https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
  - https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html
  - https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

## Project Structure >>
- main.py : The main Streamlit application script.
- requirements.txt : A list of required Python packages for the project.
- faiss_store_openai.pkl : A pickle file to store the FAISS index.
- .env : Configuration file for storing your OpenAI API key.