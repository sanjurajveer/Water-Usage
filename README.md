# Water Usage Prediction using Deep Learning

This project is part of a capstone initiative in collaboration with Connect IOT, focused on predicting water usage in multi-family residential properties using time-series data. The project utilizes advanced data preprocessing techniques and deep learning models to achieve high accuracy in forecasting.

## 🚀 Objective

To build a robust predictive model that can estimate hourly water usage across various units in a residential complex using features like temperature, unit size, time-of-day indicators, and historical consumption patterns.

## 📂 Project Structure

- `capstone_updated_2_part_ml.ipynb`: Jupyter notebook containing the entire pipeline including:
  - Data ingestion and preprocessing
  - Feature engineering (lag features, rolling statistics, time flags)
  - Categorical encoding (label + embeddings)
  - Binary classification to detect zero vs non-zero usage
  - Deep learning regression model for non-zero usage values
  - Evaluation and visualizations

## 🛠️ Technologies Used

- Python (Pandas, NumPy, scikit-learn)
- TensorFlow / Keras
- SMOTE (for class imbalance)
- Label Encoding and Embedding for categorical variables
- Matplotlib, Seaborn for data visualization

## 🧠 Model Workflow

1. **Data Cleaning & Feature Engineering**:
   - Created lag, rolling average, and time decomposition features
   - Encoded categorical variables using embeddings and label encoders

2. **Classification Task**:
   - Trained a binary classifier to predict if water usage = 0 or not
   - SMOTE used to handle class imbalance

3. **Regression Task**:
   - For non-zero predictions, a deep learning model (ANN) was trained to predict the actual water usage amount
   - Performance evaluated using MAE, RMSE, R², MAPE

## 📊 Key Results

- Achieved over **99% accuracy** in the classification task
- Regression model for non-zero usage delivered **low error rates** with robust generalization

## 📈 Future Improvements

- Incorporate weather API integration for real-time forecasting
- Use LSTM or TCN models for improved sequence modeling
- Deploy the model via Flask or FastAPI for real-time inference

## 🤝 Acknowledgements

Special thanks to:
- Connect IOT for real-world data and domain support
- UCD Capstone Program & Faculty Advisors
- Open-source contributors whose tools and libraries made this project possible

---

