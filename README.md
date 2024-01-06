<html>
<head>
    <!-- Add relevant meta tags and link external CSS if needed -->
    <title>Chicago Crime Data Presentation</title>
</head>
<body style="background-color: #f0f0f0;">
    <img src="chic1.jpeg" alt="Chicago crime" />
    <header>
        <h1>Chicago Crime</h1>
    </header>

    <div class="section">
        <h2>Introduction</h2>
        <p>
            In this presentation, we embark on a detailed exploration of reported crime incidents in Chicago, a dataset that extends from 2001 to the current date, excluding the most recent seven days. This data, extracted from the Chicago Police Department's Citizen Law Enforcement Analysis and Reporting (CLEAR) system, reflects a broad spectrum of crime incidents, with a notable exception for murders where each victim's data is separately recorded.
            <!-- Content Continues -->
        </p>
        <p>
            For more information visit: <a href="https://data.cityofchicago.org">click here</a>
        </p>
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
        <p>
            Querying massive datasets can be time-consuming and expensive without the right hardware and infrastructure. Google BigQuery solves this problem by enabling super-fast, SQL queries against append-mostly tables, using the processing power of Google's infrastructure.
        </p>
        <ul>
            <li><a href="https://cloud.google.com/python/docs/reference/automl/latest">Client Library Documentation</a></li>
            <li><a href="https://cloud.google.com/bigquery/docs/reference/rest">Product Documentation</a></li>
        </ul>
        <table>
            <tr>
                <td>SQL Code: <a href="https://github.com/dsrichard97/chicagosql">Pull Request raw code</a></td>
            </tr>
        </table>
        <img src="gif1.gif" alt="SQL alias list overview" />
        <p>Quick overview of SQL alias list.</p>
        <p><!-- Gets data from the last 5 years -->
            SELECT * FROM `bigquery-public-data.chicago_crime.crime` WHERE year >= EXTRACT(YEAR FROM CURRENT_DATE()) - 5;
        </p>
    </div>

    <div class="section" id="Usage">
        <h2>Usage</h2>
        <p>The usage is for law enforcement people or people interested in crime data. The intention of this project is rather to raise awareness of crimes and hotspots.</p>
    </div>

    <div class="section" id="Dataset">
        <h2>Dataset</h2>
        <p>
            <!-- Dataset content -->
        </p>
    </div>

    <div class="section" id="Analysis">
        <h2>Analysis</h2>
        <img src="crime.gif" alt="Crime analysis" />
        <p>
            Crime has been up in the last couple of years. The R markdown provides some quick insights on exploratory information.
        </p>
        <!-- Include code snippets and screenshots -->
    </div>

    <div class="section">
        <h2>Visuals</h2>
        <img src="tab1.png" alt="Chicago crime" />
        <p>Check out my Tableau dashboard: <a href="https://public.tableau.com/shared/2ZZDXFHQX?:display_count=n&:origin=viz_share_link">Tableau Link</a></p>
    </div>

    <div class="section">
        <h2>Additional Resources</h2>
        <p>
            <a href="https://popcenter.asu.edu/sites/default/files/learning/60steps/index3f62.html?stepNum=25">Crime Analysis in 60 steps</a><br>
            <a href="https://projects.itrcweb.org/gsmc-1/Content/GW%20Stats/5%20Methods%20in%20indiv%20Topics/5%208%20Temporal%20Analysis.htm">Motivation</a><br>
            <a href="https://pro.arcgis.com/en/pro-app/latest/help/mapping/time/temporal-data.htm">ArcGIS Pro Time Series Data Store Values</a>
        </p>
    </div>
</body>
</html>

