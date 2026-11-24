---
title: "Week 5 Worklog"
date: 2026-11-02
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->

### Week 5 Objectives:

- Understand Cloud Data Lake architectures on Amazon S3 (Medallion Architecture: Bronze/Raw, Silver/Curated, Gold/Analytics)
- Master serverless data cataloging and ETL pipelines using **AWS Glue** (Data Catalog, Crawlers, Glue ETL Jobs)
- Optimize analytical SQL queries using **Amazon Athena** and columnar storage (**Apache Parquet**, partitioning)
- Explore streaming data ingestion with **Amazon Kinesis / Data Firehose** and warehousing with **Amazon Redshift**

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Study Cloud Data Lake & Storage Formats: <br>&emsp; + Multi-zone S3 Data Lake design (`raw/`, `curated/`, `analytics/`) <br>&emsp; + Columnar formats (Apache Parquet / ORC) vs. CSV / JSON and data partitioning | 02/11/2026 | 02/11/2026 | https://cloudjourney.awsfcaj.com/ |
| 2 | - Study AWS Glue & Data Cataloging: <br>&emsp; + AWS Glue Data Catalog (Databases & Tables) & Glue Crawlers <br>&emsp; + AWS Glue ETL Jobs (PySpark & Python Shell) | 03/11/2026 | 03/11/2026 | https://cloudjourney.awsfcaj.com/ |
| 3 | - **Practice (Serverless Batch ETL):** <br>&emsp; + Ingest raw CSV/JSON data into S3 `raw/` <br>&emsp; + Run a Glue Crawler and ETL script to transform data into partitioned Parquet in `curated/` | 04/11/2026 | 04/11/2026 | https://cloudjourney.awsfcaj.com/ |
| 4 | - Study & Practice Amazon Athena: <br>&emsp; + Query S3 tables directly using serverless SQL <br>&emsp; + Benchmark data scanned and query cost between raw CSV and partitioned Parquet | 05/11/2026 | 05/11/2026 | https://cloudjourney.awsfcaj.com/ |
| 5 | - Study Streaming Ingestion & Data Warehousing: <br>&emsp; + Amazon Kinesis Data Streams vs. Amazon Data Firehose <br>&emsp; + Amazon Redshift & Redshift Serverless fundamentals | 06/11/2026 | 06/11/2026 | https://cloudjourney.awsfcaj.com/ |
| 6 | - **Practice (Streaming Pipeline):** <br>&emsp; + Write a Python producer simulating real-time JSON events into Amazon Data Firehose -> S3 <br>&emsp; + Query ingested records in Athena and clean up lab resources | 07/11/2026 | 07/11/2026 | https://cloudjourney.awsfcaj.com/ |

### Week 5 Achievements:

- Built a multi-tier S3 Data Lake and automated schema discovery with AWS Glue Crawlers.
- Converted raw datasets into partitioned Apache Parquet format, significantly reducing Amazon Athena query scan volume and cost.
- Simulated real-time streaming ingestion using a Python data producer paired with Amazon Data Firehose.