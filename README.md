# 🎬 Exploratory Data Analysis on Netflix Movies and TV Shows

## Overview

This project analyzes the Netflix content library to uncover trends in content types, genres, countries, ratings, and release patterns. The goal is to understand how Netflix has grown its library over time and which content categories dominate the platform.

## Dataset

| Field | Details |
|-------|---------|
| **Source** | [Netflix Movies and TV Shows – Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows) |
| **File** | `netflix_titles.csv` |
| **Rows** | ~8,807 |
| **Columns** | 12 |

### How to Download
1. Visit the Kaggle link above (sign in required)
2. Click **Download** → extract `netflix_titles.csv`
3. Place the file in this project folder

## Steps Performed

### 1. Importing Necessary Libraries

Essential Python libraries were imported:
- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for data visualization

### 2. Loading the Dataset

The dataset was loaded into a Pandas DataFrame. First (`head()`) and last (`tail()`) rows were inspected to understand the structure.

### 3. Checking Dataset Information

- Total rows and columns using `.shape`
- Data types using `.dtypes` and `.info()`
- Missing values using `.isnull().sum()`

### 4. Handling Missing Data

- `director` and `cast` → filled with **'Unknown'**
- `country` → filled with **mode** (most frequent country)
- `date_added` and `rating` → rows dropped (small % of dataset)

### 5. Handling Duplicates & Data Type Conversion

- Duplicate records checked and removed
- `date_added` converted from object to **datetime**
- Extracted `year_added` and `month_added` features
- `duration` split into numeric value + unit (minutes / seasons)

### 6. Statistical Analysis

- Descriptive statistics computed for numerical and categorical columns

## Exploratory Data Analysis

### i) Univariate Analysis

- **Pie Chart:** ~70% Movies vs ~30% TV Shows on Netflix
- **Bar Chart:** USA leads content production; India is second
- **Ratings:** TV-MA (Mature Audience) is the most common rating
- **Year Added:** Content additions surged from 2016 to 2019

### ii) Bivariate Analysis

- **Movie Durations:** Most movies fall between 80–120 minutes; median ~98 min
- **TV Show Seasons:** Majority have only 1 season — short-form content dominance
- **Monthly Pattern:** July and December see the most content additions

### iii) Multivariate Analysis

- **Top Genres:** International Movies and Dramas dominate
- **Genre × Type:** Documentaries skew toward Movies; Anime skews toward TV Shows
- **Release Year Trend:** Content from 2015–2021 dominates the library

## Key Insights & Findings

### 1. Content Type
- **~70% Movies, ~30% TV Shows** on Netflix
- TV show additions grew faster than movies post-2018

### 2. Country & Geography
- **USA** leads content production by a massive margin
- **India** is the second-largest contributor, reflecting Netflix's India push

### 3. Ratings
- **TV-MA** (Mature Audience) dominates — Netflix primarily targets adult viewers

### 4. Timing
- Netflix heavily ramped up additions from **2016–2019**
- **July & December** see the most content additions (summer and holiday peaks)

### 5. Genres
- **International Movies** and **Dramas** are the top two genres
- **Stand-Up Comedy** is a genre where Netflix has heavily invested

## Conclusion

This EDA of the Netflix content dataset reveals that Netflix is a movie-heavy platform with strong US dominance, though global content is growing rapidly. The platform targets mature audiences and strategically adds content around holiday and summer seasons.

---

### 📌 Next Steps
- Perform **content recommendation system** based on genre + country
- Perform **sentiment analysis** on descriptions
- Predict **content type** from metadata using ML classification

---

### 📊 Tools Used

Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

---

### 🔗 References & Credits

Dataset sourced from Kaggle for educational and analytical purposes.

---

### 📬 Connect with Me

If you have any questions or suggestions, feel free to reach out!

- **LinkedIn:** [Your LinkedIn](https://www.linkedin.com/)
- **GitHub:** [Your GitHub](https://github.com/)
- **Email:** your.email@example.com
