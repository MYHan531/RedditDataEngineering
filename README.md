# Reddit Data Engineering Pipeline

A comprehensive ETL pipeline solution for extracting, transforming, and loading Reddit data into a Redshift data warehouse. This project leverages modern data engineering tools and AWS services to create a robust and scalable data pipeline.

## 🏗️ Architecture

The pipeline consists of the following components:

- **Reddit API**: Primary data source
- **Apache Airflow & Celery**: ETL orchestration and task distribution
- **PostgreSQL**: Temporary storage and metadata management
- **Amazon S3**: Raw data storage
- **AWS Glue**: Data cataloging and ETL jobs
- **Amazon Athena**: SQL-based data transformation
- **Amazon Redshift**: Data warehousing and analytics

![Architecture Diagram](RedditDataEngineering.png)

## 🚀 Features

- Automated data extraction from Reddit API
- Efficient data transformation using AWS services
- Scalable data storage and processing
- Real-time analytics capabilities
- Robust error handling and monitoring

## 📋 Prerequisites

Before you begin, ensure you have:

- AWS Account with permissions for:
  - S3
  - Glue
  - Athena
  - Redshift
- Reddit API credentials
- Docker installed
- Python 3.9 or higher

## 🛠️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/airscholar/RedditDataEngineering.git
   ```

2. **Set up Python environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Configure the application**
   ```bash
   mv config/config.conf.example config/config.conf
   # Edit config.conf with your credentials
   ```

4. **Start the services**
   ```bash
   docker-compose up -d
   ```

5. **Access Airflow UI**
   Open your browser and navigate to: http://localhost:8080

## 📚 Documentation

For detailed documentation about each component and configuration options, please refer to the `docs` directory.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.
