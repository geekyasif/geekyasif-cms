# News Sentiment Analysis Web Application  

This file outlines the steps to set up and run the project.  

## Research & Decision  
Before starting, I conducted research to determine whether a backend was necessary. If a backend was required, I considered whether to use Node.js or Python. Alternatively, I explored the possibility of building the project solely with React.js and TensorFlow.js or other sentiment analysis libraries like `sentiment` and `natural`. While it is possible to build only the frontend using React.js, the challenge arises when dealing with large amounts of data and complex computations. In such cases, the browser may struggle to handle these operations efficiently, leading to performance issues. Ultimately, I chose Python over Node.js because Node.js is not as efficient for web scraping and handling large datasets.  

## Tech Stack  
**Frontend:** React.js, Tailwind CSS, Axios, Ant Design (Search Input & Table component)  
**Backend:** Python - Flask (For building the backend API), Spacy, TextBlob (For sentiment analysis), BeautifulSoup (For web scraping), News API (Facing some issues while using Bing Search API)  

## Backend Setup  
Clone the repository using `git clone https://github.com/geekyasif/sentiment-analysis-backend-task.git`. Install Python 3 if not already installed. Create a virtual environment using `python3 -m venv .venv` and activate it. Install dependencies using `pip install -r requirements.txt`. Create a `.env` file and set the following environment variables:  


Run the project using `flask --app main.py --debug run`, and it will be available at `http://localhost:5000`.  

## Folder Structure  
`main.py` contains the API endpoints. The `services` folder contains `fetch_news.py`, which fetches news from the News API, but since this API does not contain enough content for sentiment analysis, I scrape the data using BeautifulSoup. `analyse_sentiment.py` analyzes the content and categorizes it into Positive, Negative, and Neutral. The `config` folder exposes environment variables like API endpoints.  

## Frontend Setup  
Clone the repository using `git clone https://github.com/geekyasif/sentiment-analysis-frontened-task.git`. Install dependencies using `npm i`. Set the environment variables in the `.env` file:  


Run the project using `npm start`.  

## Demo  
Watch the demo video at [this link](https://drive.google.com/file/d/1GdbXg8LzUgYDrWNQAxcW1fsNrUvgAVLr/view?usp=drive_link).  
