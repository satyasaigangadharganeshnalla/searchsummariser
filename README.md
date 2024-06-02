## Wikipedia Scraper and Summarizer

This Python script utilizes the BeautifulSoup library to scrape content from Wikipedia articles and then generates a summary of the scraped text.

## How to Use

1. **Install Required Libraries**: Make sure you have the necessary libraries installed. If not, you can install them using pip:


```py 
pip install beautifulsoup4
pip install lxml
pip install nltk
```

2.  **Run the Script**: Run the Python script. It will prompt you to enter the topic you want to search on Wikipedia.

```py
python main.py
```

3.  **View the Summary**: The script will then scrape the Wikipedia page related to the entered topic, summarize the content, and print the summary.

## Requirements

-   Python 3
-   BeautifulSoup (`bs4`)
-   lxml
-   NLTK (Natural Language Toolkit)

## How it Works

1.  **Scraping Wikipedia**: The script takes user input to search for a topic on Wikipedia. It then fetches the content from the Wikipedia page related to that topic using the `urllib` library.

2.  **Parsing and Formatting**: BeautifulSoup is used to parse the HTML content of the Wikipedia page. The script extracts the text from paragraph tags (`<p>`) and removes any unwanted characters and numbers.

3.  **Summarization**: The script tokenizes the article text into sentences and calculates the frequency of each word. It assigns scores to sentences based on the frequency of the words they contain. The sentences with the highest scores are selected to form the summary.

4.  **Displaying Summary**: The summary, consisting of the top 7 most relevant sentences, is printed to the console.

## Example

If you were to search for the topic "Artificial Intelligence", the script would fetch the Wikipedia page for that topic, summarize its content, and print the summary.