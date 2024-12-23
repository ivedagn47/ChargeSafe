# ChargeSafe

# ChargeSafe: Credit Card Fraud Detection Pipeline

## Overview
ChargeSafe is an end-to-end data engineering pipeline built using Microsoft Azure services. The project aims to process and analyze credit card transaction data to uncover actionable insights. It leverages Azure tools for data ingestion, transformation, and storage, providing a robust foundation for detecting anomalies.

## Features
- **Data Ingestion:** Ingest credit card transaction data from various sources.
- **Data Transformation:** Clean and transform raw data using Databricks notebooks.
- **Data Storage:** Store processed data in Azure Synapse Analytics.

---

## Architecture
The project follows a modular architecture:

1. **Azure Data Factory (ADF):**
   - Ingests raw data from Azure Blob Storage.
   - Orchestrates data pipelines to Databricks for transformation.

2. **Azure Databricks:**
   - Performs data cleaning, validation, and transformation.
   - Prepares data for further analysis by correcting data types and deriving new features.

3. **Azure Synapse Analytics:**
   - Stores transformed data in a dedicated SQL pool.
   - Enables querying of structured datasets for insights.

---

## Tools and Technologies
- **Microsoft Azure Services:**
  - Azure Data Factory
  - Azure Databricks
  - Azure Synapse Analytics
  - Azure Blob Storage
- **Programming Languages:**
  - Python (PySpark)
  - SQL

---

## Getting Started

### Prerequisites
- Azure subscription with access to the listed services.
- Dataset: Credit card transaction dataset stored in Azure Blob Storage.

### Setup
1. **Clone Repository:**
   ```bash
   git clone <repository_url>
   cd ChargeSafe
   ```

2. **Azure Configuration:**
   - Set up required Azure resources using the `Azure Resource Manager` templates provided (if applicable).
   - Update connection strings, secrets, and other configurations in the project.

3. **Databricks Notebook Execution:**
   - Import notebooks from the `notebooks/` directory into your Azure Databricks workspace.
   - Run transformation scripts on the ingested data.

4. **Synapse Integration:**
   - Export transformed data to Azure Synapse Analytics using the provided scripts.

---

## Security Measures
- Secrets such as Azure credentials are stored in Azure Key Vault and accessed securely.
- Sensitive information is redacted before analysis to ensure privacy compliance.

---

## Challenges
- Handling large datasets with efficient processing.
- Ensuring accurate data transformation for meaningful insights.
- Maintaining security and compliance with sensitive data.

---

## Future Improvements
- Add machine learning-based fraud detection models.
- Automate anomaly detection using Azure Machine Learning.
- Expand the pipeline to handle streaming transaction data.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.

---

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

---

## Contact
For questions or support, contact [Your Name] at [Your Email Address].

