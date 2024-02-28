---
permalink: /
title: "Portfolio"
author_profile: true
# redirect_from: 
#   - /about/
#   - /about.html
---
# [BoardGameGeek Content-based Recommender Data Pipeline using AWS](https://github.com/cpmalenab/bgg-recommendation-using-aws)

![AWS Data Pipeline](./images/data_pipeline.png){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">AWS Architecture for BGG Recommender Model</figcaption>

The remarkable growth of board gaming industry has created a dynamic landscape where players, ranging from new comers up to board game collectors, are now presented with an array of options for their next gaming adventure. From this growing consumer interest, innovative game designs, and social interaction that board gaming promotes, it is projected that this industry will still further grow in the coming years. With thousands of games released annually, [BoardGameGeek (BGG)](https://boardgamegeek.com/) stands as the definitive hub where players can discover, discuss, and review board games of all genres and complexities. 

The objective of this project is to establish a comprehensive data pipeline spanning from data collection up to dashboard visualization, leveraging the extensive database of BoardGameGeek. Additionally, a recommendation model is developed to identify similar games based on the mechanics and categories on a specific board game. The outlined system architecture emphasizes the use of Amazon Web Services (AWS) to streamline the processing, storage, and retrieval of the dataset utilized in this project.

### Summary

* Utilized the [BoardGameGeek API](https://boardgamegeek.com/wiki/page/BGG_XML_API2) to systematically gather comprehensive data on board games and collect features including statistics, classifications, and rankings. 
* Architected an end-to-end data processing pipeline using **AWS**, orchestrating tasks from initial data ingestion through storage in data lake.
* Conducted an extensive **Exploratory Data Analysis** to identify underlying trends, feature dependencies, and correlations within the dataset, providing invaluable insights for subsequent modeling. 
* Developed a **content-based recommendation model** using Inverse-Document Frequency (IDF) to find similar games based on mechanics and categories of each board game.
* Employed **Tableau** in developing an immersive dashboard that effectively communicates key statistics and personalized recommendations for individual board games.

![Tableau Dashboard](./images/tableau_recommender_dashboard.png){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">Board Game Recommendation Application on Tableau Public</figcaption>

Please check out the BGG recommender dashboard on [Tableau Public](https://public.tableau.com/app/profile/cesar.malenab/viz/BoardGameGeek_2/Dashboard1) and feel free to explore its interactive features!

---

# [The Big One PH](https://github.com/cpmalenab/the-big-one-ph)

"The Big One PH" is an application which explores the potential impacts of a **Magnitude 7.2** earthquake along the Marikina West Valley Fault System. Through *data storytelling*, the audience can better understand the seismic risks associated with living in Metro Manila. Moreover, the application gives emphasis to the accessibility of the population to the healthcare system in a pre and post earthquake scenario. The interactive visualizations of "The Big One PH" raises awareness and promotes proactive measures in the disaster mitigation efforts to safeguard the well-being of the residents of Metro Manila.

### Summary

* Conducted comprehensive **data wrangling** on diverse datasets such as population demographics, healthcare system, and earthquake catalogs, alongside geospatial data including, fault lines, transportation networks, and barangay boundaries.
* Exectuted preprocessing of **geospatial datasets** to ensure accuracy and compatibility, validating and converting data from KML (Key Markup Language) to GeoJson format utilizing tools such as Google Earth and QuantumGIS.
* Applied the **Rational Agent Access Model (RAAM)** from the PySAL library to compute accessibility scores, facilitating insightful analysis of spatial disparities and resource distribution.
* Visualized the datasets using an engaging and interactive **data storytelling** application developed with **Plotly-Dash**, enabling users to intuitively explore key insights derived from the datasets.
* Utilized **HTML and CSS** to design a visually compelling data visualization interface, subsequently deploying the application on **Render**.

![seismicity.png](./images/seismicity.png){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">The Big One PH Data Storytelling Visualization</figcaption>

Feel free to check out "The Big One PH' at [https://the-big-one-ph.onrender.com/](https://the-big-one-ph.onrender.com/). Please note that you may experience longer loading times since the app is hosted only on a free instance of Render.

---

# [Market Demand Analysis for Data Engineering Skills using Data Modeling and Text Mining](https://github.com/cpmalenab/market_demand_analysis_for_DE_skills)

Understanding the labor market demand can (1) help present and future professionals build their portfolio with the most marketable skills, (2) supplement the frameworks of educational institutions and training centers to better prepare students in the digital industry, and (3) give an insight to the general landscape of data engineering industry with the Philippines as the geographical focus.

The figures below shows a high-level view of the data flow to extract the in-demand skill sets from the online job portal as well as the database schema employed in PostgreSQL. The data flow architecture is composed of five layers including: (1) data source, (2) data ingest layer, (3) data warehouse, (4) machine learning, and (5) data visualization.

![data_flow.jpg](./images/data_flow.jpg){: .align-center}
<figcaption style="text-align:center; font-size: smaller;">Data Flow Diagram</figcaption>

### Summary:
* Employed **BeautifulSoup and Selenium** to scrape 1000 job descriptions from indeed.com.
* Utilized **Pandas** for precise data filtering and cleaning, ensuring the integrity and quality of the dataset.
* Implemented relational data modeling in **PostgreSQL** using the **psycopg2** and **SQLAlchemy** libraries, facilitating efficient storage and retrieval of structured information using **SQL**.
* Conducted **data visualization** of key insights including geospatial distribution analysis, industry demand trends, and identification of in-demand hard and soft skills.
* Performed **topic modeling** using Non-negative Matrix Factorization to summarize the collected job descriptions into four skill sets.

![database_schema.png](./images/database_schema.png){: .align-center}
<figcaption style="text-align:center; font-size: smaller;">Database Schema</figcaption>

The findings of the study showed that SQL, Python, and ETL are the leading hard skills and communication, analytical thinking, and leadership are the coveted soft skills in the current market. In addition, knowledge in both data architecture and analytics emerges as the skill combination that would give a competitive advantage to data engineers.

For the full academic paper, please visit this [page](https://nbviewer.org/github/cpmalenab/data-portfolio/blob/master/files/Market%20Demand%20Analysis%20for%20Data%20Engineering%20Skills%20using%20Data%20Modeling%20and%20Text%20Mining.pdf).

---

# [Seismic Hazard Assessment using Monte Carlo Simulation](https://github.com/cpmalenab/seismic_hazard_assessment)

Statistics of significant earthquakes (Mw ≥ 5.0 and distance ≤ 400 km) are established for a building in Metro Manila based on an earthquake catalog in the past 122 years. Seismic hazard assessment utilizing conventional Probabilistic Seismic Hazard Analysis (PSHA) may be validated using the **Monte Carlo Simulation (MCS)** method and this notebook presents a framework for performing MCS in Python for seismic hazard assessments. The seismicity of the project site is determined through *descriptive statistics* of various earthquake parameters which will also serve as input variables for the simulation. This notebook will also highlight common methods, function calls, and visualization tools that are important in statistical studies and random sampling methods.

The following libraries were used in the simulation:

* **Numpy, Scipy, Math** - mainly used to handle statistical models, mathematical computations, and random number generators for the simulation
* **Pandas** - data manipulation and storage of multi-dimensional arrays
* **Folium, Seaborn, Matplotlib** - data visualization of geographical distribution, histograms, probability mass function, and cumulative distribution function of random variables

The United States Geological Survey (USGS) is an agency that monitors natural hazards around the world including earthquakes and the data used in this study were downloaded from their [database](https://earthquake.usgs.gov/earthquakes/).

The figure below shows the effect of varying the number of trials to the smoothness of the curve.

![simulation](./images/simulation.PNG){: .align-center}
<figcaption style="text-align:center; font-size: smaller;">Monte Carlo Simulation results at varying no. of trials</figcaption>

The plot of hazard curves with varying number of years show that at lower probabilities of exceedance (more rare events), the tail end of the graph is not as defined as those with higher probabilities. Thus, a large number of samples is required to obtain more data points at the regions of lower probability.

![hazard_curves](./images/hazard_curves.PNG){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">Spectral acceleration curves produced with 1,000,000 years of simulated earthquake at varying structural periods using Monte Carlo Simulation</figcaption>

To view the full documentation and implementation of the project, please visit this [notebook](https://nbviewer.org/github/cpmalenab/seismic_hazard_assessment/blob/main/Seismic%20Hazard%20Assesment%20using%20Monte%20Carlo%20Simulation.ipynb).
