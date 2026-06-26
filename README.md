#  Gym Attendance Predictor (Logistic Regression)

This project implements a binary classification model using **Logistic Regression** to predict a user's probability of going to the gym based on personal factors (motivation, distance) and external conditions (weather, day of the week).

The core educational value of this project is demonstrating the full ML lifecycle, from data preprocessing (One-Hot Encoding) to model training, evaluation, and, crucially, **visualization of the Sigmoid function** to explain the prediction's probability. This end-to-end implementation showcases mastery of fundamental machine learning principles and their application to a relatable, real-world decision problem.

***

##  Key Features

* **Binary Classification:** Utilizes the **Logistic Regression** algorithm, a cornerstone of classification, to predict a GO (1) or NO-GO (0) outcome. The project specifically focuses on modeling the relationship between input features and the log-odds of gym attendance.
* **Data Preprocessing:** Demonstrates robust data preparation by correctly handling nominal categorical variables (`weather`, `day_of_week`) using **One-Hot Encoding**. This ensures all features are in the numerical format required for the regression model, correctly managing the baseline categories.
* **Interactive Prediction:** Includes a script that facilitates **real-time, interactive user input**. This allows for immediate testing of the trained model with hypothetical scenarios, providing a practical demonstration of its utility.
* **Model Interpretation:** Goes beyond simple prediction by visualizing the relationship between the **Linear Predictor ($\mathbf{z}$)** and the final **Predicted Probability ($\mathbf{P}$)** via the **Sigmoid Curve**. This is a powerful tool for explaining model behavior and demonstrating a deep theoretical understanding of generalized linear models.

***

##  Technology Stack

This project was developed using standard Python data science libraries:

* **Language:** Python
* **Data Manipulation:** Pandas (for data loading and transformation)
* **Machine Learning:** Scikit-learn (for model training and evaluation)
* **Visualization:** Matplotlib (for plotting the Sigmoid curve)

***

## Project Files

* `logistic_gym_prediction.ipynb` — the full notebook, including exploratory output and the Sigmoid visualization
* `logistic_gym_prediction.py` — the same pipeline as a standalone script
* `logistic_gym_prediction.pdf` — exported notebook for quick viewing without running anything
* `gym_decision_dataset.csv` — the dataset used for training and evaluation (500 records)

## Running It

```bash
git clone https://github.com/zain-the-npc/Gym-Prediction-Model-Logistic-Regression-.git
cd Gym-Prediction-Model-Logistic-Regression-
pip install -r requirements.txt
python logistic_gym_prediction.py
```

This trains the model, prints accuracy and a classification report, then launches an interactive prompt where you can enter your own motivation level, distance, weather, and day to get a live prediction.

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

