# AI Music Genre Classifier 

A Machine Learning pipeline designed to automatically predict and categorize the musical genre of a track based purely on its acoustic features. This project was developed to automate playlist curation and track organization for DJing and event management.

##  Project Overview
Sorting thousands of tracks manually is time-consuming. Using data extracted from the Spotify API, this project builds a classification system that analyzes numerical audio features (like Tempo, Danceability, Energy, and Acousticness) to accurately predict whether a track belongs to Electronic, Latin, or Rock genres.

##  Tech Stack & Methodology
* **Language & Libraries:** Python, Scikit-Learn, Pandas, NumPy, Seaborn, Matplotlib.
* **Data Engineering:** * Ingested an open-source Spotify dataset containing over 30,000 tracks.
  * Isolated 3 distinct macro-genres for robust acoustic separation.
  * Standardized data using `StandardScaler` to ensure uniform feature distribution.
* **Algorithms Compared:**
  * **K-Nearest Neighbors (KNN):** Used as a baseline distance-based model.
  * **Random Forest Classifier:** Used as a robust ensemble method to handle complex, non-linear audio relationships.

##  Key Findings & Results
* **Random Forest** outperformed KNN, achieving a stable accuracy of **~78%**.
* **Feature Importance Analysis** revealed that *Tempo (BPM)*, *Danceability*, and *Energy* are the most critical determining factors when an AI distinguishes between Rock, Latin, and Electronic music.

##  How to Run
1. Clone the repository.
2. Install dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`.
3. Run the Jupyter Notebook. The dataset is fetched dynamically via URL, so no local CSV download is required.
