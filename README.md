<h1 align="center" id="title">New Company Success Predictor</h1>
<p align="center">Keren Haruvi, Omri Itzhaki, Or Dado</p>

<h2>📋 Contents</h2>
<ul>
    <li><a href="#section1">Overview</a></li>
    <li><a href="#section2">Installation</a></li>
    <li><a href="#section3">Data Collection and Integration</a></li>
    <li><a href="#section4">Data Analysis and Feature Selection</a></li>
    <li><a href="#section5">AI Methodologies</a></li>
    <li><a href="#section6">Results and Evaluation</a></li>
    <li><a href="#section7">Limitations and Reflection</a></li>
    <li><a href="#section8">Conclusions</a></li>
</ul>

<h2 id="section1">📚 Overview:</h2>
<p id="description">Understanding the potential success of a new company is crucial for various stakeholders, including job seekers, employees, investors, and stakeholders. This project aims to address the research question: "How likely is a new company to succeed?" We focus on measures of stability, growth, and popularity for new companies, leveraging LinkedIn data and Google Trends.</p> 

<img src="https://github.com/or1dado/LinkedIn-Company-Success-Predictor/blob/main/project%20logo.jpeg" width="250" />

<h2 id="section2">⚙️ Installation</h2>
<ol>
<li>Clone the GitHub repository:</li>
<ul>
<pre><code>https://github.com/or1dado/LinkedIn-Company-Success-Predictor.git</code></pre>
</ul>

<li>Install the required packages using pip:</li>
<ul>
<pre><code>pip install -r requirements.txt</code></pre>
</ul>

</ol>

<h2 id="section3">Data Collection and Integration</h2>
<ul>
<li>Utilized LinkedIn's company dataset, filtering by foundation year to distinguish between established and new companies.</li>
<li>Gathered additional time-series data from Google Trends by querying company names.</li>
<li>Integrated Google Trends data for stability, popularity, and growth insights into our predictive models.</li>
</ul>

<h2 id="section4">Data Analysis and Feature Selection</h2>
<ul>
<li>Preprocessed LinkedIn data by handling missing values and excluding overly common or rare values.</li>
<li>Performed column transformations and feature engineering to enhance model performance.</li>
<li>Employed various methodologies for stability, popularity, and growth measures.</li>
</ul>

<h2 id="section5">AI Methodologies</h2>
<ul>
<li>Stability Measure: Utilized cosine similarity between new and established companies to predict stability.</li>
<li>Popularity Measure: Trained a linear regression classifier model to predict popularity labels.</li>
<li>Growth Measure: Fitted SARIMA models to forecast growth trends for new companies.</li>
</ul>

<h2 id="section6">Results and Evaluation</h2>
<ul>
<li>Stability, popularity, and growth scores were predicted for new companies.</li>
<li>Manual evaluations and sampling techniques validated the accuracy of predictions.</li>
<li>Identified industries with the highest potential for success based on model results.</li>
</ul>

<h2 id="section7">Limitations and Reflection</h2>
<ul>
<li>Resource and technological constraints impacted data scraping and model optimization.</li>
<li>Data limitations and quality issues introduced uncertainties and biases in the results.</li>
</ul>

<h2 id="section8">Conclusions</h2>
<ul>
<li>Successfully answered the research question regarding new company success likelihood.</li>
<li>Provided valuable insights for stakeholders, laying a foundation for future research and analysis.</li>
</ul>
