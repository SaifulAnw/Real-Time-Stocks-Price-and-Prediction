# Real-time Data Streaming with Kafka, PostgreSQL, and Stock Price Prediction

The main components of the project include:
### Components:
#### 1. Data Collection
* API Integration: Stock data is collected from Yahoo Finance API for companies like Tesla, IBM, and Apple.
* Data Storage: The data is initially stored in CSV format for batch processing.

#### 2.Kafka Integration
* Kafka Producer: Reads stock data from the CSV file and sends it in batches to a Kafka topic.
* Kafka Consumer: Consumes the stock data from the Kafka topic and stores it in a PostgreSQL database.

#### 3.Database
* PostgreSQL: Stores the consumed stock data for further analysis and real-time processing.

#### 4.Data Processing
* Batch Processing: Utilizes CSV files for batch data processing.
* Real-Time Processing: Uses PostgreSQL for real-time data streaming and processing.

#### 5.Machine Learning
* Prediction Module: Utilizes historical stock data stored in PostgreSQL to predict future stock prices using machine learning models.

### Architecture

![Architecture](https://github.com/SaifulAnw/Real-Time-Stocks-Price-and-Prediction/blob/main/Arcithecture's%20Stock%20Market%20Project.jpg)

### How to Run:

#### Setup Kafka
* Start Kafka and create a topic named what you want, check this [command](https://github.com/SaifulAnw/Real-Time-Stocks-Price-and-Prediction/blob/main/command-kafka.txt)
#### Run the Producer
* Use the getDataMarket.py script to collect data from Yahoo Finance API and store it in a CSV file.
* Run the Kafka Producer to send data from the CSV file to the Kafka topic.
#### Run the Consumer
* Run the Kafka Consumer to consume the data from the Kafka topic and store it in PostgreSQL.
#### Run Machine Learning Predictions
* Use historical data stored in PostgreSQL or use CSV data to make future stock price predictions.



### Dependencies:
#### a. Kafka
#### b. PostgreSQL (Docker)
```bash
docker run --name your_container_name \
  -e POSTGRES_USER=your_user \
  -e POSTGRES_PASSWORD=your_password \
  -e POSTGRES_DB=your_database \
  -p 5435:5432 \
  -d postgres:16
```
#### c. Yahoo Finance API
#### d. Python Libraries:
* pandas
* numpy
* matplotlib
* seaborn
* kafka-python
* psycopg2
* scikit-learn
* yfinance
* json

### Let's try it
Clone the repository
```bash
git clone https://github.com/SaifulAnw/Real-Time-Stocks-Price-and-Prediction.git
```
Navigate to the project directory
```bash
cd Real-Time-Stocks-Price-and-Prediction
```
