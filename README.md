![Netflix Project Screenshot](images/logo.png)

# 🎬 Movie Data Analysis Project (iScale Movies)

This project analyzes a movie dataset (`moviedb.csv`) to explore **trends, popularity, genres, and voting patterns** using Python libraries like **Pandas**, **Matplotlib**, and **Seaborn**.

---

## 🧠 Project Overview

The goal of this project is to:
- Clean and preprocess raw movie data  
- Explore key statistics and distributions  
- Categorize movie ratings into meaningful groups  
- Visualize insights about genres, votes, and popularity  

---

## 🗂️ Dataset Details

The dataset `mymoviedb.csv` contains the following columns:

| Column | Description |
|:--|:--|
| `Release_Date` | Date when the movie was released |
| `Title` | Movie name |
| `Overview` | Brief summary (dropped during cleaning) |
| `Popularity` | Popularity score |
| `Vote_Count` | Total number of votes |
| `Vote_Average` | Average user rating |
| `Original_Language` | Movie language |
| `Genre` | Comma-separated list of genres |
| `Poster_Url` | Poster image link (dropped during cleaning) |

---

## 🧹 Data Cleaning Steps

1. Converted **`Release_Date`** from string to year (integer).
2. Dropped irrelevant columns:  
   - `Overview`, `Original_Language`, `Poster_Url`
3. Handled missing and duplicate values.
4. Split multiple genres into lists and exploded them into individual rows.
5. Categorized movies based on `Vote_Average` quartiles into:
   - `not_popular`, `below_avg`, `average`, `popular`

---

## 📊 Data Visualization & Insights

### Key Questions Explored:
1. **What is the most frequent genre?**  
   → 🎭 *Drama* is the most common genre (~14%).

2. **Which genre has the highest votes?**  
   → *Drama* and *Action* dominate popularity.

3. **Which movie got the highest popularity?**  
   → 🕷️ *Spider-Man: No Way Home* (Action, Adventure, Sci-Fi).

4. **Which movie got the lowest popularity?**  
   → *The United States vs Billie Holiday* and *Threads*.

5. **Which year had the most films?**  
   → 🎞️ *Year 2020* had the highest number of releases.

---

## 📈 Visuals Used
- **Bar charts** for genre and vote category distributions.  
- **Histogram** for number of movies released per year.  
- **Summary tables** for descriptive statistics.

---

## 🧩 Technologies Used

| Tool | Purpose |
|:--|:--|
| **Python 3** | Core programming language |
| **Pandas** | Data cleaning & transformation |
| **NumPy** | Numerical computation |
| **Matplotlib** | Data visualization |
| **Seaborn** | Advanced and aesthetic plotting |

---


---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Movie-Analysis-Project.git
   cd Movie-Analysis-Project

Install dependencies:

pip install pandas numpy matplotlib seaborn


Run the script:

python movies_analysis.py
