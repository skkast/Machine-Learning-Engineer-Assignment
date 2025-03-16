Project: DON Concentration Prediction using Hyperspectral Data

Overview

This project focuses on predicting Deoxynivalenol (DON) concentration in
corn samples using hyperspectral data. The pipeline includes
preprocessing, model training, evaluation, and deployment.

Repository Structure

📂 project-directory/ ├── 📄 PranjalKastwar_Assignment.ipynb \# Jupyter
Notebook with complete workflow ├── 📄 README.md \# Project
documentation ├── 📄 requirements.txt \# List of dependencies ├── 📂
src/ │ ├── data_preprocessing.py \# Preprocessing functions │ ├──
model_training.py \# Model selection, training, and evaluation │ ├──
model_inference.py \# Prediction functions ├── 📂 tests/ │ ├──
test_model.py \# Unit tests for model functions ├── 📂 deployment/ │ ├──
app.py \# Flask/FastAPI app for serving predictions │ ├── Dockerfile \#
Docker setup for deployment └── 📂 docs/ \# Additional documentation

Setup Instructions

1\. Install Dependencies

Make sure you have Python installed (recommended: Python 3.9+). Then,
install the required packages:

pip install -r requirements.txt

2\. Running the Jupyter Notebook

If you\'re working in a Jupyter Notebook environment, open and run
PranjalKastwar_Assignment.ipynb.

jupyter notebook PranjalKastwar_Assignment.ipynb

3\. Running Unit Tests

Run the following command to execute tests:

pytest tests/

4\. Running the API (Flask/FastAPI)

To serve the model via an API:

cd deployment python app.py

The API will be available at http://127.0.0.1:5000/ (Flask) or
http://127.0.0.1:8000/ (FastAPI).

5\. Deploying with Docker

To containerize the application:

docker build -t don-prediction . docker run -p 5000:5000 don-prediction

How to Use

Provide new spectral data as input to the API.

The model will return predicted DON concentration values.

Visualize predictions using provided scripts or Jupyter Notebook.

Contact

For any questions or contributions, feel free to open an issue or reach
out!
