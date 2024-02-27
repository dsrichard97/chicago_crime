<h1 align="center">Geospatial Analysis: Chicago Crime</h1>
<p align="center">
<p align="center">
  <img src="chic1.jpeg" width="400" height="340" allow="autoplay">
</p>
<body>
<body style="background-color: #f0f0f0;">


<div class="section">
    <h2>Introduction</h2>
    <p>
        
        Dive into the heart of Chicago with a captivating journey through its crime data, spanning from the year 2001 right up to the present, with a slight pause to respect the latest week's confidentiality. This data is provided from Chicago Police Department's innovative CLEAR system (Citizen Law Enforcement Analysis and Reporting).

Our expedition is guided by a profound respect for the privacy of those affected by crime. With precision, we map incidents to their blocks, preserving anonymity while shedding light on trends that shape the city's safety landscape. However, it's crucial to navigate this data with an understanding of its fluid nature—initial reports and classifications are stepping stones in an ongoing investigative process, revealing a dataset that's as alive and evolving as Chicago itself.

This exploration is not just about numbers; it's a narrative of resilience and response, painted with the broad strokes of community engagement and the fine lines of detailed analysis. While the Chicago Police Department makes every effort to ensure the reliability of this data, the complexities of crime reporting mean that absolute accuracy and timeliness are aspirational goals. Thus, this dataset stands not as a static snapshot, but as a living document, inviting a thoughtful exploration of Chicago's socio-legal fabric without the intent for time-sensitive comparisons.

Join us on this insightful journey, where data not only tells the story of crime but also of a city's ongoing quest for justice and peace. This presentation aims to provide a data-driven narrative on public safety in Chicago. We will delve into this dataset, publicly available under the terms provided by the City of Chicago and offered 'AS IS' by Google, to uncover patterns, understand trends, and offer insights into the complex domain of urban crime and safety." For more information visit: [click here](https://data.cityofchicago.org)    </p>
</div>

<div class="section">
    <h2>Table of Contents</h2>
    <ul>
        <li><a href="#Installation">Installation and Setup</a></li>
        <li><a href="#Usage">Usage</a></li>
        <li><a href="#Dataset">Dataset</a></li>
        <li><a href="#Analysis">Analysis</a></li>
        <li><a href="#Visuals">Visuals</a></li>
        <li><a href="#Resources">Resources</a></li>
        <!-- Add other sections as needed -->
    </ul>
</div>

<div class="section" id="Installation">
    <h2>Installation and Setup</h2>
    <p>Querying massive datasets can be time consuming and expensive without the right hardware and infrastructure. Google BigQuery solves this problem by enabling super-fast, SQL queries against append-mostly tables, using the processing power of Google's infrastructure.

<table border="1" style="border-collapse: collapse; width: 100%;">
    <tr>
        <td style="padding: 10px;">
            <b>SQL Code:</b> <a href="https://github.com/dsrichard97/chicagosql" target="_blank">Pull Request raw code</a>
        </td>
    </tr>
</table>


<li><a href="https://cloud.google.com/python/docs/reference/automl/latest"> Client Library Documentation</a></li>
<li><a href="https://cloud.google.com/bigquery/docs/reference/rest"> Product Documentation </a></li>


   


<center>
    <div class="container">
  <img src="gif1.gif" alt="Snow" style="width:100%;">
  <div class="bottom-left">Quick overview of SQL alias list</div>
</div>
<center>
    
    <!-- Gets data from the last 5 years -->
    SELECT * FROM `bigquery-public-data.chicago_crime.crime` WHERE year >= EXTRACT(YEAR FROM CURRENT_DATE()) - 5;
</div>

<div class="section" id="Usage">
    <h2>Usage</h2>
    <p> The usuage is for law enforcement people or people who intrested in crime data. The intention of this project is rather to raise awareness of crimes and hotspots.</p>
</div>

<div class="section" id="Dataset">
    <h2>Dataset</h2>
    <p> This project is designed for use by law enforcement professionals and individuals with an interest in crime data. Its primary objective is to increase awareness of criminal activities and to pinpoint crime hotspots. By providing detailed insights into crime trends and locations, the project aims to support proactive measures and informed decision-making in crime prevention and safety enhancement. This specifically highlights hotspots. For a quick <b>EXCEL</b> snapshot: <a href="https://github.com/dsrichard97/chicago_crime/blob/main/crimedataquery.xls">click here</a>. </p>
</div>

<div class="section" id="Analysis">
    <h2>Analysis</h2>
        <IMG SRC="crime.gif">
    <p>The report, 'Chicago Crime Data Reporting,' dated January 5, 2024, presents an in-depth exploratory data analysis (EDA) and a meticulous temporal assessment of crime statistics in Chicago for the years 2022-2023. Conducted using R and various libraries such as readr, lubridate, dplyr, ggplot2, leaflet, leaflet.extras, and cluster, the analysis encompasses data preparation, the identification of predominant crime types via bar plots, and block-level examination to identify areas with increased specific criminal activities. The study further delves into time-related trends in these regions, uncovering significant shifts in crime frequencies. A notable aspect of this analysis is the integration of geospatial and temporal visualizations with interactive maps, enhanced by machine learning techniques like <b>K-means clustering</b> to outline <b>crime hotspots</b>. This comprehensive methodology not only illuminates areas of concentrated crime and critical zones but also offers essential insights for decision-making by policymakers and law enforcement agencies. Overall, this analysis stands as a potent tool in understanding and addressing the complexities of urban crime. <b>R CODE - </b> https://rpubs.com/diazrichard98/1135536:display_count=n&:origin=viz_share_link </p>


<div class="section">
    <h2>Visuals</h2>
    <img src="tab1.png" alt="Chicago crime">
    <p>Check out my <b>Tableau dashboard</b>: https://public.tableau.com/shared/2ZZDXFHQX?:display_count=n&:origin=viz_share_link . For a high level overview - click on the PowerPoint below in the resources section. </p>
    
<div class="section">
        <h2>Resources</h2>
        <p>
             <a href="https://csulb-my.sharepoint.com/:p:/g/personal/richard_diazdeleon01_student_csulb_edu/EQnZJ2L5sJxChJji6DqvhL0BfsDbXO467AQWm8Dai6r9XA?e=uS6TA8">PowerPoint</a><br>
            <a href="https://popcenter.asu.edu/sites/default/files/learning/60steps/index3f62.html?stepNum=25">Crime Analysis in 60 steps</a><br>
            <a href="https://projects.itrcweb.org/gsmc-1/Content/GW%20Stats/5%20Methods%20in%20indiv%20Topics/5%208%20Temporal%20Analysis.htm">Motivation</a><br>
            <a href="https://pro.arcgis.com/en/pro-app/latest/help/mapping/time/temporal-data.htm">ArcGIS Pro Time Series Data Store Values</a>
        </p>
    </div>

</div>


