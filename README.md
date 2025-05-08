# M0BusinessDataAnalysis_SegalT
# 🎵 Spotify Liveness Analysis (1998–2020)

## 1. 📈 Business Understanding

A record label is evaluating the potential of its newest artists and wants to determine who might be best suited for **live audience recordings**. Using Spotify data from 1998 to 2020, this analysis explores the **"liveness"** metric across years and genres to understand:

- How live performances have trended over time.
- Which genres typically have higher liveness.
- How this data can support artist-to-genre recording decisions.

> **Business Question:**  
> *“Which artists or genres are best suited for live audience recordings, based on historical Spotify data?”*

---

## 2. 🔄 Data Lifecycle

![image](https://github.com/user-attachments/assets/830c8392-d719-462c-8d8e-9bfcbdba1abb)


### How it applies to this project:

1. **Data Creation**: Spotify generates track-level metrics, including `liveness`.
2. **Data Storage**: The dataset is provided in CSV format (`songs_normalize.csv`).
3. **Data Processing**: Data was cleaned and grouped by year and genre to calculate averages.
4. **Data Analysis**: We used Excel for initial exploration and Python for deeper analysis and visualizations.
5. **Data Visualization**: Created charts and tables to show average liveness by year and genre.
6. **Data Archiving/Disposal**: Final results can be exported or shared in reports for stakeholders.

---

## 3. 📊 Excel Analysis

### Tasks Performed:
- Imported and cleaned the dataset.
- Filtered rows by year range (1998–2020).
- Created a **pivot table** to show average liveness by year.
- Highlighted a ~0.1 difference in average liveness from highest (0.26) to lowest (0.15).
- Noted a **dip in liveness between 2016–2019**.


---

## 4. 🐍 Python Analysis

### Tasks Performed:
- Loaded CSV using `pandas`.
- Used `groupby()` to compute average liveness by `genre` and by `year`.
- Sorted genres to identify the **Top 5 with highest liveness**:


  
- Used `.dtypes` and `.info()` to understand column types.
- Could easily adapt this for artist-level recommendations.

---

## 5. 🧬 Data Types

### In the dataset (`songs_normalize.csv`):

-Column Data Types:
-artist               object
-song                 object
-duration_ms           int64
-explicit               bool
-year                  int64
-popularity            int64
-danceability        float64
-energy              float64
-key                   int64
-loudness            float64
-mode                  int64
-speechiness         float64
-acousticness        float64
-instrumentalness    float64
-liveness            float64
-valence             float64
-tempo               float64
-genre                object

---

## 6. 🧠 Conclusion

1. **Live recordings have decreased slightly in recent years**, with a dip in average liveness from 2016 to 2019.
2. **Genres like Country and Latin are far more live-oriented**, showing much higher liveness scores.
3. **Spotify’s liveness metric is a strong tool** to help record labels decide which artists and genres are best suited for live audience recordings.

---

This is a fictitious scenario
created by the github author for academic purposes only
