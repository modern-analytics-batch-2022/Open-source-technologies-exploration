![image](https://user-images.githubusercontent.com/98338535/153727108-df667a04-9b26-4dae-878e-356534ffe1b6.png)

_______________________________________________________________________________________________________________________________________________________

## Description

Great Expectations is a shared, open standard for data quality. 
It helps data teams eliminate pipeline debt, through data testing, documentation, and profiling.
![image](https://user-images.githubusercontent.com/98338535/153722159-77cc8e8b-1cc6-49c5-b0c6-fbb356172825.png)


## General informations

Great Expectations helps teams save time and promote analytic integrity by offering a unique approach to automated testing:<br>
- Pipeline tests are applied to data (instead of code) and at batch time (instead of compile or deploy time).
Pipeline tests are like unit tests for datasets: <br>
- They help you guard against upstream data changes and monitor data quality.<br> 

##### The website of great expectations technology : 
                        https://greatexpectations.io/case-studies/  
##### Great Expectations has 4 repositories available such as : 
                        https://github.com/great-expectations/great_expectations 
			
*Great Expectations is both a community and an open source project.*<br>

- The community is an inclusive space for data practitioners who want to improve data collaboration, with data quality as an integral component of that discussion.<br>
- The project provides a shared, open standard for data quality, expressed in software.<br>
- They strive for positive impact for individuals, for teams and companies, and for the whole data ecosystem.<br>

##### To learn more about this technology the community had a youtube channel :
                        https://www.youtube.com/c/GreatExpectationsData/videos 
			
This technology is under active development by James Campbell, Abe Gong, Eugene Mandel, Rob Lim, Taylor Miller, with help from many others.<br>

Abe Gong : is a core contributor to the Great Expectations open source library, and CEO and Co-founder at Superconductive.  
 <br>
Abe was Chief Data Officer at Aspire Health, the founding member of the Jawbone data science team, and lead data scientist at Massive Health.

## Main capabilities

With Great Expectations, you can assert what you expect from the data you load and transform, and catch data issues quickly <br>

*Expectations are basically unit tests for your data.*<br>

Not only that, but Great Expectations also creates data documentation and data quality reports from those Expectations.<br>

*Data science and data engineering teams use Great Expectations to:*<br>

- Test data they ingest from other teams or vendors and ensure its validity. <br>
- Validate data they transform as a step in their data pipeline in order to ensure the correctness of transformations.<br>
- Prevent data quality issues from slipping into data products. 

## Available connectors/integrations

Great Expectations works with the tools and systems that you're already using with your data, including:

<table>
	<thead>
		<tr>
			<th colspan="2">Integration</th>
			<th>Notes</th>
		</tr>
	</thead>
	<tbody>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://dev.pandas.io/static/img/pandas.svg" />                                    </td><td style="width: 200px;">Pandas                   </td><td>Great for in-memory machine learning pipelines!</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://spark.apache.org/images/spark-logo-trademark.png" />                             </td><td style="width: 200px;">Spark                    </td><td>Good for really big data.</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://wiki.postgresql.org/images/3/30/PostgreSQL_logo.3colors.120x120.png" />          </td><td style="width: 200px;">Postgres                 </td><td>Leading open source database</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://raw.githubusercontent.com/gist/nelsonauner/be8160f2e576a327bfcde085b334f622/raw/b4ec25dd4d698abdc37e6c1887ec69ddcca1d27d/google_bigquery_logo.svg" /></td><td style="width: 200px;">BigQuery</td><td>Google serverless massive-scale SQL analytics platform</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://upload.wikimedia.org/wikipedia/commons/6/63/Databricks_Logo.png" /></td><td style="width: 200px;">Databricks</td><td>Managed Spark Analytics Platform</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://www.mysql.com/common/logos/powered-by-mysql-167x86.png" />                       </td><td style="width: 200px;">MySQL                    </td><td>Leading open source database</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://www.blazeclan.com/wp-content/uploads/2013/08/Amazon-Redshift-%E2%80%93-11-Key-Points-to-Remember.png" />                 </td><td style="width: 200px;">AWS Redshift             </td><td>Cloud-based data warehouse</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://braze-marketing-assets.s3.amazonaws.com/images/partner_logos/amazon-s3.png" />   </td><td style="width: 200px;">AWS S3                   </td><td>Cloud based blob storage</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://www.snowflake.com/wp-content/themes/snowflake/img/snowflake-logo-blue@2x.png" /> </td><td style="width: 200px;">Snowflake                </td><td>Cloud-based data warehouse</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://raw.githubusercontent.com/apache/airflow/master/docs/apache-airflow/img/logos/wordmark_1.png" /></td><td style="width: 200px;">Apache Airflow           </td><td>An open source orchestration engine</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://www.sqlalchemy.org/img/sqla_logo.png" />                                         </td><td style="width: 200px;">Other SQL Relational DBs </td><td>Most RDBMS are supported via SQLalchemy</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://jupyter.org/assets/logos/rectanglelogo-greytext-orangebody-greymoons.svg" />                                             </td><td style="width: 200px;">Jupyter Notebooks        </td><td>The best way to build Expectations</td></tr>
		<tr><td style="text-align: center; height=40px;"><img height="40" src="https://cdn.brandfolder.io/5H442O3W/as/pl546j-7le8zk-5guop3/Slack_RGB.png" />            </td><td style="width: 200px;">Slack                    </td><td> Get automatic data quality notifications!</td></tr>
	</tbody>
</table>


## ways to deploy Great_Expectations
To see Great Expectations in action on your own data:

- You can install it using pip
```
pip install great_expectations
```
- or conda
```
conda install -c conda-forge great-expectations
```
- and then run
```
great_expectations init
```


#### Deploying Great Expectations with Google Cloud Composer (Hosted Airflow)

These steps are basically following the Deploying Great Expectations with Airflow documentation with some items specific to Google Cloud Composer.
###### Steps

*1-Set up your Composer environment*<br>
*2-Create Expectations*<br>
*3-Create your Data Context*<br>
*4-Create a DAG with Validations*<br>
*5-Upload your Expectations and DAG*<br>
*6-Monitor your deployment*<br>
#### Deploying Great Expectations with Astronomer

###### Steps

*1-Set the DataContext root directory*<br>
*2-Set the environment variables for credentials*<br>

## Reviews
#### Good Reviews

*-Great Expectations is a fast growing tool allowing comprehensive use to ensure data quality for the operation of a machine-learning model. The tool has been developed with special importance attached to providing the most generic possible framework and offering users many interfaces which allow them to adapt Great Expectations to their own project and extend it according to their own needs.*

*-Is an action operator which can automatically generate slack notification after validation. This and other templates can be used to design interfaces to other systems.*

*-There is a great need to take data quality testing into the world of modern data sources and development approaches with the help of a modern tool.*

#### Bad Reviews

*-Great Expectations is not a pipeline execution framework.*

*-Great Expectations is not a data versioning tool.*

*-Great Expectations currently works best in a python/bash environment.*

## Raodmap
After a hiatus of a few months, Great Expectations Community Roadmap Meeting 🕒 Tuesday, June 22n will focus on the roadmap for open source Great Expectations. 
they looking forward to input from the whole community. <br> 

This Roadmap include:<br> 

            - Promote the V3 API (BatchRequest) to primary (done)
            - Improve Docs,esp,onboarding and core skills/Concepts
            - StreamLine ecosystem partnership + eployment patterns
            - Release V3 docs for customs Expectations 
            - Launch and iterate on Expectations Gallery

