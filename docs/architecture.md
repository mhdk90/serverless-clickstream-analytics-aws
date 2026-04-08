# Architecture

```mermaid
flowchart LR
  APP[Application / Website] --> FIREHOSE[Amazon Data Firehose]
  FIREHOSE --> RAW[S3 Raw Events Bucket]
  ATHENA[Amazon Athena WorkGroup] --> RAW
  ATHENA --> RESULTS[S3 Query Results Bucket]
  QS[QuickSight - planned] -. reads analytics .-> ATHENA
  API[API Gateway / Lambda - planned] -. ingestion layer .-> FIREHOSE
