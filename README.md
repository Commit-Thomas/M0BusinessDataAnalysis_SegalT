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

1. **Business Question**: Which artists or genres are best suited for live audience recordings, based on historical Spotify data?
2. **Data Collection**: Spotify generates track-level metrics, including `liveness`.
3. **Data Processing**: Data was grouped by year and genre to calculate averages.
4. **Data Analysis**: Using Excel & Python found how strong each genres corralates with Liveness to find which artist should preform recordings live.
5. **Data Visualization/Presentation**: Created charts and tables to show average liveness by year and genre.

---

## 3. 📊 Excel Analysis

### Tasks Performed:
- Imported and cleaned the dataset.
- Filtered rows by year range (1998–2020).
- Created a **pivot table** to show average liveness by year.
- Highlighted a ~0.1 difference in average liveness from highest (0.26) to lowest (0.15).
- Noted a **dip in liveness between 2016–2019**.
- Created a **pivot table** to show average liveness by genre.
- Highlighted a ~0.8 difference in average liveness in genres from highest (0.85) to lowest (0.07).
<img width="745" alt="Screenshot 2025-05-08 at 10 27 45 AM" src="https://github.com/user-attachments/assets/b3a8262f-4391-4a2a-a02b-bb9bca0d9f47" />

---

## 4. 🐍 Python Analysis

### Tasks Performed:
- Loaded CSV using `pandas`.
- Used `groupby()` to compute average liveness by `genre` and by `year`.
- Sorted genres to identify the **Top 5 with highest liveness**:

- 1. Country, latin                           0.853
- 2. World/Traditional, pop                   0.606
- 3. Folk/Acoustic, rock                      0.560
- 4. Pop, easy listening, Dance/Electronic    0.347
- 5. Hip hop, country                         0.274
  
- Used `.dtypes` ` to understand column types.

---

## 5. 🧬 Data Types

### In the dataset (`songs_normalize.csv`):

- **Column Data Types:**
- **artist:**               object
- **song:**                 object
- **duration_ms:**           int64
- **explicit:**               bool
- **year:**                  int64
- **popularity:**            int64
- **danceability:**        float64
- **energy:**              float64
- **key:**                   int64
- **loudness:**            float64
- **mode:**                  int64
- **speechiness:**         float64
- **acousticness:**        float64
- **instrumentalness:**    float64
- **liveness:**            float64
- **valence:**             float64
- **tempo:**               float64
- **genre:**                object

---

## 6. 🧠 Conclusion

1. **Live recordings have decreased slightly in recent years**, with a dip in average liveness from 2016 to 2019.
2. **Genres like Country and Latin are far more live-oriented**, showing much higher liveness scores.
3. **Spotify’s liveness metric is a strong tool** to help record labels decide which artists and genres are best suited for live audience recordings.

---

This is a fictitious scenario
created by the github author for academic purposes only
