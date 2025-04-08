# Would We Have Met? 🤝  
*A Data-Driven Exploration of Human Meeting Potential*

This project explores a unique question using data science: **"Would two people have ever met?"**  
Inspired by dating platforms and real-world coincidences, the notebook simulates the potential of two individuals crossing paths based on **location timelines, age compatibility, shared traits, hobbies, and behavioral attributes**.

---

## 🧠 Project Objective

To build an algorithm that computes a **match score** representing the likelihood of two individuals meeting or having the potential to meet, based on synthetic data and smart heuristics.

---

## 🧩 Core Features

- **City-Time Overlap Logic**: Determines if both individuals lived in the same city at the same time.
- **Age Compatibility Filter**: Applies age tolerance (e.g., ±5 years) to filter reasonable overlaps.
- **Trait-Based Similarity Scoring**: Uses Jaccard similarity on personality traits, hobbies, and social patterns.
- **Match Score Generator**: Combines city-timeline match, age, and behavioral similarity into one score.
- **Query System**: Lets users input their profile and explore who they *almost met* or *could still meet*.

---

## 🔍 Project Structure

| Step | Description |
|------|-------------|
| 1️⃣   | Parse `city_timeline` to find overlapping periods |
| 2️⃣   | Apply `is_age_compatible()` with a tolerance factor |
| 3️⃣   | Calculate `combined_trait_similarity()` using Jaccard method |
| 4️⃣   | Return ranked potential matches with reasoning |

---

## 💾 Sample Data Fields

- `name`, `gender`, `birth_year`
- `city_timeline` – a list of (city, start_year, end_year)
- `traits`, `hobbies`, `character`
- `frequent_places`, `social_platforms`

> 🧪 All data is synthetically generated and anonymized for testing.

---

## 📊 Technologies Used

- Python (Pandas, NumPy)
- Jaccard Similarity
- Interactive logic simulation via Google Colab

---

## 🚀 How to Run

1. [Open the notebook in Google Colab](https://colab.research.google.com/drive/1YC-TPHbseW9VX7NUtxvBF2PIIm2BCN65)
2. Run cells in sequence to simulate pair matching.
3. Modify or add your own profile to test how close you are to meeting others in the dataset.

---

## 💡 Future Additions
- Add real-time location data or Google Maps APIs  
- Integrate personality model scores (MBTI, Big 5, etc.)  
- Build a Streamlit or Dash-based UI for public testing  
- Enable real user opt-in for “Did we almost meet?” queries

---

## 📜 License

This project is open-source under the MIT License.  
Created by **Yeswanth Reddy Jampala** as an experimental exploration in social logic and AI-powered timelines.

---

*If you've ever wondered if you missed someone by just a street, a year, or a hobby — this project is for you.*

