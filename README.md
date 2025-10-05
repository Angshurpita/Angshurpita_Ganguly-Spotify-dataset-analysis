Overview
This project presents a data-driven analysis of Spotify’s music catalog to uncover what defines the sound of modern music. Through exploratory data analysis (EDA) and machine learning, it reveals patterns in song characteristics such as energy, danceability, and valence, helping to understand listener preferences and industry trends.
The project segments Spotify’s music database into unique, data-defined "vibes" and translates findings into actionable insights for playlist curation, recommendation systems, and audience engagement strategies.
Dataset
The dataset contains over 100,000 Spotify tracks, with both metadata and quantitative audio features obtained from the Spotify API.
Key Attributes:
Track Metadata: name, artists, release_date
Popularity Metric: popularity (0–100 scale)
Audio Features: acousticness, danceability, energy, instrumentalness, liveness, loudness, speechiness, tempo, valence
Musical Attributes: key, mode, time_signature
Methodology
The workflow followed a structured, four-stage analytical process:
Data Preparation & Cleaning
Removed duplicates and handled missing values.
Engineered additional features such as decade and mood for trend analysis.
Exploratory Data Analysis (EDA)
Explored feature distributions such as popularity, energy, and valence.
Examined correlations and relationships using heatmaps and scatterplots.
Machine Learning: Clustering & Dimensionality Reduction
Applied K-Means clustering to uncover natural groupings within audio features.
Used the Elbow Method to determine the optimal number of clusters.
Reduced dimensionality with PCA for better visualization and interpretation.
Insight Synthesis
Combined analytical and visual findings into strategic insights and recommendations.
Core Visualizations
Mood Map (Energy vs. Valence): Shows how songs distribute across emotional dimensions.
K-Means Cluster Map (PCA Projection): Displays the five "sonic personas" identified by clustering.
Feature Importance Chart: Highlights which audio features most influence song categorization and popularity.
Key Insights and Recommendations
Mainstream Sound = High Energy, Danceable, Modern Pop
Insight: Popular tracks are generally high in energy and loudness, dominated by pop and EDM.
Recommendation: Focus playlisting and promotion efforts around this high-energy core sound.
Vibe-Based Discovery Outperforms Genre Classification
Insight: Clustering revealed five data-driven sonic personas that reflect real listener behavior better than genre labels.
Recommendation: Build AI-driven "vibe discovery" tools to recommend songs by emotional and sonic similarity.
Popularity is Concentrated (Winner-Takes-All)
Insight: Only a small number of tracks gain massive popularity, often those with strong emotional and energetic appeal.
Recommendation: Develop predictive models to identify and invest in potential super-hits early.
Energy and Valence Define Musical Emotion
Insight: These two features effectively map the emotional landscape of songs.
Recommendation: Create an interactive energy-valence grid that lets users generate playlists by selecting a mood zone.
Technical Stack
Language: Python
Data Analysis: pandas, numpy
Visualization: matplotlib, seaborn
Machine Learning: scikit-learn (K-Means, PCA, RandomForest)
Environment: Jupyter Notebook
How to Run
Clone the repository:
git clone [your-repo-link]
Install dependencies:
pip install -r requirements.txt
Launch Jupyter Notebook:
jupyter notebook
Run the project notebook:
Open SpotifyFinal2.ipynb
Ensure spotify_tracks.csv is in the same directory
Execute all cells sequentially
Project Outcomes
Created a quantitative mood map of the Spotify catalog.
Identified five unique sonic personas using clustering analysis.
Delivered data-backed business insights for personalized music discovery and marketing strategies.
Conclusion
This project bridges the gap between data science and music analytics, transforming raw Spotify data into actionable insights. By analyzing the emotional and sonic fingerprints of songs, it demonstrates how data can be used to personalize music experiences and enhance engagement across streaming platforms.
