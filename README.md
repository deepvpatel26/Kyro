# Kyro
This flask based application is as an assessment for the company Kyro_Saas. I tried to find a better dataset for classifing the news articles based on few categories but coudnt
find any state of the art dataset. I then found a BBC news dataset on Kaggle used that to train the model and I used XGboost for training. I have added delete button and 
also have used beautifulsoap for scraping content from Indianexpress.com so only contents of this url will work other urls might work but the prediciton is not at all accurate
due to not having a proper dataset. We can make a better dataset. I took headline, content and descripiton data while scrapping and used it as a content for category prediction.

Tried to throw an exception if an url apart from indianexpress is submitted but couldnt implement it. 

# Indian Express Article Category Prediction

This is a web application that predicts the category of an article from the Indian Express website. It uses machine learning models to classify articles into different categories.

## Installation

1. Clone the repository:
2. Navigate to the project directory:
3. Install the required dependencies by "pip install -r requirements.txt"
4. Set up the database:

- Create a SQLite database file named `predictions.db`.
- Run the following SQL command to create the `predictions` table:

  ```
  CREATE TABLE IF NOT EXISTS predictions (
      id INTEGER PRIMARY KEY AUTOINCREMENT,
      submission_time TIMESTAMP,
      url TEXT,
      category TEXT
  )
  ```

## Usage

1. Start the Flask development server:Set up the database:

- Create a SQLite database file named `predictions.db`.
- Run the following SQL command to create the `predictions` table:

  ```
  CREATE TABLE IF NOT EXISTS predictions (
      id INTEGER PRIMARY KEY AUTOINCREMENT,
      submission_time TIMESTAMP,
      url TEXT,
      category TEXT
  )
  ```

## Usage

1. Start the Flask development server.
2. Access the application in your web browser at `http://localhost:5000`.

3. Submit an article URL from the Indian Express website.
- If the URL is valid and belongs to the Indian Express, the application will predict the category of the article and display it.
- If the URL is invalid or does not belong to the Indian Express, an error message will be displayed.

4. View the submission history:
- Click on the "History" link in the navigation menu to view the submission history.
- The history table displays the submission time, URL, and predicted category for each submitted article.

## Customization
- You can customize the application by modifying the HTML templates in the `templates` directory to change the layout and appearance.
- The machine learning models used for article category prediction are located in the `model.py` file. You can experiment with different models or improve the existing ones.


Thanks to KYRO SAAS for providing this problem statement which enabled me to learn a lot. 

