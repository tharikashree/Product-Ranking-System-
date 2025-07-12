
Product Scraper & Ranking System

A lightweight, modular system to scrape, analyze, and rank e-commerce products based on a user's search query — using keyword relevance, price filtering, ratings, and visibility scoring.


---

📁 Project Structure

product-kpi-system/
├── product_scraper.ipynb       # Scraper to collect product data
├── shopping_results.json    # Product data (JSON list)
├── product_ranking.ipynb    # Jupyter Notebook to rank products by query
├── README.md                


---

🔎 1. Product Scraper

> Goal: Collect product data from a target e-commerce search page (e.g., Google Shopping, Amazon, Flipkart)


Functionality:

Scrapes:

Product title

Price

Rating (if available)

Image URL

Product URL

Source domain (brand)


Outputs: shopping_results.json file


Tech Used:

requests, BeautifulSoup


---

2. Product Ranking System

> Goal: Rank products by relevance to a user’s natural language query like:

"navy blue cotton bedsheets under 1500"



Features:

Parses query to extract:

Color keywords (e.g., "navy blue", "light blue")

Price cap (e.g., "under 1500")


Scores products based on:

Title keyword/phrase match

Price filter

Brand boost (Amazon, Flipkart, etc.)

Ratings (if available)


Sorts and displays top results with:

✅ Title

💰 Price

⭐ Rating

🖼️ Image

🔗 Link



How to Run

1. Open product_ranking.ipynb


2. Upload shopping_results.json


3. Enter a search query in the input box


4. View top ranked products (in scrollable HTML view)




---

Privacy and Performance

No cookies or trackers

Works fully on frontend/Colab without external services

No user data stored



---

Dependencies

Install the minimal requirements:

pip install pandas ipywidgets

If using scraping:

pip install beautifulsoup4 requests


Example Queries

light blue cotton bedsheets under 1500

navy king size cotton bedsheet under 1000

white double bed sheet under 1200 with high rating

