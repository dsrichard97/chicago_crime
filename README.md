<img src="chic1.jpeg" alt="Chicago crime">
<body>
    <header>
        <h1> Chicago Crime
</h1>
    </header>
<body style="background-color: #f0f0f0;">


<div class="section">
    <h2>Introduction</h2>
    <p>
        In this presentation, we embark on a detailed exploration of reported crime incidents in Chicago, a dataset that extends from 2001 to the current date, excluding the most recent seven days. This data is extracted from the Chicago Police Department's Citizen Law Enforcement Analysis and Reporting (CLEAR) system, reflects a broad spectrum of crime incidents, with a notable exception for murders where each victim's data is separately recorded.

A key aspect of this dataset is its commitment to the privacy of crime victims. To this end, the information is generalized to the block level, without pinpointing specific locations. It's important to highlight that the dataset encompasses unverified reports and preliminary crime classifications that may be subject to change following further investigation. This aspect underscores the dynamic and somewhat tentative nature of the data.

Given the potential for mechanical or human error, the Chicago Police Department explicitly states that the accuracy, completeness, timeliness, or correct sequencing of the data cannot be guaranteed. As a result, this dataset should not be used for time-based comparative purposes.

This presentation aims to provide a data-driven narrative on public safety in Chicago. We will delve into this dataset, publicly available under the terms provided by the City of Chicago and offered 'AS IS' by Google, to uncover patterns, understand trends, and offer insights into the complex domain of urban crime and safety." For more information visit: [click here](https://data.cityofchicago.org)    </p>
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

<li><a href="https://cloud.google.com/python/docs/reference/automl/latest"> Client Library Documentation</a></li>

    

<li><a href="https://cloud.google.com/bigquery/docs/reference/rest"> Product Documentation </a></li>


<br>
    <table> 
    <tr>
    <td> 
        SQL Code: <a href="https://github.com/dsrichard97/chicagosql"> Pull Request raw code</a>
    </td>
    </tr>
    </table> 
</br>

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
             <a href="https://github.com/dsrichard97/chicago_crime/blob/main/CHICAGO%20CRIME.pptx">PowerPoint - High Level Summary of all the Process.</a><br>
            <a href="https://popcenter.asu.edu/sites/default/files/learning/60steps/index3f62.html?stepNum=25">Crime Analysis in 60 steps</a><br>
            <a href="https://projects.itrcweb.org/gsmc-1/Content/GW%20Stats/5%20Methods%20in%20indiv%20Topics/5%208%20Temporal%20Analysis.htm">Motivation</a><br>
            <a href="https://pro.arcgis.com/en/pro-app/latest/help/mapping/time/temporal-data.htm">ArcGIS Pro Time Series Data Store Values</a>
        </p>
    </div>

</div>


