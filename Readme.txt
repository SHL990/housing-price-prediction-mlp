🏠 Housing Price Prediction using Neural Networks (MLP)
📌 Overview

This project focuses on predicting residential property prices using a Multi-Layer Perceptron (MLP) neural network.
It addresses a real-world regression problem in real estate analytics by leveraging machine learning techniques to model complex relationships between housing features and sale prices.

🎯 Objective

The goal is to predict the SalePrice of houses based on various features such as:

Property size

Construction quality

Location

Structural characteristics

This is formulated as a supervised regression problem with a continuous target variable.

📊 Dataset

Name: Ames Housing Dataset

Source: Kaggle

Samples: 2,930 houses

Features: 81 input variables + 1 target

💰 Target Variable (SalePrice)

Min: $12,789

Max: $755,000

Mean: ~$180,796

Median: $160,000

🔍 Feature Types

Numerical: Lot area, year built, rooms, garage size, etc.

Categorical: Neighborhood, zoning, house style, materials, etc.

⚙️ Data Preprocessing

To ensure optimal model performance, several preprocessing steps were applied:

🧹 Handling Missing Values

Numerical → replaced with median

Categorical → replaced with "None"

🔢 Encoding

Applied One-Hot Encoding to categorical variables

📏 Feature Scaling

Standardized numerical features using StandardScaler

🔀 Data Split

80% Training

20% Testing

🧠 Model Architecture (MLP)

The neural network was implemented using TensorFlow / Keras.

Architecture:

Dense (128 neurons, ReLU)

Dropout (20%)

Dense (64 neurons, ReLU)

Dense (32 neurons, ReLU)

Output Layer (1 neuron, Linear)

⚙️ Training Configuration

Optimizer: Adam

Loss: Mean Squared Error (MSE)

Metric: Mean Absolute Error (MAE)

Epochs: 50

Batch size: 32

📈 Results
✅ Model Performance

Strong convergence during training

No significant overfitting

Stable training and validation loss

📊 Evaluation Metrics

RMSE: Low prediction error

R² Score: High → model explains most variance

📉 Predictions

Predictions closely match actual values

Scatter plot shows alignment along diagonal (good accuracy)

🔍 Example Prediction

The model was tested on unseen data and produced accurate price estimates, demonstrating its practical usability.

🧪 Key Insights

Neural networks effectively capture non-linear relationships

Proper preprocessing is critical

Model generalizes well to unseen data

🚀 Tech Stack

Python

TensorFlow / Keras

Scikit-learn

Pandas / NumPy

Matplotlib / Seaborn

📌 Project Structure
.
├── data/
├── models/
├── notebooks/
├── src/
├── README.md
└── requirements.txt
🔮 Future Improvements

Hyperparameter tuning

Feature selection / dimensionality reduction

Comparison with ensemble models (XGBoost, Random Forest)

📜 License

This project is licensed under the MIT License.

👨‍💻 Author

Souhail Merghich
AI & Data Enthusiast | Computer Science Engineer