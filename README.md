# Eventism Music | Modern Data Engineering Project

## Introduction

The goal of this project is to stream events generated from a fake music 
streaming service (similar to Spotify) and create a data pipeline that consumes the real-time data. The data coming in would be similar to an event of a user listening to a song, navigating on the website, authenticating. The data would be processed in real-time and stored to the data lake periodically (every two minutes). The hourly batch job will then consume this data, apply transformations, and create the desired tables for our dashboard to generate analytics. 

We will try to analyze metrics like popular songs, active users, user demographics etc.
A data pipeline with Kafka, Spark Streaming, dbt, Docker, Airflow, Terraform, GCP and much more!

### Architecture

<img src="images\Streamify-Architecture.jpg">

## Technology Used
- Programming Language - Python
- Google Cloud Platform (GCP)
1. Google Storage
2. BigQuery
3. Looker Studio
- Apache Kafka
- Terraform (IAAS)
- Docker
- Apache Spark
- Apache Airflow (Orchestration)
- dbt (Transformation)

### Dataset

[Eventsim](https://github.com/Interana/eventsim) is a program that generates event data to replicate page requests for a fake music web site. The results look like real use data, but are totally fake. The docker image is borrowed from [viirya's fork](https://github.com/viirya/eventsim) of it, as the original project has gone without maintenance for a few years now.

Eventsim uses song data from [Million Songs Dataset](http://millionsongdataset.com) to generate events. I have used a [subset](http://millionsongdataset.com/pages/getting-dataset/#subset) of 10000 songs.

## Data Model
<img src="images\data_model.png">

## Dashboard
<img src="images\dashboard.png">

