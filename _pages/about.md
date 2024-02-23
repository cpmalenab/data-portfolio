---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Project Portfolio

# [Project 1: Market Demand Analysis for Data Engineering Skills using Data Modeling and Text Mining](https://github.com/cpmalenab/market_demand_analysis_for_DE_skills)

Understanding the labor market demand can (1) help present and future professionals build their portfolio with the most marketable skills, (2) supplement the frameworks of educational institutions and training centers to better prepare students in the digital industry, and (3) give an insight to the general landscape of data engineering industry with the Philippines as the geographical focus.

The figures below shows a high-level view of the data flow to extract the in-demand skill sets from the online job portal as well as the database schema employed in PostgreSQL. The data flow architecture is composed of five layers including: (1) data source, (2) data ingest layer, (3) data warehouse, (4) machine learning, and (5) data visualization.

Summary:
* Scraped over 1000 job descriptions on indeed.com using BeautifulSoup and Selenium.
* Performed data filtering and cleaning using Pandas. 
* Modeled the data in PostgreSQL using psycopg2 and SQLAlchemy libraries.
* Conducted data visualization of geospatial distribution, industry demand, and in-demand hard and soft skills.
* Performed topic modeling using Non-negative Matrix Factorization to extract the most sought after skill set combination.

The findings of the study showed that SQL, Python, and ETL are the leading hard skills and communication, analytical thinking, and leadership are the coveted soft skills in the current market. In addition, knowledge in both data architecture and analytics emerges as the skill combination that would give a competitive advantage to data engineers.

For the full academic paper, please visit this [page](https://github.com/cpmalenab/market_demand_analysis_for_DE_skills/blob/main/final%20paper/Market%20Demand%20Analysis%20for%20Data%20Engineering%20Skills%20using%20Data%20Modeling%20and%20Text%20Mining.pdf).