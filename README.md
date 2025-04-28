# ⚽ In-Game Win Probability Model

## Project Overview
This project builds a real-time model that predicts the probability of a football match ending in a Home Win, Draw, or Away Win based on evolving match events.  
Inspired by models like FiveThirtyEight’s soccer predictions, it helps visualize match dynamics and key turning points.

The project includes:
- A basic logistic regression model.
- Match event-based feature engineering.
- Real-time probability plots over match duration.
- A framework for future dashboard deployment.

---

## Problem Statement
In football, momentum and key events (like goals or red cards) heavily influence match outcomes.  
The aim is to create a data-driven system that can *quantify* and *visualize* these changing probabilities live during matches.

---

## Data Sources
- **Match Event Data** (example: FiveThirtyEight, Football-Data.org, StatsBomb Open Data)
- Features engineered include:
  - Minute
  - Current score difference
  - Red cards (per team)
  - Possession share
  - Expected goals (xG) differential

---

## Methodology
- **Feature Engineering**: Construct features capturing match state.
- **Model**: Logistic Regression (multi-class classification).
- **Training**: Using match snapshots at different minutes.
- **Evaluation Metrics**:
  - Accuracy
  - Log Loss
  - Classification Report (Precision, Recall, F1-score)

---

## Project Structure
/data/ # Match event datasets (CSV, JSON) 
/notebooks/ # Jupyter Notebooks for feature engineering and model training 
/models/ # Saved models (optional) 
/dashboard/ # Streamlit or Dash app (future work) 
/README.md # Project documentation

---

## Results
The first model achieves reasonable accuracy predicting match outcomes using only basic in-game statistics.  
The probability plots provide a dynamic way to monitor how key events shift a team's chances throughout the match.

**Example Graph:**  
*(Insert a generated probability graph image here once available)*

---

## Future Improvements
- Add live xG accumulation and recent momentum features.
- Incorporate rolling shot counts and dangerous attacks.
- Experiment with tree-based models (RandomForest, XGBoost).
- Build and deploy a live Streamlit dashboard.
- Calibration plots to validate predicted probabilities.

---

## How to Run
1. Clone this repository.
2. Place match data inside `/data/` folder.
3. Open `notebooks/Win_Probability_Model.ipynb`.
4. Run cells to train model and plot results.

---

## Contact
Feel free to reach out for collaborations or questions:

**Name**: [Moritz Philipp Haaf]  
**LinkedIn**: [https://www.linkedin.com/feed/]  
**Email**: [moritz_haaf@outlook.com]

---

# 🚀 Let's Predict the Game, One Minute at a Time!
