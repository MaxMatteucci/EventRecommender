# EventRecommender
# 🎟️ EventRecommender

This repository contains a Google Colab based event recommendation system. It analyzes event data and recommends similar events based on metadata such as genre, location, date, and venue capacity.

---

## 🚀 What This Project Does

The recommender performs the following steps:

- Loads and cleans a CSV of events  
- Builds numeric and encoded categorical features  
- Generates vector representations for each event
- Builds user preferences by asking an array of questions and thus developing a sophisticated recommendation system.
- Computes similarity scores between events.
- Returns the most similar events based on user input. 

You may use any event dataset that includes fields such as event name, genre, city, venue, and date.

---

## 📂 Repository Structure

EventRecommender/  
│  
├── SimilarEvents.ipynb  
├── ProfBuilderAndRecommender.ipynb  
├── tm_indiana_chicago_events_with_capacity.csv  
└── README.md  

---

## 🧑‍💻 How to Use This Project in Google Colab

### 1. Open the Notebook

Upload or open either of the notebooks in Google Colab:

- ProfBuilderAndRecommender.ipynb  
- SimilarEvents.ipynb  

---

### 2. Upload Your CSV File

At the top of the notebook you will see a section instructing you to upload your dataset.

Use this pattern:

    from google.colab import files
    uploaded = files.upload()

Then load your CSV:

    df = pd.read_csv("your_file_name.csv")

Make sure the filename matches the one you uploaded.

---

### 3. Build Features

Run the preprocessing and feature engineering steps. These will:

- Extract date features  
- Encode categorical fields  
- Scale numeric columns  
- Build event vectors  

---

### 4. Generate Recommendations 🎯

Run the recommender function with an event or preference, for example:

    recommend_similar_events("Taylor Swift: The Eras Tour", top_n=5)

This returns the top five similar events based on vector similarity.

---

## 🛠️ Future Improvements

Planned enhancements:

- Embedding based similarity  
- Streamlit or Flask web interface  
- User profile based personalization  
- Referral link monetization  

---

## 📜 License

This project is publicly available for educational use.
