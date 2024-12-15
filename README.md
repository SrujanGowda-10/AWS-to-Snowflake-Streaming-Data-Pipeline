# AWS-to-Snowflake-Streaming-Data-Pipeline

## Introduction
This data pipeline is designed to ingest customer data, transform it, and load it into Snowflake, while maintaining Slowly Changing Dimension (SCD) tables using Snowflake streams. The pipeline leverages AWS services such as Lambda, S3, and Glue to process the data, and Snowpipe and Snowflake procedures to load the data into the Snowflake database.

## Architecture
![SCD Architecture](https://github.com/user-attachments/assets/44ac1bed-caa8-40b4-806b-e55c0e195bd5)

## Snowflake Table Structure
### Stage Table
![image](https://github.com/user-attachments/assets/e2c78f8d-efbe-42f2-aa8d-88bec606a89d)

### SCD1 Table
![image](https://github.com/user-attachments/assets/e3d66456-2e69-4bf0-992b-bc7d139fe22c)

### SCD2 Table
![image](https://github.com/user-attachments/assets/2195007b-4759-4c3e-a1f4-46962152d5d2)


## Tools and Techniques Used
- **Data Source**: AWS Lambda with Python Faker module for generating fake customer data
- **Data Storage**: AWS S3 for raw and transformed data
- **Data Transformation**: AWS Glue with PySpark for data transformation
- **Data Ingestion**: Snowpipe for automatic loading of transformed data into Snowflake
- **Slowly Changing Dimensions**: Snowflake streams and stored procedures for maintaining SCD tables


