# Flight Delay Prediction

## Project structure
The project contains 3 main sections:
- Exploratory Data Analysis (1_EDA.ipynb)
- Comparision of performance of different models (2_TrainAndTest.ipynb)
- A flask app that uses the pickled file of the best performing model to predict flight delay possibility. (FlaskApp)

## How to run the project?
- Extract the data (for the year 2022) from the [link](https://www.transtats.bts.gov/DL_SelectFields.aspx?gnoyr_VQ=FGJ&QO_fu146_anzr=b0-gvzr). Extract only the columns shown under "Check columns" markdown of the 1_EDA.ipynb file.
- Run the 1_EDA.ipynb notebook on that dataset. This will give us the exploratory data analysis and data pre-processing.
- In 1_EDA.ipynb we are saving the pre-processed data into an us-flight-cleaned-data.csv. So, we'll use this in our next notebook - 2_TrainAndTest.ipynb.
- Run the 2_TrainAndTest.ipynb to get the performance of different models and their respective pickle files.
- Copy the pickle file of the best performing model and save it in the /FlaskApp/app folder.
- Now, after navigating to /FlaskApp/app folder, first install the libraries mentioned in requirements.txt (creating a virtual environment is advised) using the command: ```pip install -r requirements.txt```.
- Now, run the command ```flask run``` to run the flask app. Now, you can enter the details and predict the possibility of a flight being delayed.

## Screenshots

<img width="700" alt="ss_fdp_1" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/47575f92-68fb-4a76-a878-c23b2c8a10d8">

<img width="700" alt="ss_fdp_2" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/6d8f8b96-1ce7-4145-b945-b8b702ea8e0b">

<img width="700" alt="ss_fdp_3" src="https://github.com/gkseehra/Flight-Delay-Prediction/assets/35463826/bd9aa08d-527a-44fe-9ad0-2282f6ae6067">
