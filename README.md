# Serverless Clickstream Analytics on AWS

## Overview
This project demonstrates a serverless clickstream analytics pipeline on AWS using Firehose, S3, and Athena.

## Goal
Build a low-operations analytics pipeline that can ingest clickstream events, store them cost-effectively in S3, and make them queryable for analytics.

## Current Scope
- S3 bucket for raw clickstream events
- S3 bucket for Athena query results
- IAM role for Firehose delivery
- Firehose delivery stream
- Athena workgroup with enforced settings

## Repository Structure
- `cloudformation/` – CloudFormation templates
- `docs/` – architecture, example queries, and deployment notes

## Planned Next Steps
- Add API Gateway as the ingestion layer
- Add Lambda transformation for event enrichment
- Add Athena table DDL examples
- Add dashboard notes for QuickSight

## Security Notes
- No secrets are stored in this repository
- Environment-specific values are parameterized
- Athena results are written to a controlled S3 location
