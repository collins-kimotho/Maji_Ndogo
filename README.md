# Maji Ndogo: From Analysis to Action

### Clustering Data to Unveil Maji Ndogo's Water Crisis

## Project Background and Overview

Maji Ndogo, a region facing a severe water crisis, has compiled a comprehensive database from a nationwide water survey conducted by a dedicated team of engineers, field workers, scientists, and analysts. This database, md_water_services, contains over 60,000 records detailing water sources, visits, quality assessments, and pollution levels across provinces and towns. As a data analyst embedded within the Maji Ndogo water services team, my role was to explore this data to identify access inequalities, operational inefficiencies, and contamination risks.
The primary goals of this analysis were to:

* Assess the distribution and types of water sources to highlight disparities between rural and urban areas.
* Analyze visit patterns and queue times to pinpoint bottlenecks in water access.
* Evaluate water quality and pollution data to detect health risks.
* Develop a prioritized repair and intervention plan to improve commercial and public health outcomes.

This project synthesizes insights from sales trends (e.g., access volumes), product performance (e.g., source types), and regional comparisons to drive actionable improvements in water infrastructure. For technical details on data cleaning, queries, and methodologies, see the Jupyter Notebook or SQL scripts.

## Data Structure Overview
The md_water_services database includes 8 interconnected tables with over 60,000 unique records and 43 columns. Key tables cover employee details, global water access benchmarks, locations, visits, water quality, sources, and well pollution. Below is an Entity Relationship Diagram (ERD)-style overview based on the data dictionary, showing table relationships and key columns. Tables join primarily via IDs like source_id, location_id, and assigned_employee_id, enabling complex queries for insights.

![ERD Diagram](Maji_Ndogo_ERD.png)

his structure is broadly applicable to public health and infrastructure domains, with temporal elements (e.g., dates in visits), demographic info (e.g., provinces, towns), and performance metrics (e.g., people served, queue times). The ERD was created using MySQL Workbench for clarity.

## Executive Summary

Overview of Findings: After a 2.5-year survey period, Maji Ndogo's water access shows stark inequalities, with 60% of sources in rural areas leading to longer queues and higher contamination risks. Key KPIs reveal declines in access efficiency: average queue time is 123 minutes (spiking to 8+ hours at shared taps), 45% of home taps are broken, and many wells exceed safe biological contamination levels (e.g., >0.01 CFU/mL). These issues, compounded by seasonal peaks, indicate a return to pre-intervention inefficiencies but highlight opportunities for targeted fixes.

## Insights Deep Dive
This section breaks down key findings with supporting metrics and visuals, focusing on historical trends and comparisons.

**1. Rural-Urban Divide in Source Distribution:** 60% of water sources are rural, where residents rely heavily on shared taps (43% of population, averaging 2,000 people per tap) or wells (prone to pollution). Urban areas benefit from home taps, but 45% are broken, affecting 31% of the population. Year-over-year, rural access has declined by 15% due to unmaintained infrastructure.

**2. Queue Time Analysis:** Average queue time across shared taps is 123 minutes, with peaks on Saturdays (246 minutes) and during morning/evening hours. This represents a 20% increase from initial survey benchmarks, attributed to overcrowding. 


![queue_time_analysis](queue_time_analysis.png)