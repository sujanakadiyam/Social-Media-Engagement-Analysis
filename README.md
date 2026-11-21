# 📊 Social Media Engagement Analysis
### Python Data Analytics | Data Cleaning | Exploratory Data Analysis | Visualization

A data analytics project focused on cleaning, analyzing, and visualizing social media engagement data using Python to uncover patterns in audience interaction and platform performance.

---

## 🎯 Project Objective

The objective of this project is to analyze social media engagement data by transforming raw, inconsistent data into a structured dataset and extracting meaningful insights through exploratory data analysis and visualization.

The project aims to understand how engagement metrics relate to one another, explore platform-wise engagement patterns, and investigate whether factors such as hashtag count influence engagement rates.

---

## 📌 Project Overview

Social media engagement is influenced by several factors, including platform, content type, reach, likes, comments, shares, and hashtags. Analyzing these factors can help us better understand audience interaction and content performance.

However, real-world datasets may contain missing values, duplicate records, inconsistent categorical entries, invalid numerical values, and formatting issues.

This project follows a complete data analytics workflow, starting from raw dataset exploration and preprocessing to statistical analysis, visualization, insight generation, and recommendations.

The original dataset is preserved, while cleaning and analysis are performed on a separate copy.

---

## 📁 Project Structure

```text
Social-Media-Engagement-Analysis/
│
├── README.md
├── P55_EverCurious.ipynb
├── problem_55_social_media_posts.csv
├── cleaned_dataset.csv
└── .gitignore
```

| File | Description |
|---|---|
| `P55_EverCurious.ipynb` | Jupyter Notebook containing data exploration, preprocessing, analysis, visualizations, and insights. |
| `problem_55_social_media_posts.csv` | Original raw dataset used for analysis. |
| `cleaned_dataset.csv` | Cleaned and processed dataset exported after preprocessing. |
| `README.md` | Project overview, objectives, workflow, insights, and documentation. |
| `.gitignore` | Specifies files Git should ignore. |

---

## 🛠️ Technologies & Libraries

| Technology | Purpose |
|---|---|
| Python | Core programming and analysis |
| NumPy | Numerical operations and invalid value handling |
| Pandas | Data manipulation, cleaning, grouping, and analysis |
| Matplotlib | Plot creation and customization |
| Seaborn | Statistical visualizations |

---

## 🔄 Workflow

### 1. Data Loading & Exploration

- Loaded the CSV dataset using Pandas.
- Created a separate copy to preserve the original data.
- Explored the dataset using `head()`, `shape`, `columns`, `size`, `info()`, and `describe()`.
- Examined data types, statistical summaries, and dataset structure.

### 2. Data Preprocessing

- Converted the `posted_at` column into datetime format.
- Identified invalid negative values in numerical columns.
- Replaced invalid negative values with `NaN`.
- Standardized inconsistent platform names using dictionary mapping.
- Standardized content-type entries to maintain category consistency.

### 3. Data Cleaning

- Identified and removed duplicate records.
- Examined missing-value distribution across columns.
- Handled missing categorical values using mode-based imputation.
- Handled missing numerical values using mean and median imputation.
- Applied platform-wise grouping during imputation to preserve platform-specific patterns.
- Verified missing values after cleaning.

### 4. Exploratory Data Analysis (EDA)

Explored the relationships and distributions of engagement metrics to identify trends, patterns, and observations.

### 5. Data Visualization

Created multiple visualizations to understand engagement data:

- Scatter plot
- Histogram
- Correlation heatmap
- Line plot

### 6. Insight Generation

Interpreted the visualizations, identified patterns, and developed data-driven recommendations.

### 7. Dataset Export

Exported the cleaned data into a separate CSV file using Pandas, keeping the raw dataset unchanged.

---

## 📈 Visualizations & Analysis

### 1. Hashtag Count vs Engagement Rate

**Visualization:** Scatter Plot

Analyzed the relationship between the number of hashtags used and the engagement rate of posts.

**Observations:**
- Engagement rates vary even for posts with similar hashtag counts.
- No clear linear relationship was observed.
- Increasing the number of hashtags does not necessarily result in higher engagement.

