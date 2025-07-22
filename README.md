# House Price Prediction for Nepal

A web application built with **Django** to predict house prices based on key property features using a machine learning model. This project integrates user authentication, prediction history tracking, and leverages **PostgreSQL** as the database backend.

---

## Features

- **User Authentication:**
  - Registration with validation
  - Login and Logout
  - Forgot password functionality with user verification
  - Password reset with confirmation

- **House Price Prediction:**
  - Predict house prices based on features such as number of rooms, bathrooms, floors, area, road width, amenities, city, and road type.
  - Uses a pre-trained Random Forest regression model saved as a pickle file.
  - Input features are scaled before prediction and the output price is transformed back to the original scale.

- **Prediction History:**
  - Each prediction is saved with user info, input features, predicted price, and timestamp.
  - Users can view their past predictions (history).

---
## DATASET USED
https://www.kaggle.com/datasets/sagyamthapa/nepali-housing-price-dataset

Cleaning of data with handling null values was done before experimenting to create a prediction model, the cleaning and null handling however is not shown in node was done in a seperate colab file, but is easy to replicate and can be provided if notified

## Technologies Used

- **Backend:** Django (Python)
- **Database:** PostgreSQL
- **Machine Learning Model:** Random Forest Regressor (pre-trained, loaded via pickle)
- **Frontend:** Django Templates with HTML forms for input and authentication
---

To run this project:-
1. Create and activate a virtual environment:
python -m venv venv
* On Windows:
venv\Scripts\activate
* On macOS/Linux:
source venv/bin/activate

2.pip install -r requirements.txt

3.python manage.py migrate

4.python manage.py runserver
