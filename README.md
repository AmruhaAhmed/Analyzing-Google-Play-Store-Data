# 📊 Analyzing Google Play Store Data

I have performed an in-depth analysis of Google Play Store data to understand the factors contributing to an app's success, such as user ratings, number of installs, and category trends. This analysis aims to help developers and businesses optimize their app offerings.

![image](https://github.com/user-attachments/assets/676464ff-8fef-4551-8832-aa9fd70a7a92)


## 📁 Datasets Used

Link to the datasets: [Kaggle - Google Play Store Data](https://www.kaggle.com/datasets/utshabkumarghosh/android-app-market-on-google-play)

I used two datasets from Kaggle related to over 9000 apps from 20+ categories, along with app reviews for this analysis. The datasets are:

- **apps.csv**: Contains 14 columns related to the apps listed on Google Play Store
- **user_reviews.csv**: Contains 5 columns related to the reviews received by each app and the corresponding sentiment

---

### Columns in the Datasets

#### apps.csv
- `Unnamed: 0`
- `App`
- `Category`
- `Rating`
- `Reviews`
- `Size`
- `Installs`
- `Type`
- `Price`
- `Content Rating`
- `Genres`
- `Last Updated`
- `Current Ver`
- `Android Ver`

#### user_reviews.csv
- `App`
- `Translated_Review`
- `Sentiment`
- `Sentiment_Polarity`
- `Sentiment_Subjectivity`

---

## 🏗️ Project Structure

The analysis was performed through the following steps:

1. **Initial Data Exploration**
2. **Data Cleaning**
3. **Feature Engineering**
4. **Descriptive Statistics**
5. **Data Visualization**
6. **Data Analysis**

---

### 1️⃣ Initial Data Exploration
- Loaded the datasets and stored them in pandas dataframes
- Imported necessary libraries

### 2️⃣ Data Cleaning
- Handled missing values in critical columns like Rating and Reviews
- Converted data types for columns like Installs and Price
- Removed punctuation from text-based columns such as Category and Genres
- Removed stopwords from text-based columns such as Translated Reviews

### 3️⃣ Feature Engineering
- Created new columns such as opinion type, average price of apps per category, and average number of reviews per category

### 4️⃣ Descriptive Statistics
- Calculated key performance indicators (KPIs) using measures of central tendency
- Important insights:
  - Most apps are in the "free" category
  - Average rating of apps is 4.17
  - Average size of each app is 20.41 MB
  - Most reviews are positive

### 5️⃣ Data Visualization
- Utilized various graphs using matplotlib, seaborn, and wordcloud libraries
- Key visualizations include:
  - Distribution of ratings
  - Count of categories of apps
  - Content ratings of apps

### 6️⃣ Data Analysis
- Top insights from the visualizations:
  - Majority of apps are in the "family" category, followed by games and tools
  - Finance and lifestyle apps have the highest average prices
  - Art and design, and education categories have the highest average ratings
  - Gaming apps and family apps have the highest average size per category
  - Communication and video player categories have the highest average number of installations
  - Most apps listed are free to use
  - Free apps occupy slightly more size on average compared to paid apps
  - Average number of installations for free apps is far greater than for paid apps
  - Most apps have "everyone" or suitable for all ages rating
  - Tools, education, and entertainment are the most commonly used words to describe app genres
  - Most reviews evoke a positive sentiment and are subjective
  - Common words in app reviews include "good," "game," and "great"

---
