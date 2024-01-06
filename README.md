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
    
    <!-- Gets data from the last 5 years -->
    SELECT * FROM `bigquery-public-data.chicago_crime.crime` WHERE year >= EXTRACT(YEAR FROM CURRENT_DATE()) - 5;
</div>

<div class="section" id="Usage">
    <h2>Usage</h2>
    <p> The usuage is for law enforcement people or people who intrested in crime data. The intention of this project is rather to raise awareness of crimes and hotspots.</p>
</div>

<div class="section" id="Dataset">
    <h2>Dataset</h2>
    <p> If you are intrested in looking at the sql pull look at the previous. However, I highlighted most of my energy and portion into visuals to show the rise of crime from 2019-2023. The tableau link includes a high level overview of the data. For more programmers, I have attached a link to python file and r code that display a temporal analysis. Crime rates have been up and the goal is to raise awareness of how important governement officials are. This specifically highlights hotspots. </p>
</div>

<div class="section" id="Analysis">
    <h2>Analysis</h2>
        <IMG SRC="crime.gif">
    <p> Crime has been up in the last couple of years. The R markdown provides some quick insights on exploratory information. </p>
    <!-- Include code snippets and screenshots -->
</div>

<div class="section">
    <h2>Visuals</h2>
    <img src="tab1.png" alt="Chicago crime">
    <p>Check out my Tableau dashboard: https://public.tableau.com/shared/2ZZDXFHQX?:display_count=n&:origin=viz_share_link  </p>

</div>
<div class='tableauPlaceholder' id='viz1704503669657' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;CR&#47;CRIMEDATA_17044875678690&#47;MAINDB&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='views&#47;CRIMEDATA_17044875678690&#47;MAINDB?:language=en-US&amp;:embed=true' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;CR&#47;CRIMEDATA_17044875678690&#47;MAINDB&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1704503669657');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='1366px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='818px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='1366px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='818px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.minHeight='1450px';vizElement.style.maxHeight=(divElement.offsetWidth*1.77)+'px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>


<div class="section">
    <h2>Additional Resources</h2>
    <p>Links to additional documentation, related projects...</p>
</div>

</body>
</html>
