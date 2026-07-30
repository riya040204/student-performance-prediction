Student Performance Prediction
About The Project

This project predicts a student's math exam score based on demographic and academic factors — gender, race/ethnicity group, parental education level, lunch type, test preparation course completion, and their reading/writing scores. It's built on the well-known "Students Performance in Exams" dataset.

The pipeline covers the full ML lifecycle: data ingestion, preprocessing (imputation, encoding, scaling), model selection via cross-validated grid search across multiple regressors, and serving predictions through a Flask web app.

Credit: This project is forked and adapted from KalyanM45/Student-Perfomance-Prediction. I made the following changes to get it running on a current environment and fixed some issues along the way:

Fixed a pandas 3.x compatibility issue in Data_transformation.py (.drop() no longer accepts both columns and axis together)
Retrained the model and preprocessor from scratch using current scikit-learn/CatBoost versions, resolving pickle version-mismatch warnings from the original artifacts
[Add anything else you change — e.g. README rewrite, deployment, UI tweaks]
Built With
Pandas
Numpy
Seaborn
Matplotlib
Scikit-learn
Catboost
Flask
Dill
Getting Started
1. Clone the repository
bash
git clone https://github.com/riya040204/student-performance-prediction.git
cd student-performance-prediction
2. Create a virtual environment
bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # Mac/Linux
3. Install dependencies
bash
pip install -r requirements.txt
4. Run the app
bash
python app.py

Then open http://127.0.0.1:8080 in your browser.

License

Distributed under the MIT License. See LICENSE for more information.

Acknowledgements

Original project by Kalyan Murapaka. This fork adapts and maintains it for a current Python/library environment.
