Briefly: A Summarized News Portal
Briefly is a web application built using Streamlit that provides summarized news articles from various categories. Users can select trending news, favorite topics, or search for specific topics to get the latest news updates in a brief format.

Features
Trending News: Get the latest trending news articles.
Favorite Topics: Select from a list of categories such as World, Nation, Business, Technology, Entertainment, Sports, Science, and Health.
Search Topic: Search for news articles by entering a specific topic.
Installation
To install and run this application, follow the steps below:

Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/briefly.git
cd briefly
Create a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Download NLTK data:

python
Copy code
import nltk
nltk.download('punkt')
Run the Streamlit application:

bash
Copy code
streamlit run app.py
Usage
After running the Streamlit application, a web page will open in your browser. Follow these steps to use the application:

Select Category: Choose a category from the dropdown menu.
Number of News: Use the slider to select the number of news articles you want to display.
View News: The news articles will be displayed with a brief summary and a link to read more.
Code Overview
Main Components
Fetching News:

fetch_news_search_topic(topic): Fetches news articles based on the search topic.
fetch_top_news(): Fetches the top trending news articles.
fetch_category_news(topic): Fetches news articles from a specific category.
Displaying News:

fetch_news_poster(poster_link): Fetches and displays the news article image.
display_news(list_of_news, news_quantity): Displays the news articles with summaries.
Streamlit Application:

run(): Main function to run the Streamlit application.
Requirements
streamlit
Pillow
beautifulsoup4
urllib3
newspaper3k
nltk
License
This project is licensed under the MIT License.

Acknowledgements
Streamlit
Newspaper3k
BeautifulSoup
