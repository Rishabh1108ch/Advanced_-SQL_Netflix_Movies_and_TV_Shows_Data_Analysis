# 🎬 Advanced SQL Project — Netflix Data Analysis (15 Business Problems)

> End-to-end SQL project analyzing **Netflix titles, ratings, categories, user behavior, popularity, content trends**, and business metrics.  
> Solves **15 real-world business questions** using advanced SQL: CTEs, window functions, aggregations, date functions, and subqueries.

---

## 📘 About This Project

This SQL project analyzes Netflix’s content catalog to extract valuable business insights such as audience trends, genre performance, global reach, actor collaborations, rating distribution, and content growth over time.

It demonstrates **advanced SQL analytics** and replicates the kind of reporting used by streaming platforms like Netflix to support content strategy, marketing, and user engagement.

---

## 🎯 Objectives of Netflix Analysis

Netflix leadership, content strategists, and marketing teams need insights to:

- Identify best-performing genres and regions  
- Understand audience preferences  
- Improve content acquisition decisions  
- Detect trends in movies vs TV shows  
- Optimize platform engagement  
- Support data-driven decision-making

This project solves **15 major business problems** using SQL.

---

## 🗂 Dataset Overview

Netflix dataset includes information such as:

- `show_id`
- `title`
- `type` (Movie/TV Show)
- `director`
- `cast`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `genre/listed_in`
- `description`

**Tables Used (Typical Netflix schema):**
- `netflix_titles`  
- (Optional) `ratings`, `countries`, `actors`, `genre_bridge`, etc.  

**Size:** 8,800+ records  
**Columns:** 12 attributes per title  

---

## 🧭 Business Problems / Tasks (15)

1. **Count the number of Movies vs TV Shows on Netflix.**  
2. **Find the most common rating for Movies and TV Shows.**  
3. **Identify the oldest TV show or movie in the dataset.**  
4. **List all titles released in a specific year (e.g., 2020).**  
5. **Top 10 countries with the most Netflix titles.**  
6. **Find titles added in the last 5 years.**  
7. **Find the most frequent genre categories.**  
8. **List all titles featuring a specific actor (e.g., Robert De Niro).**  
9. **Find the director with the highest number of titles.**  
10. **Identify multi-country co-produced content.**  
11. **Count titles added per year to analyze content growth.**  
12. **Top actors appearing together in multiple titles.**  
13. **Find the average duration of Movies & TV Shows.**  
14. **Identify countries producing the highest number of documentaries.**  
15. **List content suitable for kids (G, PG, TV-Y, TV-G, etc.)**

---

## 🧠 SQL Techniques Used

- **Window Functions:**  
  `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `OVER()`

- **Aggregations:**  
  `COUNT()`, `SUM()`, `AVG()`, `MAX()`, `MIN()`

- **String Functions:**  
  `LIKE`, `CHARINDEX`, `SPLIT`, `TRIM`

- **Date Functions:**  
  `YEAR()`, `DATEADD()`, `DATEDIFF()`

- **CTEs:**  
  Used to structure complex analytics

- **Subqueries & Derived Tables**

---
## 📊 Key Business Insights

### 📈 1. Content Distribution
- Movies dominate the platform compared to TV shows.  
- Content availability is strongly influenced by major producing countries like the **US, India, UK, and Canada**.

---

### 🎭 2. Genre Popularity
- Top genres include **Dramas, International Movies, Stand-Up Comedy, and Kids' Content**.  
- Documentary content has shown **steady growth** in recent years.

---

### 🎥 3. Actors with Most Appearances
- Several actors appear repeatedly across Netflix-exclusive titles, indicating **long-term collaborations and partnerships**.

---

### 🌍 4. Regional Content Trends
- Netflix adds more **international content** each year.  
- Co-produced titles are increasing, supporting **global expansion and distribution**.

---

### 🕒 5. Content Growth Over Time
- Rapid content growth occurred between **2015–2020**, reflecting Netflix’s global expansion.  
- Annual title additions demonstrate continuous **platform diversification and scale**.

---

### 👨‍👩‍👧 6. Kids & Family Content
- A significant portion of titles are **family-friendly**, aligning with Netflix’s strategy to support **multi-user households**.

---

## 🛠 Tools & Environment
- **DBMS:** Microsoft SQL Server  
- **IDE:** SSMS (SQL Server Management Studio)  
- **Dataset:** Netflix Titles CSV dataset  


## 🧾 Sample SQL Solutions (From Uploaded File)

### 1) Movies vs TV Shows Count
```sql
SELECT type, COUNT(*) AS total_titles
FROM netflix_titles
GROUP BY type;





