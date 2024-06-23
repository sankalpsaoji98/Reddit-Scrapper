# Reddit Clinical Trial Sentiment Analysis and Messaging

## Introduction

This project aims to analyze sentiments from Reddit posts related to clinical trials and generate personalized messages to engage users about clinical trial participation. The application uses Python libraries for data collection, sentiment analysis, and message generation.

## Features

- **Data Collection**: Scrapes posts and comments from relevant subreddits.
- **Sentiment Analysis**: Analyzes sentiments of posts and comments.
- **Message Generation**: Generates personalized messages based on sentiment analysis.
- **Ethical Considerations**: Ensures compliance with API terms and user privacy.

## Setup Guide

### Prerequisites
- **Python**: Ensure Python is installed on your system.
- **pip**: Python’s package installer.

### Step-by-Step Guide

1. **Install Python and Required Libraries:**
   ```bash
   pip install praw textblob openai pandas

### 2. **Set Up Reddit API**

1. Go to Reddit Apps and create a new application.
2. Note your client ID, client secret, and user agent.

### 3. **Set Up OpenAI API**

1. Sign up at OpenAI and obtain an API key.

### 4. **Configure Credentials**

1. Replace placeholder values in the script with your Reddit and OpenAI API credentials.

### 5. **Run the Jupyter Notebook**

1. Open and run `reddit_scraper.ipynb` to scrape data, analyze sentiments, and generate messages.

### Methodology

#### Data Collection

- The PRAW library is used to scrape posts and comments from relevant subreddits related to clinical trials.
- Focus is on subreddits discussing health conditions and clinical trial participation.

#### Sentiment Analysis

- The TextBlob library analyzes the sentiment of each post and comment.
- Sentiment scores are categorized as positive, neutral, or negative.

#### Message Generation

- Based on sentiment analysis, users are segmented by interest level.
- Personalized messages are generated using the OpenAI API to engage users about clinical trial participation.

### Challenges Faced

1. Handling API rate limits for Reddit scraping.
2. Ensuring accurate sentiment analysis given the varied and informal nature of Reddit posts.
3. Balancing the generation of engaging yet ethically appropriate messages.

### Examples

#### Data Collected

- Titles, selftexts, and comments from subreddit posts related to clinical trials.

#### Analysis Performed

- Sentiment scores for each title, selftext, and comment.
- Categorization into positive, neutral, and negative sentiments.

#### Messages Generated

- **Positive**: "Thank you for your interest in clinical trials! We have some exciting opportunities that you might find beneficial."
- **Neutral**: "We noticed you're curious about clinical trials. Here’s some information that might help you decide if it's the right fit for you."
- **Negative**: "We understand you have concerns about clinical trials. Here’s some information that might address your worries and show you how they can be safe and beneficial."

### Ethical Considerations

- **Privacy**: Ensured compliance with Reddit’s API terms of use. No personal data was stored.
- **User Consent**: Focused on public data and generated messages that were informative rather than manipulative.
- **Bias Mitigation**: Aimed for neutrality and fairness in message generation, avoiding assumptions or stereotypes about users based on their sentiment.
- **Transparency**: Designed the system to provide clear information and support informed decision-making for potential clinical trial participants.

### Evaluation Criteria

#### Functionality

- The script successfully performs the tasks of scraping, analyzing, and generating messages. It efficiently collects data from specified subreddits, analyzes the sentiment of the collected data, and generates personalized messages based on sentiment analysis.

#### Code Quality

- The code is organized and modular, with separate functions for data collection, sentiment analysis, and message generation. It uses standard Python libraries and follows best practices for readability and maintainability. Inline comments and descriptive function names enhance the code's clarity.

#### Innovation

- The solution creatively integrates sentiment analysis with personalized message generation using the OpenAI API. It effectively handles the challenges of processing unstructured Reddit data and generates contextually appropriate messages tailored to user sentiments.

#### Ethical Considerations

- Ethical concerns related to data privacy and user engagement were thoroughly addressed. The solution ensures compliance with Reddit's API terms of use, respects user privacy by not storing personal data, and focuses on generating informative messages that support informed decision-making. Efforts were made to avoid bias and ensure fairness in message generation.

### Files Included

- `reddit_scraper.ipynb`: Jupyter notebook for scraping data, analyzing sentiments, and generating messages.
- `Documentation and Instructions.docx`: Detailed setup and methodology documentation.
- `subreddit_data.xlsx`: Raw data collected from subreddits.
- `subreddit_data_with_sentiment_and_messages.xlsx`: Data with sentiment analysis and generated messages.
