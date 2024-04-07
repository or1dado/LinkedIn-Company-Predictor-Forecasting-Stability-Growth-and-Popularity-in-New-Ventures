<h1 align="center" id="title">New Company Success Predictor</h1>
<p align="center">Keren Haruvi, Omri Itzhaki, Or Dado</p>

<h2>📁 Contents</h2>
<ul>
    <li><a href="#section1">Overview</a></li>
    <li><a href="#section2">How To Run?</a></li>
    <li><a href="#section3">Data Collection and Integration</a></li>
    <li><a href="#section4">Data Analysis and Feature Selection</a></li>
    <li><a href="#section5">AI Methodologies</a></li>
    <li><a href="#section6">Results and Evaluation</a></li>
    <li><a href="#section7">Limitations</a></li>
    <li><a href="#section8">Conclusions</a></li>
</ul>

<h2 id="section1">📚 Overview:</h2>
<p id="description">Understanding the potential success of a new company is crucial for various stakeholders, including job seekers, employees, investors, and stakeholders. This project aims to address the research question: "How likely is a new company to succeed?" We focus on measures of stability, growth, and popularity for new companies, leveraging LinkedIn data and Google Trends.</p> 

<img src="https://github.com/or1dado/LinkedIn-Company-Success-Predictor/blob/main/images/project%20logo.jpeg" width="250" />

<h2 id="section2">⚙️ How To Run?</h2>
<ol>
  <li>
    <p>Run the "Create companies URLs for Scraping" notebook in Databricks. This step is optional and is only necessary if you want to perform the scraping process yourself. The output of the notebook will be used in the scraping phase.</p>
  </li>
  <li>
    <p>Use the "scrape code" to perform scraping from the URLs extracted in the previous phase. This step is also optional and is only required if you want to conduct the scraping process yourself. The data is already available in the data file.</p>
  </li>
  <li>
    <p>Run the "Merge code" notebook. This notebook will merge the output of the scraping process and create two datasets: one for new companies and the other for old companies. The merged datasets will be saved in the following path: "data/trend_data".</p>
  </li>
  <li>
    <ol>
      <li>
        <p>Run the "Project_preprocess" notebook. Before running this notebook, make sure to add the paths of the datasets for the new and old companies in Cell 4. Additionally, edit the paths where the output of the notebook will be saved in Cell 29.</p>
        <p>Follow these steps as illustrated in the images below:</p>
        <img src="https://github.com/or1dado/LinkedIn-Company-Success-Predictor/blob/main/images/pre_process_guide.jpg" width="1050" />
        <img src="https://github.com/or1dado/LinkedIn-Company-Success-Predictor/blob/main/images/pre_process_save_guide.jpg" width="1050" />
      </li>
      <li>
        <p>Run the "Features_analysis" notebook in Databricks. This is optional if you want to explore the features. To run it, replace paths in cell 7 with those of the pre-process.</p>
      </li>
    </ol>
  </li>
  <li>
    <p>Run the "Project_part1_stability" notebook in Databricks again. Edit the paths in Cell 7 to match the paths saved in the pre-process phase. Specify the path to save the output of the notebook in Cell 15. This phase calculates the stability scores.</p>
  </li>
  <li>
    <p>Run the "Project_part2_popularity" notebook in Databricks again. Edit the paths in Cell 7 to match the paths saved in the pre-process phase. Also edit the path of the stability df saved in phase 5 in cell 13. Specify the path to save the output of the notebook in Cell 17. This phase calculates the popularity scores.</p>
  </li>
  <li>
    <p>Run the "Project_results" notebook in Databricks again to get results and perform analysis. Edit the paths in Cell 5 to match the paths saved in the pre-process phase. Also, edit the paths in Cells 7 and 9 to the output paths from phases 6 (stability) and 5 (popularity) respectively. To view the images in Cells 31 and 32, replace the paths with those in the image files ('images/quant.png', 'images/kodiak.png').</p>
  </li>
</ol>




<h2 id="section3">👩🏻‍💻 Data Collection and Integration</h2>
<ul>
<li>Utilized LinkedIn's company dataset, filtering by foundation year to distinguish between established and new companies.</li>
<li>Gathered additional time-series data from Google Trends by querying company names.</li>
<li>Integrated Google Trends data for stability, popularity, and growth insights into our predictive models.</li>
</ul>

<h2 id="section4">📊 Data Analysis and Feature Selection</h2>
<ul>
<li>Preprocessed LinkedIn data by handling missing values and excluding overly common or rare values.</li>
<li>Performed column transformations and feature engineering to enhance model performance.</li>
<li>Employed various methodologies for stability, popularity, and growth measures.</li>
</ul>

<h2 id="section5">🧠 AI Methodologies</h2>
<ul>
<li>Stability Measure: Utilized cosine similarity between new and established companies to predict stability.</li>
<li>Popularity Measure: Trained a linear regression classifier model to predict popularity labels.</li>
<li>Growth Measure: Fitted SARIMA models to forecast growth trends for new companies.</li>
</ul>

<h2 id="section6">📋 Results and Evaluation</h2>
<ul>
<li>Stability, popularity, and growth scores were predicted for new companies.</li>
<li>Manual evaluations and sampling techniques validated the accuracy of predictions.</li>
<li>Identified industries with the highest potential for success based on model results.</li>
</ul>

<h2 id="section7">🚧 Limitations</h2>
<ul>
<li>Resource and technological constraints impacted data scraping and model optimization.</li>
<li>Data limitations and quality issues introduced uncertainties and biases in the results.</li>
</ul>

<h2 id="section8">🗨 Conclusions</h2>
<ul>
<li>Successfully answered the research question regarding new company success likelihood.</li>
<li>Provided valuable insights for stakeholders, laying a foundation for future research and analysis.</li>
</ul>
