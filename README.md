# Iris Flower Classifier with Flask

This project features a machine learning model that classifies Iris flowers using a Flask web application. The classifier can predict whether a flower is **Iris Setosa**, **Iris Versicolor**, or **Iris Virginica** based on its measurements.

## Features

- **Machine Learning Model**: Classifies Iris flowers using an SVM model trained on the Iris dataset.
- **Flask Web Application**: Provides a user-friendly interface to input flower measurements and obtain predictions.

## Technologies Used

- **Machine Learning**: Scikit-learn
- **Web Framework**: Flask
- **Python**: 3.x
- **HTML/CSS**: For the web interface

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/rudrapatel001/Iris_Flower_Classifier_Ml_Model.git
   cd iris-flower-classifier
   ```

2. **Create a Virtual Environment:**
   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment:**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies:**
   Create a `requirements.txt` file with the following content:
   ```
   Flask
   scikit-learn
   pandas
   numpy
   ```
   Then install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Train the Model:**

   Ensure you have the Iris dataset file (`iris.data`) in the project directory. Run the `iris.py` script to train the model and save it as `iri.pkl`.

   ```bash
   python iris.py
   ```

2. **Run the Flask App:**

   Start the Flask application by running `app.py`:
   ```bash
   python app.py
   ```

   Access the web application at `http://127.0.0.1:5000/home`.

3. **Interact with the Web Interface:**

   - **Home Page**: Go to `http://127.0.0.1:5000/` to access the input form.
   - **Prediction Page**: Submit flower measurements on the home page to get predictions on the next page.

## Code Overview

- `iris.py`: Trains an SVM model on the Iris dataset and saves it as `iri.pkl`.
- `app.py`: The main Flask application file that handles predictions and rendering the web interface.
- `basics.py`: A basic Flask application file that serves the home page. You might not need this if `app.py` is handling everything.

## Files

- `iris.py`: Script to train and save the machine learning model.
- `app.py`: Flask application for serving predictions.
- `basics.py`: (Optional) Basic Flask setup file.
- `home.html`: HTML template for the input form.
- `after.html`: HTML template to display predictions.
- `iri.pkl`: Serialized machine learning model.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request. For significant changes, please open an issue to discuss your changes before proceeding.

## Acknowledgements

- Iris dataset from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris).
- Scikit-learn for the machine learning framework.
- Flask for the web framework.

---

Feel free to adjust any details as necessary!
