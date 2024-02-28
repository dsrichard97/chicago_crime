<h1 align="center">Geospatial & Cluster Analysis - Chicago Crime</h1>
<p align="center">
<p align="center">
  <img src="chic1.jpeg" width="400" height="340" allow="autoplay">
</p>
<body>
<body style="background-color: #f0f0f0;">
<p>
  <img src="https://img.shields.io/badge/SQL%2B-green" title="SQL">
  <img src="https://img.shields.io/badge/Cluster%3B-blue" title="Cluster">
  <img src="https://img.shields.io/badge/Reports%2B-orange" title="Reports">
    <img src="https://img.shields.io/badge/Tableau%2B-red" title="Tableau">
  <img src="https://img.shields.io/github/last-commit/dsrichard97/chicago_crime">
  <img src="https://img.shields.io/github/repo-size/dsrichard97/chicago_crime">

<p>
  <h2>Authors</h2>
  <ul>
    <li><a href="https://github.com/dsrichard97">@dsrichard97</a></li>
  </ul>
</p>

<div class="section">
    <p>
  <h2>Table of Contents</h2>
  <ul>
    <li><a href="#business-problem" target="_parent">Business Problem</a></li>
    <li><a href="#data-source">Data Source</a></li>
    <li><a href="#methods">Methods</a></li>
    <li><a href="#tech-stack">Tech Stack</a></li>
    <li><a href="#quick-glance">Quick glance at the Results</a></li>
    <li><a href="#lesson-learned">Lessons learned and Recommendation</a></li>
    <li><a href="#limitation">Limitation and what can be Improved</a></li>
  </ul>
</p>
</div>


<P>
  <section id="business-problem">
    <h2>Business Problem</h2>
    <p>
      Create reports that visualizes geographic crimes to be able to gather informed decisions for law enforcement.
    </p>
    <h2>Crime Information</h2>
    <p>
      Crime data spans from 2001 to near present. Data is capture from Chicago Police department knowne as the CLEAR(Citizen Law Enforcement Analysis and Reporting) system.
The data contains incidents to their blocks and crimes. This exploration is not just about numbers; it's a narrative of resilience and response, painted with the broad strokes of community engagement and the fine lines of detailed analysis. While the Chicago Police Department makes every effort to ensure the reliability of this data, the complexities of crime reporting mean that absolute accuracy and timeliness are aspirational goals.This presentation aims to provide a data-driven narrative on public safety in Chicago. We will delve into this dataset, publicly available under the terms provided by the City of Chicago and offered 'AS IS' by Google, to uncover patterns, understand trends, and offer insights into the complex domain of urban crime and safety. For more information visit:
      <a href="https://data.cityofchicago.org">Chicago Crime</a>
    </p>
  </section>
</P>

<p>
  <section id="data-source">
    <h2>Data Source</h2>
     <p> This project is designed for use by law enforcement professionals and individuals with an interest in crime data. Its primary objective is to increase awareness of criminal activities and to pinpoint crime hotspots. By providing detailed insights into crime trends and locations, the project aims to support proactive measures and informed decision-making in crime prevention and safety enhancement. This specifically highlights hotspots. For a quick <b>EXCEL</b> snapshot: <a href="https://github.com/dsrichard97/chicago_crime/blob/main/crimedataquery.xls">click here</a>. </p>
  </section>
</p>


<p>
  <section id="methods">
    <h2>Methods</h2>
    <ul>
      <li>SQL Code</li>
      <li>Excel Data</li>
      <li>Tableau Dashboard</li>
      <li>R code - Geospatial Analysis </li>
      <li>PowerPoint</li>
    </ul>
  </section>
</p>


<p>
  <section id="quick-glance">
    <h2>Quick Glance at the Results</h2>
       <td style="padding: 10px;">
            <b>SQL Code:</b> <a href="https://github.com/dsrichard97/chicagosql" target="_blank">Pull Request</a>
        </td>
      </p>

<center>
    <div class="container">
  <img src="gif1.gif" alt="Snow" style="width:100%;">
  <div class="bottom-left">Data Type</div>
</div>
<body>
    <h2>SQL Code Snippet:</h2>
    <!-- Code block for copying -->
    <pre>
        SELECT * 
        FROM `bigquery-public-data.chicago_crime.crime` 
        WHERE year &gt;= EXTRACT(YEAR FROM CURRENT_DATE()) - 5;
    </pre>
    <p>Copy the above SQL code snippet to query data from the last 5 years.</p>
</body>


<body>
  <h3>R Code</h3>
  <p>
  Click on image to link
  </p>
    <a href="http://rpubs.com/diazrichard98/1135536" target="_blank">
        <img src="https://raw.githubusercontent.com/dsrichard97/chicago_crime/main/crime.gif" alt="Descriptive Text" style="width: auto; height: auto;">
    </a>
</body>

<body>
    <h3>Python Code</h3>
  <p>
    Click on image to link
  </p>
<a href="https://github.com/dsrichard97/chicago_crime/blob/main/crime%20data/crime%20data.md" target="_blank">
        <img src="https://raw.githubusercontent.com/dsrichard97/chicago_crime/main/pyplot.png" alt="Descriptive Text" style="width: auto; height: auto;">
    </a>
  <ul>
<li> Cluster 0: This is one group or 'cluster' of crime incidents as identified by the K-means algorithm. All points in this cluster are more similar to each other (in terms of their geographical location - latitude and longitude) than they are to points in other clusters. <\li>
  
<li> Cluster 1: This represents a different group of crime incidents, again grouped based on their proximity to each other. <\li>
  
<li> Clusters 2, 3, and 4: Similarly, these labels represent additional groups of crime incidents. <\li>
</ul>

The goal of this clustering is to identify 'hotspots' of crime in Chicago based on geographical data. Each cluster represents a geographical area where crimes have occurred with higher density compared to other areas. By examining these clusters, you can gain insights into which areas require more attention or resources for crime prevention and law enforcement.

</body>


<body>
    <h3>Tableau Dashboard</h3>
  <p>
    Click on image to link
  </p>
  <a href="https://public.tableau.com/views/CRIMEDATA_17044875678690/MAINDB?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link" target="_blank">
        <img src="https://raw.githubusercontent.com/dsrichard97/chicago_crime/main/tab1.png" alt="Descriptive Text" style="width: auto; height: auto;">
    </a>
</body>

<b>Visualizations: The goal is to craft compelling narratives for stakeholders. </b>
          <li> I utilized R and Python programming to analyze and reveal patterns of crime, delving into the complex relationship between geographic locations and time to highlight less explored aspects of urban crime. Through geospatial analysis, I identified crime hotspots and patterns at a micro-level, effectively pinpointing critical areas needing attention. The reports I crafted aim to provide actionable insights, enabling targeted strategic interventions.

My analysis of Chicago's 2022-2023 crime data spotlighted the top five crimes, showcasing my capability to simplify complex datasets into clear, actionable insights. This work not only brought to light prevalent crime trends, such as deceptive practices, but also employed sophisticated techniques like K-means clustering in Python for a comprehensive analysis of crime across a wider scope. This effort demonstrates my technical prowess, innovative problem-solving approach, and strategic thinking in crime prevention and safety.
          </li>
        </ul>
<p>


<p>
  <section id="lesson-learned">
  <h2>Lessons Learned and Recommendation</h2>
  <p>
   
  </p>



<P>
  <section id="limitation">
    <h2>Limitation and what can be Improved</h2>
    <p>












  
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



