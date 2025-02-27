
---

# Airline Price Prediction  

This project predicts airline ticket prices using machine learning techniques. The dataset includes flight details such as airline, source, destination, departure and arrival times, total stops, and price. The model is optimized using hyperparameter tuning for better accuracy.  

## Dataset Description  
The dataset consists of the following columns:  
- **Airline**: The name of the airline  
- **Source**: Departure city  
- **Destination**: Arrival city  
- **Total_Stops**: Number of stops between source and destination  
- **Price**: Ticket price  
- **Journey Date**: Date of travel  
- **Departure Time**: Flight departure time  
- **Arrival Time**: Flight arrival time  

## Data Preprocessing & Feature Engineering  

### 1. Handling Missing Values  
- Checked for null values and dropped rows containing them.  

### 2. Feature Engineering  
- Extracted **day, month, and year** from the journey date.  
- Split **departure and arrival times** into separate hour and minute columns.  
- Computed **duration** as the difference between arrival and departure times.  

### 3. Encoding Categorical Features  
- Applied **one-hot encoding** to categorical columns such as **Airline, Source, and Destination**.  
- Converted ordinal categorical values like **Total_Stops** into numerical format.  

### 4. Feature Selection  
- Used **mutual information regression** to determine feature importance.  
- Retained only relevant features for model training.  

## Model Training  
- Split the dataset into **training and testing sets**.  
- Trained multiple regression models, including:  
  - **Linear Regression**  
  - **Random Forest**  
  - **Decision Tree**  
    
- Evaluated models using **R² score and RMSE**.  

## Hyperparameter Tuning  
- Used **GridSearchCV** and **RandomizedSearchCV** to optimize hyperparameters.  
- Selected the best-performing model for prediction.  

## Results & Performance  
- Compared model accuracy and errors.  
- The optimized model achieved **high accuracy with minimal error**.  

## Future Improvements  
- Experiment with deep learning models.  
- Implement real-time price prediction using web scraping.  
- Enhance feature engineering with additional flight attributes.  

---

