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
- `cloudformation/` – CloudFormation YAML templates
- `docs/` – notes and architecture explanations

## Planned Next Steps
- Add API Gateway as the event ingestion layer
- Add Lambda transformation for event enrichment
- Add Athena table DDL examples
- Add architecture diagram
- Add QuickSight notes

## Security Notes
- No secrets are stored in this repository
- Environment-specific values should be passed as parameters
- Query results should be written to a controlled S3 location

## What I Learned
- How to define analytics infrastructure in CloudFormation YAML
- How to store streaming events in S3 efficiently
- How to isolate analytics queries with Athena workgroups
- How to structure an analytics project for GitHub and CV use
