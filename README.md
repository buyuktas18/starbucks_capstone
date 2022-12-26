# Predicting Customer Response to Starbucks Benefits

This project aims to predict whether a customer will respond to a benefit offered by Starbucks, based on historical data.

##  Requirements
To run this project, you will need the following software and libraries:

- Python 3.x
- Pandas
- NumPy
- Scikit-learn

## Data

The data used in this project consists of customer information and whether or not they responded to a benefit offered by Starbucks. We have also some information about the properties of offers. The data is stored in the data/ directory in a CSV file.

Here is the schema and explanation of each variable in the files:

### **portfolio.json**

- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

### **profile.json**

- age (int) - age of the customer
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

### **transcript.json**

- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record


## Project Structure
The project has the following structure:

- **data/:** directory containing the input data
- **notebooks/:** directory containing Jupyter notebooks with code for exploring and preprocessing the data, and for training and evaluating models
- **models/:** directory containing trained models

## Running the Project
To run the project, follow these steps:

- Install the required libraries and software listed in the Requirements section.
Navigate to the notebooks/ directory and open the file Starbucks_Capstone_notebook.ipynb.
Follow the instructions in the file to run the code and see the results.
Results
The results of the project, including evaluation metrics for the trained models, will be printed when you are running notebook cells. You can also observe them by reading the medium blog post related to this topic:

