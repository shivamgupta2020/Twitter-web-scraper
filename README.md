# Twitter Web-Scraping App
In this repository it was created by using Selenium script that can read the Twitter home page (on your local computer) and fetch the top 5 trending topics under “What’s Happening” section from the homepage. 

## Technologies Used:
1. Selenium: Selenium is a popular tool for automating web browsers. In this project, it is used for web scraping to interact with the Twitter website and extract trending topics.
2. MongoDB: MongoDB is a NoSQL database program. It is used to store the scraped data (trending topics) in a database for persistence.
3. HTML and Jinja: HTML is used to structure the web pages, while Jinja is a templating engine for Python that is used with Flask to generate dynamic HTML content. 
4. Python-Dotenv: Python-Dotenv is a Python library that manages environment variables stored in a .env file. It is used in this project to securely store sensitive information such as credentials.
5. Flask: Flask is a micro web framework written in Python. It is used to build the web application and define routes for handling HTTP requests.

## Features:
1. Web Scraping: Utilizes Selenium and BeautifulSoup for web scraping to extract trending topics from Twitter's homepage.
2. MongoDB Integration: Stores scraped data in a MongoDB database for persistence.
3. Flask Web Interface: Provides a simple web interface for triggering the scraping process and displaying the scraped data.

## Files Included: 
1. Web.py: Flask application script containing routes for triggering the scraping process and displaying scraped data.
2. twitter_scrapping.py: Python script for scraping Twitter's homepage and storing trending topics in MongoDB.
3. requirements.txt: File containing a list of Python dependencies required for running the project.
4. index.html: HTML template file for rendering the web interface.
5. .env: Environment variable file containing sensitive information like credentials.

### Installation
Clone the repository to your local machine:

```bash
git clone https://github.com/shivamgupta2020/Twitter-Web-Scraping.git
```
Navigate to the project directory:

```bash
cd twitter-scraping-app
```
Install the required dependencies using pip:

```bash
pip install -r requirements.txt
```
Set up your environment variables by creating a .env file in the project directory and adding the necessary credentials:

```makefile
proxymesh_user=your_proxymesh_username
proxymesh_pass=your_proxymesh_password
X_EMAIL=your_twitter_email
X_PASS=your_twitter_password
X_USER=your_twitter_username
MONGODB_URI=your_mongodb_uri
```
Usage
Run the Flask application:

```bash
python Web.py
```
Open your web browser and go to http://localhost:5000 to access the web interface.

Click the "Scrape Data" button to trigger the scraping process.

Once the scraping is complete, the trending topics will be displayed on the webpage.

## Live Hosted
![Project picture](./image/image.png)
