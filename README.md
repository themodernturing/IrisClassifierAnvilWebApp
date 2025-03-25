# Iris Classifier Web App

This repository contains a Jupyter Notebook (`iris-classifier-finished.ipynb`) that trains an Iris classification model using scikit-learn and integrates it with a web application using Anvil.

## Project Description

The notebook trains a k-nearest neighbors (KNN) model to classify Iris flowers based on sepal and petal measurements. The model is then made accessible through an Anvil web app, allowing users to input measurements and receive predictions.

## Technologies Used

* **scikit-learn:** For machine learning (KNN classifier).
* **Anvil:** For building the web application and connecting to the Colab notebook.
* **Jupyter Notebook (Google Colab):** For development and execution.
* **matplotlib:** For plotting data (used during development, not in the final app).
* **joblib:** For saving the trained model.

## Setup and Usage

1.  **Clone this repository:**
    ```bash
    git clone [repository URL]
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Connect to Anvil:**
    * Follow the instructions in the notebook to connect it to your Anvil app using your Uplink key.
4.  **Run the Anvil app:**
    * Run the anvil app from your anvil account.
5.  **Input Measurements:**
    * Use the web app to input sepal and petal measurements.
6.  **Get Prediction:**
    * The app will display the predicted Iris species.

## Notebook Structure

* `iris-classifier-finished.ipynb`: The main notebook containing the model training and Anvil integration code.
* `requirements.txt`: A list of python libraries used.
* `README.md`: This file, providing project information.

## Limitations

* **Model Simplicity:** The KNN model is relatively simple and may not achieve the highest possible accuracy on complex datasets.
* **Data Dependence:** The model's performance is highly dependent on the quality and distribution of the Iris dataset.
* **Colab Runtime Dependence:** The Anvil app requires the Colab notebook to be running continuously to function. If the Colab runtime is interrupted, the app will lose connection.
* **KeyboardInterrupt Error:** When running `anvil.server.wait_forever()` the colab runtime will stay active. If you manually
