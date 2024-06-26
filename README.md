# Briefly: A Summarized News Portal

Briefly is a web application built using Streamlit that provides summarized news articles from various categories. Users can select trending news, favorite topics, or search for specific topics to get the latest news updates in a brief format.

## Features

- **Trending News:** Get the latest trending news articles.
- **Favorite Topics:** Select from a list of categories such as <span style="color:blue">World</span>, <span style="color:green">Nation</span>, Business, Technology, Entertainment, Sports, Science, and Health.
- **Search Topic:** Search for news articles by entering a specific topic.

## Installation

To install and run this application, follow the steps below:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/briefly.git
    cd briefly
    ```

2. **Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Download NLTK data:**
    ```python
    import nltk
    nltk.download('punkt')
    ```

5. **Run the Streamlit application:**
    ```bash
    streamlit run app.py
    ```

## Usage

After running the Streamlit application, a web page will open in your browser. Follow these steps to use the application:

1. **Select Category:** Choose a category from the dropdown menu.
2. **Number of News:** Use the slider to select the number of news articles you want to display.
3. **View News:** The news articles will be displayed with a brief summary and a link to read more.

## Code Overview

### Main Components

- **Fetching News:**
  - `fetch_news_search_topic(topic)`: Fetches news articles based on the search topic.
  - `fetch_top_news()`: Fetches the top trending news articles.
  - `fetch_category_news(topic)`: Fetches news articles from a specific category.

- **Displaying News:**
  - `fetch_news_poster(poster_link)`: Fetches and displays the news article image.
  - `display_news(list_of_news, news_quantity)`: Displays the news articles with summaries.

- **Streamlit Application:**
  - `run()`: Main function to run the Streamlit application.

## Requirements

- streamlit
- Pillow
- beautifulsoup4
- urllib3
- newspaper3k
- nltk

## License

This project is licensed under the MIT License.

## Acknowledgements

- [Streamlit](https://www.streamlit.io/)
- [Newspaper3k](https://newspaper.readthedocs.io/en/latest/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)

