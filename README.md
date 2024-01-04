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

This presentation aims to provide a data-driven narrative on public safety in Chicago. We will delve into this rich dataset, publicly available under the terms provided by the City of Chicago and offered 'AS IS' by Google, to uncover patterns, understand trends, and offer insights into the complex domain of urban crime and safety." For more information visit: [click here
](https://data.cityofchicago.org)    </p>
</div>

<div class="section">
    <h2>Table of Contents</h2>
    <ul>
        <li><a href="#Installation">Installation and Setup</a></li>
        <li><a href="#Usage">Usage</a></li>
        <li><a href="#Dataset">Dataset</a></li>
        <li><a href="#Analysis">Analysis</a></li>
        <!-- Add other sections as needed -->
    </ul>
</div>

<div class="section" id="Installation">
    <h2>Installation and Setup</h2>
    <p>Querying massive datasets can be time consuming and expensive without the right hardware and infrastructure. Google BigQuery solves this problem by enabling super-fast, SQL queries against append-mostly tables, using the processing power of Google's infrastructure.
<br>
- <a href="https://cloud.google.com/python/docs/reference/automl/latest"> Client Library Documentation</a>
</br>
<br>
- <a href="https://cloud.google.com/bigquery/docs/reference/rest"> Product Documentation </a>
</br>
<br>
    <table> 
    SQL Code Configuration
    <tr>
    <td> 
        SQL Code: <a href="https://github.com/dsrichard97/chicagosql"> Pull Request raw code</a>
    </td>
    </tr>
    </table> 
</br>

<center>
    <IMG SRC="gif1.gif">
</center>
Quick overview of SQL alias list.
    
    <!-- Include any code snippets if necessary -->
    SELECT *
FROM `bigquery-public-data.chicago_crime.crime` 
WHERE year >= EXTRACT(YEAR FROM CURRENT_DATE()) - 5;
</div>

<div class="section" id="Usage">
    <h2>Usage</h2>
    <p>Detailed examples of how to use your project...</p>
    <!-- Include code snippets and screenshots -->
</div>

<div class="section" id="Dataset">
    <h2>Dataset</h2>
    <p>Detailed examples of how to use your project...</p>
    <!-- Include code snippets and screenshots -->
</div>

<div class="section" id="Analysis">
    <h2>Analysis</h2>
    <p>Detailed examples of how to use your project...</p>
    <!-- Include code snippets and screenshots -->
</div>

<div class="section">
    <h2>Visuals</h2>
    <p>Showcase your project with images, GIFs, or videos...</p>
</div>


<div class="section">
    <h2>Additional Resources</h2>
    <p>Links to additional documentation, related projects...</p>
</div>

</body>
</html>
