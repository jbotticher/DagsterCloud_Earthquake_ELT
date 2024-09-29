# Data Engineering Camp Capstone Project

## **Earthquakes ELT**
Author: _Joshua Botticher_

## Objective:
The objective of this project is to create a real-time monitoring system that visualizes earthquake data, and dashboards using historical data from the USGS Earthquake API for public use.

## Consumers:
- Researchers: They use the data for analyzing seismic activity patterns and predicting future events.
- Students: They need access to earthquake data for educational projects and learning purposes.
- Educators: They require the data to teach seismic activity and its impacts.
- General Public: They seek to understand earthquake risks and safety measures.

## Questions I Want To Answer:
1) What are the most recent earthquakes and their magnitudes?
2) Which regions are experiencing the highest frequency of earthquakes?
3) What are the patterns and trends in seismic activity over the past year?
4) Which areas are most at risk based on historical data?


| `Source Name`  | `Source Type` | `Source Docs`                               | `Endpoint` |
| -------------  | ------------- | ------------                                | -----------|
|  USGS Earthquake Catalog    | rest api      | https://earthquake.usgs.gov/fdsnws/event/1/ | https://earthquake.usgs.gov/fdsnws/event/1/query|


## Architecture:
![architecture_earthquakes drawio-2](https://github.com/user-attachments/assets/30416493-e6cd-4531-9c23-70e9d336245e)

##Instructions:

1) Clone this repo.
2) Deploy Airbyte on an AWS EC2 Instance. Airbyte deployment docs: https://docs.airbyte.com/deploying-airbyte/on-aws-ec2
3) Create a Dagster cloud account and connect your Github repo to Dagster. Dagster cloud deployment docs: https://docs.dagster.io/deployment/open-source.
4) Update environment variable in Dagster and Snowflake login info (dbt_earthquake->profiles.yml).
