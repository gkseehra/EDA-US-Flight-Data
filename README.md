# Flight Delay Prediction

## Overview
This project aims to predict the likelihood of flight delays using machine learning models. The project structure is divided into three main sections: Exploratory Data Analysis (EDA), model training and testing, and a Flask application for real-world application.

## Project Structure
The project comprises the following components:
1. **Exploratory Data Analysis and Data Pre-processing (`1_EDA.ipynb`):** This notebook contains the initial analysis of the flight data and the necessary steps to pre-process the data for modeling.
2. **Model Comparison (`2_TrainAndTest.ipynb`):** This notebook details the comparison of various machine learning models to determine the best performer.
3. **Flask Application (`FlaskApp`):** A web application built using Flask that utilizes the best-performing model (saved as a pickle file) to predict flight delay probabilities.

## How to Run the Project
1. **Data Extraction:**
   - Download the 2022 flight data from [this link](https://www.transtats.bts.gov/DL_SelectFields.aspx?gnoyr_VQ=FGJ&QO_fu146_anzr=b0-gvzr). Ensure you select only the columns specified in the "Check columns" section of the `1_EDA.ipynb` notebook.
   
2. **Run `1_EDA.ipynb`:**
   - This notebook will provide insights through exploratory data analysis and pre-process the data. The cleaned data will be saved as `us-flight-cleaned-data.csv`.

3. **Run `2_TrainAndTest.ipynb`:**
   - This notebook evaluates different models' performance. The best model will be saved as a pickle file.

4. **Set Up the Flask App:**
   - Copy the pickle file of the best-performing model into the `/FlaskApp/app` folder.
   - Navigate to `/FlaskApp/app`.
   - It is recommended to create a virtual environment.
   - Install the required libraries using: `pip install -r requirements.txt`.

5. **Run the Flask App:**
   - Execute `flask run` to start the application.
   - Access the web interface to input flight details and receive delay predictions.

## Tools Used
- Python 3.x
- Jupyter Notebook
- Flask

## Installation
- Clone this repository.
- Follow the "How to Run the Project" instructions above.

## Screenshots

<img width="700" alt="ss_fdp_1" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/47575f92-68fb-4a76-a878-c23b2c8a10d8">

<img width="700" alt="ss_fdp_2" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/6d8f8b96-1ce7-4145-b945-b8b702ea8e0b">

<img width="700" alt="ss_fdp_3" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/bd9aa08d-527a-44fe-9ad0-2282f6ae6067">

## Author
- Gurleen Kaur (gurleenkseehra@gmail.com).
