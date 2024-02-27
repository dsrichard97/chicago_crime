<h1 align="center">Geospatial Analysis - Chicago Crime</h1>
<p align="center">
<p align="center">
  <img src="chic1.jpeg" width="400" height="340" allow="autoplay">
</p>
<body>
<body style="background-color: #f0f0f0;">
<p>
  <img src="https://img.shields.io/badge/SQL%2B-green" title="SQL">
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
      Create an interactive dashboard that visualizes geographic crimes to be able to gather informed decisions for law enforcement.
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
    R code:
    
</body>

<body>
    Python code:
    
</body>


<body>
    Tableau Dashboard:
  
</body>








  
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



