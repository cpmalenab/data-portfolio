---
permalink: /blogs/
title: "Blog Posts"
author_profile: true
---

# [From Domain to Idioms: A Critique of Failure Factories](https://cpmalenab.github.io/data-portfolio/blogs/failure-factories/)

![failure_factories](/data-portfolio/images/failure_factories.jpg){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">Failure Factories by Tampa Bay Times</figcaption>

Data journalism is a data-driven approach to communicating stories and presenting news for mass media consumption. The award-winning story, [Failure Factories](https://projects.tampabay.com/projects/2015/investigations/pinellas-failure-factories/chart-failing-black-students/), adopted this approach to showcase the increasing resegregation of Pinellas County public schools to the public at the broadest reach possible. The decision to publish the story through a scroll-based format, paired with its easy accessibility using mobile platforms, reflects the writers’ aim to engage more readers in the ongoing crisis in Pinellas County. 

---

# [Database Normalization](https://github.com/cpmalenab/database_normalization)

Organizing information in a relational database requires eliminating redundancy to maintain the integrity and consistency of data. If left unchecked in the initial stages of project development, this could result in serious ramifications in terms of performance and waste of resources. For instance, if there is only a single table to store the entire data set then the program has to do a full database scan even for queries that require only a few records. Moreover, if data is repeated over several rows, a single error can cause erroneous data or potential loss of information.

![music_schema](/data-portfolio/images/music_schema.PNG){: .align-center height="600px"}
<figcaption style="text-align:center; font-size: smaller;">Relational Schema of Music Library after Database Normalization</figcaption>

This [notebook](https://nbviewer.org/github/cpmalenab/database_normalization/blob/main/Creating%20Normalized%20Tables.ipynb) aims to discuss the following:

1. Demonstrate the normalization process through a sample music library database.
2. Present and discuss each *normal form* supplemented by Python code and psycopg2 library to manipulate the PostgreSQL database.
3. Define concepts behind database normalization to better understand the theoretical foundation of the topic.
4. Complement the normalized database using an Entity-Relationship Diagram.
5. Identify possible trade-offs and implications of normalizing a database.

---