### 2. Engagement Rate Distribution

**Visualization:** Histogram

Explored the distribution and frequency of engagement rates.

**Observations:**
- Most posts fall within the lower-to-middle engagement range.
- The frequency of posts decreases as engagement rates increase.
- Only a relatively small number of posts achieve exceptionally high engagement.

### 3. Correlation Between Numerical Variables

**Visualization:** Correlation Heatmap

Examined relationships between likes, comments, shares, reach, hashtags, and engagement rate.

**Observations:**
- Likes and comments showed a strong positive correlation (approximately 0.82).
- Likes and shares showed a strong positive correlation (approximately 0.81).
- Reach was positively related to likes, comments, and shares.
- Hashtag count showed almost no linear correlation with engagement rate.

### 4. Engagement Rate by Platform

**Visualization:** Line Plot

Compared average engagement rates across the social media platforms present in the dataset.

**Observations:**
- LinkedIn recorded the highest average engagement rate (approximately 9.67).
- Instagram followed closely (approximately 9.62).
- X recorded approximately 9.53.
- YouTube recorded approximately 9.24.
- The differences between platform averages were relatively small.

---

## 💡 Key Insights

- **Platform matters, but the differences are small:** LinkedIn and Instagram recorded slightly higher average engagement rates in this dataset.
- **Hashtag quantity is not a guarantee of engagement:** Hashtag count showed almost no linear relationship with engagement rate.
- **Audience interactions are connected:** Likes, comments, and shares showed positive relationships with one another.
- **Reach and engagement are different:** Higher reach does not necessarily guarantee a higher engagement rate.
- **Engagement varies across posts:** Even posts with similar characteristics can receive different levels of engagement.

> These observations are based on the analyzed dataset and should not be treated as universal social media rules.

---

## 📌 Recommendations

- Develop platform-specific content strategies based on observed audience engagement.
- Focus on content relevance and quality rather than simply increasing hashtag count.
- Encourage meaningful audience interaction.
- Evaluate both reach and engagement rate when assessing post performance.
- Use data-driven insights to refine future content strategies.
- Continue monitoring engagement patterns as new data becomes available.

---

## 📂 Dataset Output

The cleaned dataset is exported as:

`cleaned_dataset.csv`

The original dataset is preserved separately as:

`problem_55_social_media_posts.csv`

This makes the cleaned data reusable for further analysis without repeating the preprocessing workflow.

---

## 🧩 Bonus Challenge — Team Name Generation

An additional string manipulation challenge was implemented to combine two strings character by character using Python.

**Concepts explored:**

- `zip()`
- `max()`
- `ljust()`
- String manipulation
- Generator expressions
- `join()`

The solution handles strings of unequal lengths by padding them before combining corresponding characters.

---

## 🚀 Future Improvements

- Analyze engagement trends across days and months.
- Explore the relationship between posting time and engagement.
- Compare content-type performance across platforms.
- Investigate factors associated with high-engagement posts.
- Perform deeper statistical analysis.
- Explore predictive modeling for engagement.
- Build an interactive dashboard for engagement monitoring.

---

## 🏁 Conclusion

This project demonstrates the practical application of Python in data analytics, from handling imperfect raw data to extracting insights through exploratory analysis and visualization.

It emphasizes the importance of data quality, systematic preprocessing, analytical thinking, and communicating findings through visualizations.

Through this process, raw data becomes more than a collection of records—it becomes a source of information that can support better understanding and decision-making.

---

## 👩‍💻 Author

**Sujana Kadiyam**

🎓 B.Tech – Computer Science and Engineering Student

Interested in programming, analytical thinking, understanding how technology works, and learning through practical problem-solving.

- **LinkedIn:** [Connect with me](https://linkedin.com/in/sujana-kadiyam-2a14933b3)
- **GitHub:** [Explore my repositories](https://github.com/sujanakadiyam)

---

*Built as part of a Python & Data Analytics Hackathon — learning through exploration, analysis, and hands-on problem solving.*
