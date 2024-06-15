# Build Fast API in Python using Logistic Regression Classifier on IRIS Data set

**This project provides a FastAPI-based web service for predicting the species of an Iris flower using a Logistic Regression classifier. The prediction is based on the famous Iris dataset.**

### Installation

### Prerequisites

- Python 3
- pip (Python package installer)

### 1. Clone the repository:
    **git clone https://github.com/codeefy/Fast-API-in-Python.git**

### 2.Set up the environment :
      **python -m venv myenv**
     
Run this commnad in vs code terminal 

### 3.Activate the environment 
      **.\myenv\Scripts\activate**

### 4. Install important Dependecies
      **pip3 install fastapi uvicorn**
      **pip3 install scikit-learn**

### 5. Run the FastAPI server:
      **uvicorn main:app --reload**
    **The server will start at `http://127.0.0.1:8000`.**
## Usage

To use the API, send a POST request to the `/predict` endpoint with the sepal and petal measurements of the Iris flower.

### Example using `curl` 
Run this command in command line terminal

      **curl -X POST "http://127.0.0.1:8000/predict/" -H "Content-Type: application/json" -d "{\"sepal_length\": 5.1, \"sepal_width\": 3.5, \"petal_length\": 1.4, \"petal_width\": 0.2}"**
