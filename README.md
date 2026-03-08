# Data Engineering Projects

## Project 1 — Snowflake ELT Pipeline

### Architecture
S3 → Snowpipe → Raw Tables → Streams → Tasks → Clean Tables → Analytics

### Tools Used
- Snowflake (Data Warehouse)
- AWS S3 (Storage)
- AWS SQS (Event Notifications)
- Snowpipe (Auto Ingestion)
- Streams + Tasks (CDC Pipeline)

### Pipeline Flow
1. CSV files land in S3
2. Snowpipe auto-ingests into raw tables
3. Streams detect new rows
4. Tasks transform and load into clean tables
5. Analytics layer answers business questions

### Key Concepts Demonstrated
- ELT pattern (not ETL)
- Change Data Capture (CDC)
- Storage Integration (IAM Role security)
- Automated pipeline with zero manual intervention
