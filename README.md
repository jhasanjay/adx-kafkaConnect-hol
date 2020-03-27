# Azure Data Explorer - Kafka Integration Hands On Lab series


## About
The following are instructional hands on labs for Kafka integration with Azure Data Explorer through our KafkaConnect sink.

## Labs
### 1.  Standalone KafkaConnect on HDInsight
Public dataset: <br>
Chicago crimes<br>

Services: <br>
- Azure Storage v2 (peristent store for the raw and curated data), 
- Azure Databricks (download data, stream to Kafka), 
- Azure HDInsight Kafka (not ESP), with edge node running KafkaConnect service
- Azure Data Explorer as sink

[Lab](hdi-standalone-nonesp/README.md)

