\# Serverless Clickstream Analytics on AWS



\## Overview

This project demonstrates a serverless clickstream analytics pipeline on AWS using Firehose, S3, and Athena.



\## Goal

Build a low-operations analytics pipeline that can ingest clickstream events, store them cost-effectively in S3, and make them queryable for analytics.



\## Current Scope

\- S3 bucket for raw clickstream events

\- S3 bucket for Athena query results

\- IAM role for Firehose delivery

\- Firehose delivery stream

\- Athena workgroup with enforced settings



\## Planned Next Steps

\- Add API Gateway as the event ingestion layer

\- Add Lambda transformation for event enrichment

\- Add partitioned Athena tables

\- Add QuickSight dashboard layer

\- Add architecture diagram



\## Services Covered

\- Amazon Data Firehose

\- Amazon S3

\- Amazon Athena

\- AWS IAM

\- Amazon API Gateway

\- AWS Lambda

\- Amazon QuickSight



\## What I Learned

\- How to define analytics infrastructure in CloudFormation YAML

\- How to store streaming events in S3 efficiently

\- How to isolate analytics queries with Athena workgroups

\- How to structure an analytics project for GitHub and CV use

