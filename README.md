# 📱 Google Play Store Data Preprocessing & Analysis

## 🧩 Project Overview
This project focuses on **cleaning, preprocessing, and analyzing** a real-world dataset from the **Google Play Store**.  
The goal was to explore data quality issues, perform thorough data cleaning, and derive meaningful insights through exploratory data analysis (EDA).

---

## 📊 Dataset Description
The dataset contains detailed information about mobile applications published on the Google Play Store, including:

| Column | Description |
|--------|--------------|
| App | Name of the application |
| Category | App category (e.g., Business, Game, Education) |
| Rating | Average user rating |
| Reviews | Number of user reviews |
| Size | Application size (in MB) |
| Installs | Number of user installs |
| Type | Whether the app is Free or Paid |
| Price | Price of the app (if Paid) |
| Content Rating | Age group suitability (e.g., Everyone, Teen) |
| Genres | Genre or subcategory of the app |
| Last Updated | Date when the app was last updated |
| Current Ver | Current version of the app |
| Android Ver | Minimum Android version required |

---

## 🧼 Data Preprocessing Steps
Several preprocessing steps were applied to prepare the dataset for analysis:

1. **Removed duplicate rows and null values**
2. **Cleaned and standardized numeric columns** (e.g., converted `Price` and `Installs` to numeric)
3. **Handled missing and invalid values** in `Rating`, `Size`, and `Android Ver`
4. **Extracted useful features**:
   - Split `Genres` column into `Before_Genres` and `After_Genres`
   - Converted `Size` values (e.g., "14M", "23k") into float MB units
5. **Categorized apps** as *Free* or *Paid*
6. **Converted data types** for analysis compatibility
7. **Created visual summaries** (distributions, correlations, bar charts)

---

## 🔍 Analytical Questions & Insights

After completing the data preprocessing, several analytical questions were explored to extract valuable insights from the cleaned dataset:

1. **What is the most expensive app on the Play Store?**  
   → Found the single highest-priced app among all listings.

2. **Which genre has the highest number of apps?**  
   → Identified the most popular app genre on the platform.

3. **What is the average size of free vs. paid apps?**  
   → Compared app sizes to see if paid apps are generally larger.

4. **What are the top 5 most expensive apps with a perfect rating (5)?**  
   → Analyzed which premium apps also achieved the best user ratings.

5. **How many apps have received more than 50K reviews?**  
   → Calculated the number of highly-reviewed apps.

6. **What is the average price of apps, grouped by genre and number of installs?**  
   → Studied how pricing trends vary with popularity and app category.

7. **How many apps have a rating higher than 4.7, and what is their average price?**  
   → Found the number and cost of top-rated apps.

8. **What is Google’s estimated revenue from apps with 5,000,000+ installs?**  
   → Estimated revenue assuming a 30% commission from app sales.

9. **What are the maximum and minimum sizes of free vs. paid apps?**  
   → Compared size distributions between free and paid applications.

10. **Is there a correlation between an app’s rating, number of reviews, size, and price?**  
    → Used correlation analysis and heatmaps to identify key relationships.

11. **How many apps exist for each type (free/paid) across different content ratings?**  
    → Explored app distribution by content maturity and type.

12. **How many apps are compatible with Android version 4.x?**  
    → Counted apps still supporting older Android versions.

---

These analyses helped uncover patterns in app pricing, size, popularity, and user satisfaction — providing deeper business and technical insights into the Google Play Store ecosystem.


## 📈 Tools & Libraries Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 💡 Key Insights
- Most apps on the Play Store are **free**.  
- **Games** and **Education** dominate the platform by count.  
- Paid apps tend to have **larger sizes** on average.  
- Higher-rated apps generally receive **more installs and reviews**.  
- Google earns significant revenue from top-installed paid apps.  
- Strong correlations were found between **Reviews, Installs, and Ratings**.

---

## 🏁 Conclusion
This project demonstrates the importance of **data preprocessing** as a foundation for reliable analysis.  
By cleaning and transforming the raw data, we were able to uncover insights about app trends, user preferences, and market structure in the Google Play Store.

---
