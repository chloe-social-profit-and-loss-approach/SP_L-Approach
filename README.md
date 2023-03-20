<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<div align="center">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

</div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://www.chloe.com/">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7c/Chlo%C3%A9_logo.svg/2560px-Chlo%C3%A9_logo.svg.png" alt="Logo" width="160" height="51">
  </a>

  <h3 align="center">Social Profit & Loss Approach</h3>

  <p align="center">
    Women Forward. For a Fairer Future.
    <br />
    <a href="https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://lookerstudio.google.com/u/0/reporting/054e19cc-7ae2-48d4-b1ee-fe6ed73e6a7b/page/p_jdgn2b7auc">View Demo</a>
    ·
    <a href="https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/issues">Report Bug</a>
    ·
    <a href="https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details open>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#build-and-provide-the-gcloud-environment">Build and provide the gcloud environment</a></li>
        <li><a href="#compute-kpis">Compute KPIs</a></li>
        <li><a href="#weighing-rule">Weighing rule</a></li>
      </ul>
    </li>
    <li><a href="#how-to-implement-data-visualization">How to implement Data Visualization</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<div align="center">

[![SP&L Screenshot][product-screenshot]](https://lookerstudio.google.com/u/0/reporting/054e19cc-7ae2-48d4-b1ee-fe6ed73e6a7b/page/p_jdgn2b7auc)

</div>

__The Social Profit & Loss Approach__

At Chloé, we believe that informing strategies and action plans all start with impact measurement. Measuring social impact means gaining a better insight into the potentially positive impacts that organisations can have on their stakeholders throughout their value chains – from raw material extraction to a product’s end of life. This was our rationale for creating the Social Profit & Loss approach (SP&L). The SP&L approach enables organisations to measure, evaluate, and visualise an organisation’s positive impact on their stakeholders, and to draft tailor-made action plans for making immediate and long-term improvements to their own practices as well as their suppliers. 

__Open Source__

Chloé believes transparency is central to advancing industry practices. We have created the SP&L to further the collective discussion around positive social impact. The SP&L methodology and its implementation formats therefore are open sourced.

__Steps__ 

The methodology has five main steps: (1) social auditing and decent practices monitoring as a pre-requisite, (2) potentially positive social performance measurement through a data collection using jotform, (3) data evaluation, (4) data visualization, and (5) a data verification process to consolidate the final results.
The data collection format (url) and evaluation format detailing metrics and calculations rules (url) are available here/on chloe.com(url), as well as the general [Methodology Note and Guidelines](https://www.chloe.com/cloud/chloewp/uploads/2023/03/Chloe_SPL_Methodology.pdf).

Once you have sent the surveys (using jotform) and that the data collection is completed, this github will describe how to clean and automatize data evaluation and visualisation. 
Impact visualisation is instrumental to informing decision-making, and in supporting suppliers when it comes to improving their immediate and long-term social practices. In the methodology, a dashboarding tool, linked to the evaluation tool, provides a multi-level visualisation of positive social impact including the aggregated impact, supplier’s impact and product’s impact. 

<br />

__We have thus created this github to provide insight and an example as to how to :__
1)	Automatize the data evaluation using Jotform and GCP
2)	Go from data collection and evaluation to data visualization

__We encourage highly collaboration and contribution to improve this project according to the needs of the community.__

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### __Built With__

This section list the major frameworks/libraries used to bootstrap the project. 

* [![Google Cloud][Google-Cloud]][Google-Cloud-url]
* [![Looker][Looker]][Looker-url]
* [![Microsoft Excel][Excel]][Excel-url]
* [![Jotform][Jotform]][Jotform-url]


In a first version, the project uses Google Cloud for data storage in BigQuery, calculation of scoring rules with a Google Cloud workflow, visualization of results with Google Cloud Looker.
Microsoft Excel for the processing of form data (Deprecated) and exportation of Submission Form (from JotForm).
Python as a framework to build the cloud function in GCP to export the excel file from a Bucket to a BigQuery table.

The final output of this project is a Dashboard built with Looker Studio where you can explore the result of the social performance measurements process.

#### About Looker Studio:

