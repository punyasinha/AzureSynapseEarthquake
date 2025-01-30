# AzureSynapseEarthquake
This is a project on Synapse to ingest data using API and transforming it using notebooks and orchestrating the notebooks through synapse pipeline

## Technologies used
Azure Synapse
  Azure Notebooks
  Azure Pipelines
  Apache Spark Pool
  Azure Gen2 Storage

Source data- https://earthquake.usgs.gov/fdsnws/event/1/

Step 1- Data is fetcehd through an API call (in the bronze notebook) and dumped in the bronze layer.
Step 2- Data is read from the bronze layer and saved to the silver layer after some data quality checks/ data cleaning
Step 3- Data is read form the silver layer. Some transformation is applied using installed packages on the spark pool and saved to the gold layer
Step 4- The 3 notebooks are orchestrated through a pipeline


<img width="1023" alt="Screenshot 2025-01-30 at 2 56 11 pm" src="https://github.com/user-attachments/assets/440e0fd1-9f27-4807-9c8f-8d3d3bd9d8bf" />
