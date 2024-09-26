# XRange Analyzer

This project is an application that is GUI-based for displaying currency exchange rates, calculating risk based on volatility, and plotting custom currency baskets. The data is fetched from the MySQL database, the application uses Tkinter for the user interface and Matplotlib for graph plotting. Preprocessing includes filling missing values in the dataset and removing extra spaces.
## Features

- Data Preprocessing: It fills in missing values and removes extra spaces in the dataset automatically.
- Currency exchange rate visualization : Displays the weekly, monthly, or quarterly exchange rate of a chosen currency against a base currency.
- Risk Assessment: The application computes the volatility of a currency and flags it to be "High Risk" or "Low Risk" based on the standard deviation.
- Custom Basket of Currencies: Build a custom basket of currencies, assigning the weights, and then plot its value against a base currency.
- Peak and Low Identify: It features the highest and lowest exchange rates within the period considered.
## Requisites 
- Ensure you have the following dependencies installed:
Python 3.x
- pandas (for data manipulation)
- mysql-connector-python (for MySQL database connectivity)
- matplotlib (for plotting graphs)
- tkinter (for GUI development)
- numpy (for math operations)

## Deployment

To deploy this project run
- Clone the repository - 
git clone https://github.com/your-username/currency-exchange-viewer.git
- Install the required dependencies
pip install pandas mysql-connector-python matplotlib numpy
- Set up the MySQL database as
Create a MySQL database with the name currency_rates.

Create a table called exchange_rates with the following structure:

CREATE TABLE exchange_rates (
    Date DATE,
    Currency1 FLOAT,
    Currency2 FLOAT,
    -- Add columns for other currencies as needed
);

- Open the project folder and run the main.py file:
python main.py

## Usage/Examples

- Select Currency: Choose the currency you want to visualize from the dropdown.
- Select Base Currency: Choose the base currency to compare against.
- Select Year: Choose the year for which you want to visualize the exchange rates.
- Plot Data: Click on "Plot Weekly Data", "Plot Monthly Data", or "Plot Quarterly Data" to visualize the exchange rates.
- Custom Currency Basket: In the "Custom Currency Basket" tab, you can select up to three currencies, assign weights, and plot the basket value against a base currency.
- Risk Level: The app automatically calculates the volatility and indicates if the currency is "High Risk" or "Low Risk".

## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

## Demo

Insert gif or link to demo

## Future Improvements

- Add more currencies to the database and allow dynamic import of new currency data.
- Introduce more complex risk assessments based on additional financial indicators.
- Improve UI and make it more responsive.