_Looker Studio is a web-based data modeling and analysis tool that allows users to create, manage, and share interactive data insights and dashboards. It offers a drag-and-drop interface for data modeling, data exploration, and visualization. Looker Studio integrates with various data sources, including databases, data warehouses, and cloud services, to provide a unified view of data. It also allows users to create custom calculations and metrics, and to build complex data models that can be easily understood by both technical and non-technical users._



<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

In order to implement this project in your own Google Cloud infrastructure, this section should cover few examples of how we decided to implement the SP&L project in our infrastructure. 

__However, with the form available and the calculation rules defined, everyone is free to adapt this implementation to their own environment according to their needs and resources.__

### Prerequisites

To implement the project the way it was designed to be, you first need to install Google Cloud SDK on your local machine.
_Follow this link for further information https://cloud.google.com/sdk/docs/install?hl=fr#windows_

Secondly, you need to setup your JotForm account or any other form provider and implements the questions to your survey.

__The survey questions that you need to implement can be found directly in the [Survey Question](https://www.chloe.com/cloud/chloewp/uploads/2023/03/Survey_English.pdf) document.__

### Build and provide the gcloud environment 

_Below is an example of how you can deploy the Google Cloud instances to implement the project in your infrastructure._

1. Export the submission form in XSLX format or CSV from your form provider
2. Create a dedicated project inside your GCP environment
_Follow this link for further information https://cloud.google.com/sdk/gcloud/reference/projects/create_
   ```sh
   gcloud projects create <project-id> --name="Happy project" --labels=type=happy
   ```
4. Create a bucket in your GCP environment and upload the submission form
_Follow this link for further information https://cloud.google.com/storage/docs/creating-buckets?hl=en_
   ```sh
   gcloud storage buckets create gs://<bucket-name>

   gcloud storage cp path/to/submission_form.csv gs://<bucket-name>/
   ```
5. Create a dataset in your BigQuery environment 
_Follow this link for further information https://cloud.google.com/bigquery/docs/datasets?hl=en_
   ```sh
   bq --location=<location-name> mk -d <dataset-name>
   ```
6. Create the table in your dataset to load the submission form with the proper table json schema of your submission

    ⚠️ _In order for the fields (questions from your survey) to be accepted as a field name, it is recommended to reformat to follow the syntax rules for field names in BigQuery. Field names in lower case, no number as a first character, cannot contain spaces or special characters such as "?", "/", "'", "é", "à", "%" etc._ 

    ___Example___: The question `6. Have you formalized and/or implemented an inclusion and/or non-discrimination policy?` in your survey should be reformatted to comply with Google Cloud Platform (GCP) naming conventions when you export your submission form as follows `have_formalized_and_or_implemented_inclusion_non_discrimination_policy`

    _Follow this link for further information https://cloud.google.com/bigquery/docs/schemas#column_names_
      ```sh
      bq mk --table <project-id>:<dataset-name>.<table-name> <path_to_schema_json>
      ```

8. Create a cloud function in Google Cloud Functions to process the submission form and load the data into your BigQuery table automatically
_Follow this link for further information https://cloud.google.com/sdk/gcloud/reference/functions_

    * Configure the cloud function to trigger execution as soon as a file is dropped in the bucket
    ```sh
    gcloud functions deploy <funtion-name> --runtime python37 --trigger-bucket <bucket-name> --entry-point <function-entry-point>
    ```

<details><summary>Cloud function example code</summary>

```python
import logging
import pandas as pd
from google.cloud import storage, bigquery

def load_data_to_bq(event, context):
    """Triggered by a change to a Cloud Storage bucket.
    Extracts data from a new Excel file and loads the data into BigQuery.
    """
    file = event
    bucket_name = file['bucket']
    file_name = file['name']
    destination_table = 'your_dataset.your_table'
    
    # Connect to Google Cloud Storage
    storage_client = storage.Client()
    bucket = storage_client.get_bucket(bucket_name)
    blob = bucket.blob(file_name)
    
    # Read the Excel file into a Pandas DataFrame
    df = pd.read_excel(blob.download_as_string())
    
    # Connect to BigQuery
    bq_client = bigquery.Client()
    table_ref = bq_client.dataset(destination_table).table(destination_table)
    table = bq_client.get_table(table_ref)
    
    # Load the data into BigQuery
    errors = bq_client.insert_rows(table, df.to_dict(orient='records'))
    
    if errors == []:
        logging.info(f'Data loaded to {destination_table}')
    else:
        logging.error(errors)
```
</details>

<br />

### Compute KPIs

_This section covers some example of how you can compute the final KPIs based on the scoring grid definitions in BigQuery SQL._

⚠️ _Please refer to the [Evaluation and Sources Detail](https://www.chloe.com/cloud/chloewp/uploads/2023/02/Chloe-SPL_evaluation-and-sources.xlsx) to implement the scoring notation grid associated to the scoring metrics based on your own implementation._

<br />
<details><summary><b>Scoring metrics</b></summary>
<table>
    <tr>
        <td><b>Maturity level metrics:</td>
        <td>Non existent</td>
        <td>Policy does not exist</td>
    </tr>
      <tr>
        <td></td>
        <td>Formalized</td>
        <td>Policy has been defined / outlined but is not yet fully in place</td>
    </tr>
        <tr>
        <td></td>
        <td>In place</td>
        <td>Policy is fully in place</td>
    </tr>
        <tr>
        <td></td>
        <td>Improvement iterations</td>
        <td>Actions are regularly taken to improve the impact of the policy</td>
    </tr>
        <tr>
        <td></td>
        <td>Reporting</td>
        <td>Impact of the policy is measured and reported on</td>
    </tr>
    <tr>
        <td><b>Representation metrics</td>
        <td>Some metrics cannot be measured the same from country to country. They have been adapted based on local demographics and customs.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Country dependent metrics</td>
        <td>For instance, the population in Madagascar is much younger than in Europe, so the "% of employees 50 or older" should represent this gap.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Coverage metrics:</td>
        <td>Metrics rated from low worker coverage, or 0% (rated 1) to full worker coverage, or 100% (rated 5).</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>This form of evaluation is relevant when it comes to contracts, living wage payment, access to services, and training.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Industry-specific metrics:</td>
        <td>Some metrics require a benchmark from the fashion industry. For the time being we used averages from national data, however this evaluation should be updated after the industry consultation.</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>This is particularly relevant for "Job Quality" and "Know-How" metrics, and gender balance metrics which are specific to the fashion industry.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Binary metrics:</td>
        <td>Some metrics should either be answered by "yes" (rated 5) or "no" (rated 1) as a gradual evaluation would not be relevant.
        </td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>For instance annual meetings or whether publications are in place.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Gradation towards equality metrics:</td>
        <td>Metrics that should reflect the gap (or lack thereof) in practices depending on worker's profile and characteristic (ie gender, age, etc).</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>For instance, the gap between men's and women's salary for a similar job position with similar competences and experiences.</td>
        <td></td>
    </tr>
    <tr>
        <td><b>Gender balance metrics</td>
        <td>For gender representation metrics, we aligned ourselves on both the principle of gender balance (women should represent 50 to 60% of the workforce) and on the specificities of the fashion industry, which has a workforce composed of women in
 majority.</td>
       <td></td>
    </tr>
        <tr>
        <td><b>Specificity and hypothesis</td>
        <td>The metric related to % of the workforce is within the diversity category and is therefore stricter regarding parity, whereas metrics regarding representation in leadership are less strict as the presence of women in leadership (while not extreme,
 up until 90%) is deemed a positive impact.</td>
        <td></td>
    </tr>
        <tr>
        <td></td>
        <td>Those hypothesis will be reconsidered and updated after the industry consultation, as they are industry-specific metrics.</td>
        <td></td>
    </tr>
</table>
</details>
In this section we will provide examples to implement the scoring rules using different types of metrics in BigQuery SQL.

<br />

1. __Maturity level metric__

___Maturity level grid___
__<center>Calculation method</center>__
<table>
    <tr>
        <td>Non existent</td>
        <td>Policy does not exist</td>
    </tr>
      <tr>
        <td>Formalized</td>
        <td>Policy has been defined / outlined but is not yet fully in place</td>
    </tr>
        <tr>
        <td>In place</td>
        <td>Policy is fully in place</td>
    </tr>
        <tr>
        <td>Improvement iterations</td>
        <td>Actions are regularly taken to improve the impact of the policy</td>
    </tr>
        <tr>
        <td>Reporting</td>
        <td>Impact of the policy is measured and reported on</td>
    </tr>
</table>

  * __Question 6__: Have you formalized and/or implemented an inclusion and/or non-discrimination policy?
  * _BigQuery Field: `have_formalized_implemented_inclusion_non_discrimination_policy`_
<details open><summary><i>Deploy to see the code</i></summary>

```sql
------ Maturity level metric example ------
SELECT 
  CASE 
    WHEN have_formalized_implemented_inclusion_non_discrimination_policy = 'Policy does not exist' THEN 1
    WHEN have_formalized_implemented_inclusion_non_discrimination_policy = 'Policy has been defined / outlined but is not yet fully in place' THEN 2
    WHEN have_formalized_implemented_inclusion_non_discrimination_policy = 'Policy is fully in place' THEN 3
    WHEN have_formalized_implemented_inclusion_non_discrimination_policy = 'Actions are regularly taken to improve the impact of the policy' THEN 4
    WHEN have_formalized_implemented_inclusion_non_discrimination_policy = 'Impact of the policy is measured and reported on' THEN 5
  END AS equal_opportunity_policy_or_practices_in_place
    
FROM <project-id>.<dataset-name>.<table-name>
```
</details>
<br />

2. __Representation metric & depends on country__

Some metrics cannot be measured the same from country to country. They have been adapted based on local demographics and customs. 

__<center>Calculation method</center>__

  $${\text{Number of employees [>50]} \over \text{Number of employees}} * 100$$
  * __Question 1:__ Répartition des employés >> Ayant plus de 50 ans >> Nombre total d’employés
  * _BigQuery Field: `employee_distribution_over_50_total_count`, `total_employee_count`_
  * The grade depends on: Country
<details><summary><i>Deploy to see the code</i></summary>

```sql
------ Representation & depends on country example ------
SELECT 
  CASE

    WHEN Country_Code in ('FR') and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 5 or
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 50 THEN 1

    WHEN Country_Code in ('FR') and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 5 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 10 or
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 40 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 50 THEN 2
  
    WHEN Country_Code in ('FR') and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 10 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 15 or
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 30 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 40 THEN 3

    WHEN Country_Code in ('FR') and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 15 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 20 or
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 25 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 30 THEN 4

    WHEN Country_Code in ('FR') and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 20 and
      CAST(employee_distribution_over_50_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 25 THEN 5

    WHEN Country_Code in ('ES') ...
    .
    .
    .

    WHEN Country_Code in ('IT') ...
    .
    .
    .

    WHEN Country_Code in ('RO') ...
    .
    .
    .
  
  END AS percentage_of_employees_who_are_50_years_old_and_older

FROM <project-id>.<dataset-name>.<table-name>
```
</details>
<br />

3. __Coverage metric__

Metrics rated from low worker coverage, or 0% (rated 1) to full worker coverage, or 100% (rated 5). 

__<center>Calculation method</center>__

  $${\text{Workers who are between [19-26] and have a a permanent contract} \over \text{Number of employees [19-26]}} * 100$$
  * Question 2: Permanent contracts >> Between 19 and 26 years old >> Number of employees with permanent contracts 
  * Question 1: Distribution of employees >> Between 19 and 26 years old >> Total number of employees
  * _BigQuery Field: `permanent_contracts_19_to_26_years_old_count`_, `employee_distribution_19_to_26_years_old_total_count`

<details><summary><i>Deploy to see the code</i></summary>

```sql
------ Coverage metric example ------
SELECT 
  CASE
      WHEN CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 <= 50 THEN 1

      WHEN CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 > 50 and
      CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 <= 60 THEN 2

      WHEN CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 > 60 and
      CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 <= 75 THEN 3

      WHEN CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 > 75 and
      CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 <= 90 THEN 4

      WHEN CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 > 90 and
      CAST(permanent_contracts_19_to_26_years_old_count AS INT64) / CAST(employee_distribution_19_to_26_years_old_total_count AS INT64) * 100 <= 100 THEN 5

  END AS Workers_who_are_between_18_26_and_have_a_permanent_contract
    
FROM <project-id>.<dataset-name>.<table-name>
```
</details>
<br />

4. __Industry-specific metric__

Some metrics require a benchmark from the fashion industry. For the time being we used averages from national data, however this evaluation should be updated after the industry consultation. 

__<center>Calculation method</center>__

  $${\text{Number of women} \over \text{Number of employees}} * 100$$
  * Question 2: Distribution of employees >> Who are women >> Total number of employees
  * _BigQuery Field: `employee_distribution_female_total_count`_, `total_employee_count`
<details><summary><i>Deploy to see the code</i></summary>

```sql
------ Industry-specific metric example ------
SELECT 
  CASE 
    WHEN 
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 20 or  
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 > 96 THEN 1

    WHEN 
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 20 and  
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 30  or
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 90 and
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 <= 96 THEN 2

    WHEN 
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 30 and  
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 40  or
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 75 and
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 90 THEN 3

    WHEN 
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 40 and  
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 45  or
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 60 and
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 < 75 THEN 4

    WHEN
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 >= 50 and  
      CAST(employee_distribution_female_total_count AS INT64) / CAST(total_employee_count AS INT64) * 100 <= 60 THEN 5
  
  END AS Percentage_of_women_in_total_workforce 

FROM <project-id>.<dataset-name>.<table-name>
```
</details>
<br />

5. __Gradation towards equality metric__

Metrics that should reflect the gap (or lack thereof) in practices depending on worker's profile and characteristic (ie gender, age, etc).

_For instance, the gap between men's and women's salary for a similar job position with similar competences and experiences._

__<center>Calculation method</center>__

  $${\text{Average men managers salary} - \text{Average women managers salary} \over \text{Average men managers salary}}$$
  * Question 5B: Equal Pay - Middle and Senior Management >> Average for men >> Gross salary per management employee
  * Question 5C: Equal Pay - Middle and Senior Management >> Average for women >> Gross salary per management employee
  * _BigQuery Field: `salary_equality_male_mid_level_managers_average_gross_salary`_, `salary_equality_female_mid_level_managers_average_gross_salary`

<details><summary><i>Deploy to see the code</i></summary>

```sql
------ Gradation towards equality metric example ------
SELECT 
  CASE
    WHEN 
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) >= 15 then 1

    WHEN 
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) >= 10 and
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) <= 15 then 2

    WHEN 
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) >= 1 and
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) <= 10 then 3

    WHEN 
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) < 1  then 4

    WHEN 
      CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) - CAST(salary_equality_female_mid_level_managers_average_gross_salary AS INT64) / CAST(salary_equality_male_mid_level_managers_average_gross_salary AS INT64) = 0 then 5

  END AS Gap_from_pay_equality_based_on_gender_in_perc_in_management

FROM <project-id>.<dataset-name>.<table-name>
```
</details>
<br />

__ℹ️ All the calculation methods, scoring grids, scoring metrics and descriptions are well documented in the [Evaluation and Sources Detail](https://www.chloe.com/cloud/chloewp/uploads/2023/02/Chloe-SPL_evaluation-and-sources.xlsx)__

### Weighing rule

Each KPIs are part of a ___category___. 
Inside each ___category___, the grade is calculated as the average of the grades of this ___category___. 

__The overall grade is calculated as the average of all twelve categories, with the two categories "living wage" and "gender equality" weighing twice as much in the final agreggated score.__

$${\text{AVG}(\text{all categories except living wage and gender equality}) * 10 + (2 * \text{living wage grade}) + (2 * \text{gender equality grade}) \over 14} $$

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## How to implement Data Visualization

The purpose of the visualization process is to guide decision-making towards optimization at both lifecycle and value chain levels. Once the data is completed on the digital survey form, the social data is directly evaluated and automatically translated visually on a dashboard:

-	At the headquarters or operations level
-	At the supplier level
-	At the product level 

The initial SP&L version mobilizes Google Cloud Platform (GCP), a BI & analytics serving dashboards for in-depth, consistent analysis in order to avoid mistakes and provide a consistent analysis. GCP allows a real-time data processing, and constitutes an essential step in the visualization process. An Excel file for input/output file in an effort to harmonize and centralize all feedback and SP&L results from operations and suppliers.

While the SP&L does not cover decent working conditions itself through the process, but focuses on positive impacts, the visualization includes audit score at every level: organization and product through the completion on GCP or any social risk information or auditing information. 

The visualization offers a granularity : 
-	Audit score covering decent working conditions
-	Overall performance score (aggregated)
-	Score per impact category
-	Score per metrics, with best practices and necessary improvement showcased.

Other direct available information are: the number of workers mobilized by collection, the number of workers mobilized by product reference (in average), and a List of references the supplier has worked on – and _link_ to access the visualization per product reference.

__Through the first version of the SP&L approach was created a visualization tool which synthesizes essential elements for decision-making and optimization, by creating the basis for a multicriteria performance scoreboard, including certifications et audit scores, to facilitate access, reporting and accounting. 
Please find below an example of the representation of the organizations and product scorecards.__ 

<br />
<div align="center">

![dashboard-screenshot](https://i.ibb.co/W3z2xkD/spnl-visual-1.png)

Organization or product site dashboard – _anonymized example_

![dashboard-screenshot](https://i.ibb.co/2nngV26/spnl-visual-2.png)

Product dashboard – _anonymized example_
</div>

___ℹ️ You can develop your own scoring dashboard based on the template [Dashboard Looker](https://lookerstudio.google.com/u/0/reporting/054e19cc-7ae2-48d4-b1ee-fe6ed73e6a7b/page/p_jdgn2b7auc). You can simply `create a copy` of the dashboard and connect it to your aggregated result table.___

_⚠️ Don't forget to refer to the official documentation of Looker if you want more technical information on how to connect the dashboard to your BigQuery Table [Quick start with Looker Studio](https://cloud.google.com/bigquery/docs/bi-engine-looker-studio?hl=fr)._

<!-- USAGE EXAMPLES -->
## Usage

In terms of use, integrated into reporting and accounting, the SP&L approach insights are meant to better inform and facilitate decision-making when it comes to resource allocation, targeted investment for operations, and capacity-building within the supply chain. By facilitating the systematic access to quantified positive social performance data which can be compared and monitored over time, the SP&L provides useful insights for decision-making, valuable and valuated when included in an investment and resource allocation analysis. In that way, the SP&L approach provides a different take on Social Return on Investment (SROI) by creating the necessary and direct basis for a social investment efficiency analysis, resource allocation optimization evaluation and forecasts. 


__The approach directly enables:__

-	The integration of new performance criteria into fully quantified performance reviews of activities, collections and products
-	A systematized resource allocation optimization and maximization analysis, assessing and anticipating the efficiency of resources. The SP&L approach facilitates the assessment of the efficiency of resources allocation through monitoring performance results, directly and over time, and systematically relinking social value creation to investment efficiency.


__Data collected can be useful:__

-	For certification process such as B Corp
-	As the basis for monitoring supplier social practices, capacity-building and creating improvement plans for suppliers 
-	As a basis for social investment efficiency analysis (monitoring changes in social performance over time whenever resources are allocated)
-	Within product optimization analysis


__Taking action:__

The aim with the SP&L was to provide additional insight for decision-making and to better accompany change within our supply chain. 
In that way, the steps to take after visualization are the following:
(1)	Communicate key information and results to suppliers
(2)	Define a capacity-building plan based on SP&L KPI with suppliers
(3)	Monitor change and organize yearly evolution monitoring
(4)	Train internal teams to ancitipate data collection, monitoring, and discussion with suppliers. 


_For more examples, please refer to the [Methodology Note and Guidelines](https://www.chloe.com/cloud/chloewp/uploads/2023/03/Chloe_SPL_Methodology.pdf)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

The SP&L approach is by nature exploratory and evolutive. It is intrinsically meant to evolve over time as socio-economic situation by country, regulations, but also industry standards regarding social impact evolve. Living wage, which is one of the key item measured in this methodology, has not yet a single international recognized standard. 

The methodology will be regularly updated. Other key topics which we aim to include in a future iteration of the methodology are value sharing, value distribution and value redistribution which we aim to include in a “value chain partners” new stakeholder category. Further, current progress in traceability will more than likely further the possibilities to get additional insight and better manage positive social impact within supply chains. We hope this leads to a systemization of performance measurement and monitoring in the longer run. 

The creation of the SP&L approach created an opportunity to discuss best practices at the industry level related to social impact. As these discussion continue, we hope and anticipate that they will also contribute to ambitiously move the needle. We welcome change, progress and conversation to continue this journey together. Please do not hesitate to contact as sustainability@chloe.com 


See the [open issues](https://github.com/Chloe-social-profit-and-loss-approach/SP_L-Approach/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. We are always open to contributions to improve the SP&L project. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Chloé is a company that has always acted in favor of equality.
We aim to foster a community where people of all genders, ethnicities, social backgrounds, sexual orientations, ages and disabilities - visible and invisible - to make participation in our project and our community.
  
Therefore, you are requested to follow the code of conduct at [CODE_OF_CONDUCT.md](https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/blob/main/CODE_OF_CONDUCT.md) while contributing to the project 😄
  
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the GNU AGPLv3 License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

* Mathilde Asseman - [@MathildeAsseman](https://github.com/MathildeAsseman) - mathilde.asseman@chloe.com
* Numan Sahnou - [@NumanSahnou](https://github.com/NumanSahnou) - numan.sahnou@chloe.com
* Adin Hrelja - [@AdinHrelja](https://github.com/AdinHrelja) - adin.hrelja@chloe.com

Project Link: [https://github.com/Chloe-social-profit-and-loss-approach/SP_L-Approach/](https://github.com/Chloe-social-profit-and-loss-approach/SP_L-Approach/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

The SP&L approach is a collaborative effort as well as a discussion, and Chloé would like to thank all the experts and organizations which reviewed and/or participated to the essential industry consultation for the tool. In that way, we would like to acknowledge the essential work done by Kering on the pioneering EP&L methodology, without which there would be no SP&L approach. 

We would like to thank the Sustainable team at PwC France for reviewing the methodology, and the Fédération de la Mode et de la Haute Couture for coordinating the Industry Consultation that took place in 2022, and Textile Exchange for facilitating the conversation with other industry collaborators and experts. 

A warm thank you also to our academic partners, the Insitut Français de la Mode (IFM) and the Conservatoire National des Arts et Métiers (CNAM) for providing crucial insights throughout the development process for the SP&L approach methodology. 

Thank you to Elevate for providing essential insights when it comes to the data verification process and its deployment. 

Thank you to the numereous experts who shared essential insights, and a specific thank you to Philippe Aghion (Collège de France), Caterina Occhio (SeeMe), and Erinch Sahan (Doughnut economics action lab) for their continuous feedbacks. 

Internally, the conception and deployment of the tool united our Sustainability, IT and Operations Departments who made crucial efforts into making the SP&L come to life.

_This list is non-exhaustive and we hope to keep the conversation regarding the measurement, evaluation and visualization of social impact going_


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/chloe-social-profit-and-loss-approach/SP_L-Approach.svg?style=for-the-badge
[contributors-url]: https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/chloe-social-profit-and-loss-approach/SP_L-Approach.svg?style=for-the-badge
[forks-url]: https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/network/members
[stars-shield]: https://img.shields.io/github/stars/chloe-social-profit-and-loss-approach/SP_L-Approach.svg?style=for-the-badge
[stars-url]: https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/stargazers
[issues-shield]: https://img.shields.io/github/issues/chloe-social-profit-and-loss-approach/SP_L-Approach.svg?style=for-the-badge
[issues-url]: https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/issues
[license-shield]: https://img.shields.io/github/license/chloe-social-profit-and-loss-approach/SP_L-Approach.svg?style=for-the-badge
[license-url]: https://github.com/chloe-social-profit-and-loss-approach/SP_L-Approach/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/company/chloe/
[product-screenshot]: https://i.postimg.cc/3Jg14ybr/spl-visuel-front.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/

[Google-Cloud]: https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white
[Google-Cloud-url]: https://cloud.google.com/

[Excel]: https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white
[Excel-url]: https://www.microsoft.com/fr-fr/microsoft-365/excel

[Python]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[Python-url]: https://www.python.org/

[Looker]: https://img.shields.io/badge/Looker-4285F4?logo=looker&logoColor=fff&style=for-the-badge
[Looker-url]: https://www.looker.com/

[Jotform]: https://img.shields.io/static/v1?label=%20Jotform&message=%20&color=555555&logo=data:image/png;base64,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&style=for-the-badge
[Jotform-url]: https://www.jotform.com/


[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/

[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
