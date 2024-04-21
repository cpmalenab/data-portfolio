---
permalink: /
title: "Portfolio"
author_profile: true
# redirect_from: 
#   - /about/
#   - /about.html
---
# [Prediction of Fire Resistance of FRP-strengthened Concrete Beams using Machine Learning Techniques](https://github.com/cpmalenab/fire-resistance)

![Grenfell Fire](./images/grenfell_fire.png)

Structural retrofitting of concrete buildings is necessitated by building aging, changes in occupancy, structural code updates, seismic events, and construction errors, with various techniques such as concrete jacketing, steel plate bonding, and Fiber Reinforced Polymer (FRP) application being utilized. FRP stands out due to its quick installation, lightweight nature, durability, and adaptability, but it suffers from diminished performance at *elevated temperatures* and potential adhesion failure. **Fire resistance** is defined as the duration for which a structural member sustains the applied loading under fire exposure. Assessing the fire resistance (in minutes) of FRP-strengthened concrete beams involve prescriptive codes, experimental tests, and numerical simulations, with challenges including cost and practicality. While experimental studies show enhanced capacities with insulation, full-scale tests are expensive, and numerical analysis requires specialized training and resources. Balancing cost, practicality, and accuracy is essential in selecting the most suitable fire resistance evaluation method.

Existing methodologies for determining the fire performance of FRP-strengthened concrete beams are often oversimplified and impractical, necessitating a more pragmatic approach such as the integration of machine learning (ML) algorithms and artificial intelligence (AI) in Fire Engineering and Sciences (FES). The key goals of incorporating ML and AI in FES include creating advanced fire assessment tools, enhancing knowledge-based methods, and utilizing computational power to tackle complex FES problems. This study aims to develop ML models capable of capturing the nonlinear characteristics involved in assessing beam fire resistance, with the intention of providing fire engineers with a complementary tool and exploring its potential for industry adoption.

## Summary

* Conducted feature engineering and exploratory data analysis to prepare the dataset for optimal utilization by machine learning models.
* Utilized **Scikit-learn** to evaluate candidate machine learning models, including Linear Regression with ElasticNet, Support Vector Regressor, Random Forest, and XGBoost, using diverse performance metrics (R^2, RMSE, MAE) for assessment.
* Employed **PyTorch** to design and train a five-layer Deep Neural Network with ReLU activation function and Adam optimizer, following a systematic evaluation of architecture over multiple iterations.
* Determined feature importance across all models using **SHAP** (SHapley Additive exPlanations) to provide valuable insights into the most important features driving the predictive performance of the models.
* Summarized the results through a research [paper](https://nbviewer.org/github/cpmalenab/fire-resistance/blob/master/paper/Prediction%20of%20Fire%20Resistance%20of%20Fiber-Reinforced%20Polymer-Strengthened%20Concrete%20Beams%20Using%20Machine%20Learning%20Techniques.pdf), providing in-depth analysis of model performance, feature relevance, and practical implications of the developed models for real-world use.

<center>

| Model                      | RMSE (minutes) | MAE (minutes) | R^2 (%) |
|----------------------------|----------------|---------------|---------|
| XGBoost                    |     17.82      |     9.87      |  0.942  |
| Random Forest              |     18.58      |     10.33     |  0.937  |
| Deep Neural Networks       |     17.66      |     12.15     |  0.942  |
| Support Vector Regressor   |     26.49      |     14.71     |  0.871  |
| Linear Regression          |     44.10      |     33.77     |  0.650  |

</center>

![xgboost_results](./images/xgboost_results.JPG)

The findings of this research indicate that XGBoost demonstrates strong performance in overall fire resistance prediction, while Deep Neural Networks excel particularly in capturing extreme values of fire resistance. Key factors influencing fire resistance prediction include load ratio, insulation depth, steel area, concrete cover, and total load. By showcasing the effectiveness of machine learning methods, this study emphasizes their potential to address highly nonlinear problems in classical engineering domains where conventional knowledge-based approaches may prove impractical or unfeasible. The automated nature of these approaches holds promise for significant time and resource savings, reducing reliance on manual effort.

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
