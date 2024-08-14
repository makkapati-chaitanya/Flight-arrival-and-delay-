# Flight Arrival Delay Prediction

## Overview

This project focuses on predicting flight arrival delays using machine learning techniques. The predictive model is built using Python, Apache Spark, and the DecisionTreeRegressor algorithm, aiming to provide accurate forecasts of flight delays. The project leverages distributed processing with Spark for handling large datasets efficiently and includes a Flask-based web interface for user interactions. The application is deployed on AWS Lambda, ensuring scalability and cost-effective cloud deployment.

## Features

- **Predictive Modeling:**
  - Developed a model using DecisionTreeRegressor to predict flight arrival delays.
  - Trained the model on historical flight data to enhance prediction accuracy.

- **Distributed Processing:**
  - Utilized Apache Spark for distributed data processing and feature engineering.
  - Enhanced efficiency and scalability when working with large datasets.

- **Web Interface:**
  - Built a user-friendly interface using Flask to allow users to input flight details and receive delay predictions.
  - The interface provides real-time predictions based on the trained model.

- **Cloud Deployment:**
  - Deployed the Flask application on AWS Lambda, ensuring scalability and efficient resource utilization.
  - Leveraged AWS services to manage and scale the application as needed.

## Technologies

- **Programming Languages:** Python
- **Frameworks:** Flask
- **Big Data Tools:** Apache Spark
- **Cloud Services:** AWS Lambda

## Installation

To set up and run the Flight Arrival Delay Prediction project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/flight-delay-prediction.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd flight-delay-prediction
   ```

3. **Set up a virtual environment (optional but recommended):**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

4. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

5. **Configure AWS Lambda:**

   - Set up your AWS Lambda environment by configuring your AWS credentials.
   - Deploy the Flask application to AWS Lambda using the provided deployment script or manually via the AWS Management Console.

6. **Run the Application Locally:**

   If you wish to run the application locally:

   ```bash
   python app.py
   ```

   The web interface will be accessible at `http://127.0.0.1:5000/`.

## Usage

1. **Access the Web Interface:**
   - Input the required flight details into the provided fields on the web interface.
   - Click on the "Predict" button to receive a prediction of the expected flight arrival delay.

2. **Interpreting the Results:**
   - The prediction will indicate the estimated delay in minutes.
   - The model’s prediction is based on historical flight data and factors such as departure time, weather conditions, and more.

## Project Structure

```
flight-delay-prediction/
├── app.py                  # Flask application script
├── model/                  # Directory containing the predictive model files
├── templates/              # HTML templates for the Flask interface
├── static/                 # Static files (CSS, JavaScript, images)
├── requirements.txt        # Python dependencies
├── deployment/             # AWS Lambda deployment scripts
└── README.md               # Project documentation
```

## Contributing

Contributions to this project are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.



This README file provides a comprehensive guide for understanding, setting up, and using the Flight Arrival Delay Prediction project, along with details on the technologies used and how to contribute.
