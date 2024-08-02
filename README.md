# Real-time Data Streaming with Kafka, PostgreSQL, and Stock Price Prediction

The main components of the project include:
### Components
### 1. Data Collection
* API Integration: Stock data is collected from Yahoo Finance API for companies like Tesla, IBM, and Apple.
* Data Storage: The data is initially stored in CSV format for batch processing.

### 2.Kafka Integration
* Kafka Producer: Reads stock data from the CSV file and sends it in batches to a Kafka topic.
* Kafka Consumer: Consumes the stock data from the Kafka topic and stores it in a PostgreSQL database.

### 3.Database
* PostgreSQL: Stores the consumed stock data for further analysis and real-time processing.

### 4.Data Processing
* Batch Processing: Utilizes CSV files for batch data processing.
* Real-Time Processing: Uses PostgreSQL for real-time data streaming and processing.

### 5.Machine Learning
* Prediction Module: Utilizes historical stock data stored in PostgreSQL to predict future stock prices using machine learning models.

### Architecture

![Architecture](https://github.com/SaifulAnw/Real-Time-Stocks-Price-and-Prediction/blob/main/Arcithecture's%20Stock%20Market%20Project.jpg)
