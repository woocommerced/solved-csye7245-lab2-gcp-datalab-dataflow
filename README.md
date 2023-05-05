Download Link: https://assignmentchef.com/product/solved-csye7245-lab2-gcp-datalab-dataflow
<br>
This lab demonstrates GCP services like Datalab, Dataflow and BigQuery for implementing data analysis and preprocessing for machine learning.

Google Cloud Platform (GCP), offered by <a href="https://en.wikipedia.org/wiki/Google">Google</a>, is a suite of <a href="https://en.wikipedia.org/wiki/Cloud_computing">cloud computing</a> services that runs on the same infrastructure that Google uses internally for its end-user products, such as <a href="https://en.wikipedia.org/wiki/Google_Search">Google Search</a>, <a href="https://en.wikipedia.org/wiki/Gmail">Gmail</a>, <a href="https://en.wikipedia.org/wiki/Google_Drive">file storage</a>, and <a href="https://en.wikipedia.org/wiki/YouTube">YouTube</a>. Alongside a set of management tools, it provides a series of modular cloud services including computing, <a href="https://en.wikipedia.org/wiki/Computer_data_storage">data storage</a>, <a href="https://en.wikipedia.org/wiki/Data_analysis">data analytics</a> and <a href="https://en.wikipedia.org/wiki/Machine_learning">machine learning</a>.




Google Cloud Platform provides <a href="https://en.wikipedia.org/wiki/Infrastructure_as_a_service">infrastructure as a service</a>, <a href="https://en.wikipedia.org/wiki/Platform_as_a_service">platform as a service</a>, and <a href="https://en.wikipedia.org/wiki/Serverless_computing">serverless computing</a> environments.




Cloud <strong>Datalab </strong>is a powerful interactive tool created to explore, analyze, transform and visualize data and build machine learning models on Google Cloud Platform. It runs on Google Compute Engine and connects to multiple cloud services easily so you can focus on your data science tasks.




Google Cloud <strong>Dataflow </strong>is a cloud-based data processing service for both batch and real-time data streaming applications. It enables developers to set up processing pipelines for integrating, preparing and analyzing large data sets, such as those found in Web analytics or big data analytics applications.




Storing and querying massive datasets can be time consuming and expensive without the right hardware and infrastructure. <strong>BigQuery</strong> is an <a href="https://cloud.google.com/solutions/bigquery-data-warehouse">enterprise data warehouse</a> that solves this problem by enabling super-fast SQL queries using the processing power of Google’s infrastructure.

<h1><strong> Dataset</strong></h1>

We used public Natality dataset to create an ML model to predict a baby’s weight given a number of factors about the pregnancy and the baby’s mother.




We cloned the <a href="https://github.com/GoogleCloudPlatform/training-data-analyst"><strong>https://github.com/GoogleCloudPlatform/training-data-analyst</strong></a> github path and used <strong>training-data-analyst/blogs/babyweight/babyweight.ipynb</strong> notebook for our data processing and model creation.




<h1></h1>

<h1><strong>Experiment Setup</strong></h1>

<h2><strong>Prerequisites</strong></h2>

<ol>

 <li>In the Google Cloud Console, on the project selector page, select or create a Google Cloud project.</li>

 <li>Enabled the BigQuery, AI Platform, Cloud Source Repositories, Dataflow, and Datalab APIs.</li>

</ol>

<h2><strong>Launching Datalab</strong></h2>




Following are the steps to launch Datalab:




<ul>

 <li>Open Cloud Shell Editor</li>

</ul>







<ul>

 <li>Retrieved Google Cloud Project id using the below command</li>

 <li>Created a Datalab instance</li>

 <li>Connection was established and instance of Datalab created at port 8081</li>

</ul>

<h2><strong>Cloning Datalab Notebook</strong></h2>

<ul>

 <li>Opened a new notebook and copy pasted below command</li>

</ul>

!git clone <a href="https://github.com/GoogleCloudPlatform/training-data-analyst">https://github.com/GoogleCloudPlatform/training-data-analyst</a>

<h1><strong>Use Cases</strong></h1>

<h2><strong>Data Exploration, Preprocessing and Visualization in Datalab</strong></h2>

Project ID and Bucket setup in notebook

<ul>

 <li>In the first cell, set the variable PROJECT to your project ID.</li>

 <li>Set the variable BUCKET to your bucket name in the first cell. For your bucket name, use your project ID as a prefix and my-bucket: project-ID-my-bucket</li>

 <li>Leave REGION as us-central1.</li>

</ul>




Fetching data in dataframe using BigQuery

Visualizing count and average of babies

Visualizing correlation between Mother’s age and number of babies and there average weight

Visualizing plurality trends

Correlation between gestation period and babies weight and count

<h2><strong>Preprocessing using apache beam</strong></h2>

We modified the data such that we can simulate what is known if no ultrasound has been performed. If I didn’t need preprocessing, I could have used the web console. Also, I prefer to script it out rather than run queries on the user interface. Therefore, I am using Cloud Dataflow for the preprocessing.




<h1><strong>Results</strong></h1>

Job took around 48mins to finish

Throughput Metrices




CPU Utilization

<h2><strong>Data loaded in the GCP bucket in csv form</strong></h2>

<h1><strong>Lesson Learned</strong></h1>

<ol>

 <li>Learned to set up a project in Google Cloud and instantiate DataLab from Cloud shell editor using shell commands.</li>

 <li>Data exploration in Datalab and writing BigQuery to load data in dataframe and visualization.</li>

 <li>Preprocessing of data using Dataflow</li>

</ol>




<strong>References</strong>

<a href="https://console.cloud.google.com/home/dashboard?project=sunlit-adviser-303301&amp;_ga=2.197393647.171323457.1614132709-2114907062.1611967416&amp;_gac=1.91198568.1613410875.Cj0KCQiA1KiBBhCcARIsAPWqoSqLlRaYf255AYUskJXnXDtQpOTIqR6qIKcffq5HM2JDrJjXDpgeKkwaAnrnEALw_wcB"><strong>https://console.cloud.google.com/home/dashboard?project=sunlit-adviser-303301&amp;_ga=2.197393647.171323457.1614132709-2114907062.1611967416&amp;_gac=1.91198568.1613410875.Cj0KCQiA1KiBBhCcARIsAPWqoSqLlRaYf255AYUskJXnXDtQpOTIqR6qIKcffq5HM2JDrJjXDpgeKkwaAnrnEALw_wcB</strong></a>

<strong> </strong>

<a href="https://en.wikipedia.org/wiki/Google_Cloud_Platform"><strong>https://en.wikipedia.org/wiki/Google_Cloud_Platform</strong></a>

<strong> </strong>

<strong> </strong>

<strong> </strong>