<div align="center">

  <h1>DHRUV SURTI</h1>
  <p><b>Bachelor of Computer Science (Major in Data Science) | Deakin University</b></p>
  <p>Melbourne, Victoria, Australia</p>

  <p>
    <a href="https://dhruv-surti.github.io/">
      <img src="https://img.shields.io/badge/PORTFOLIO-dhruv--surti.github.io-0F4C81?style=for-the-badge&labelColor=0F172A" alt="Portfolio Website" />
    </a>
    <a href="https://www.linkedin.com/in/dhruv-surti-73b782390/">
      <img src="https://img.shields.io/badge/LINKEDIN-DHRUV_SURTI-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0F172A" alt="LinkedIn" />
    </a>
    <a href="https://github.com/dhruv-surti">
      <img src="https://img.shields.io/badge/GITHUB-dhruv--surti-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=0F172A" alt="GitHub" />
    </a>
    <a href="mailto:youhavereacheddhruv@gmail.com">
      <img src="https://img.shields.io/badge/EMAIL-youhavereacheddhruv%40gmail.com-0D7A5F?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0F172A" alt="Email" />
    </a>
  </p>

</div>

<hr />

### ABOUT ME

Computer Science graduate from Deakin University with a High Distinction average across all final-year subjects. I build software systems, scalable cloud deployments, automated data pipelines, and interactive analytics dashboards across Python, C#, SQL, Snowflake, and AWS.

* **Current Work:** Part-time AI and Data Systems Engineer at **Natural Velocity** (Docklands, Melbourne), preparing domain datasets for local LLMs on NVIDIA Spark servers, maintaining cloud and server infrastructure, and managing corporate IT support for The District Docklands.
* **Capstone Leadership:** Directed a 17-member data engineering team for the **FireFusion** Victorian bushfire forecasting platform at Deakin University, designing a 60-cell spatial-temporal schema in Supabase and a unified Python ETL pipeline aligning 78,691 fire, weather, and vegetation records.
* **Applied ML Research:** Authored an ACM-formatted NLP research paper benchmarking six machine learning model families on emergency bushfire tweets, achieving a **0.886 F1 score** with a fine-tuned RoBERTa transformer.
* **Athletics:** Represented Deakin University in cricket at the 2024 UniSport Nationals tournament.

<hr />

### FEATURED REPOSITORIES AND TECHNICAL WORK

#### 1. Data Pipelines and Business Intelligence

<table>
  <thead>
    <tr>
      <th width="32%" align="left">Repository</th>
      <th width="46%" align="left">Architecture and Implementation</th>
      <th width="22%" align="left">Key Outcomes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/sme-funding-pipeline">sme-funding-pipeline</a></b><br />
        <sub><code>Python</code> <code>Fivetran</code> <code>Snowflake Dynamic Tables</code></sub>
      </td>
      <td>
        End-to-end ELT pipeline extracting historical AusTender government contract files from the data.gov.au API, cleaning <code>cp1252</code> streams in Python, syncing via Fivetran every 6 hours, and transforming into 3 SME loan tiers using Snowflake Dynamic Tables.
      </td>
      <td>
        6-hour automated sync<br />
        1-hour lag Dynamic Tables<br />
        3 SME lending tiers
      </td>
    </tr>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/clinical-data-pipeline">clinical-data-pipeline</a></b><br />
        <sub><code>Python</code> <code>PostgreSQL</code> <code>dbt</code> <code>REST API</code></sub>
      </td>
      <td>
        Engineered live JSON ingestion from the ClinicalTrials.gov REST API (v2) using transactional PostgreSQL upserts (<code>ON CONFLICT DO UPDATE</code>) and dbt staging/mart models.
      </td>
      <td>
        Idempotent re-runs<br />
        4 automated dbt test suites
      </td>
    </tr>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/Residential-Energy-Analytics-Margin-Assurance">Residential-Energy-Analytics-Margin-Assurance</a></b><br />
        <sub><code>MySQL</code> <code>Excel</code> <code>Tableau</code></sub>
      </td>
      <td>
        Modelled grid power consumption across Australian households in MySQL, remediated data quality anomalies via SQL, and built an Excel and Tableau tariff margin model.
      </td>
      <td>
        10,000 households<br />
        $218K billings modelled<br />
        150 SQL fixes
      </td>
    </tr>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/coles-sales-dashboard">coles-sales-dashboard</a></b><br />
        <sub><code>Power BI</code> <code>DAX</code> <code>Power Query</code></sub>
      </td>
      <td>
        Architected a Star Schema dimensional model across 6 Australian states to evaluate store-level gross sales, team productivity, and quarterly target variance.
      </td>
      <td>
        $28.5M retail revenue<br />
        6 states tracked<br />
        2 quarters analysed
      </td>
    </tr>
  </tbody>
</table>

#### 2. Software, Cloud Infrastructure, and Applied AI

<table>
  <thead>
    <tr>
      <th width="32%" align="left">Project / Repository</th>
      <th width="46%" align="left">Architecture and Implementation</th>
      <th width="22%" align="left">Key Outcomes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/bushfire-tweet-domain-shift-nlp">bushfire-tweet-domain-shift-nlp</a></b><br />
        <sub><code>Python</code> <code>PyTorch</code> <code>Hugging Face</code> <code>RoBERTa</code></sub>
      </td>
      <td>
        Benchmarked 6 machine learning model families to classify actionable bushfire tweets versus noise under domain shift. Fine-tuned a RoBERTa transformer in PyTorch.
      </td>
      <td>
        0.886 F1 score<br />
        Outperformed 1.3B zero-shot LLM<br />
        High Distinction
      </td>
    </tr>
    <tr>
      <td>
        <b><a href="https://github.com/dhruv-surti/NVIDIA-Brev-Code-Portal">NVIDIA-Brev-Code-Portal</a></b><br />
        <sub><code>JavaScript</code> <code>Apps Script</code> <code>HTML/CSS</code></sub>
      </td>
      <td>
        Built an instant credential lookup web application for a live NVIDIA developer workshop, replacing dynamic claims with deterministic pre-assigned QR lookups.
      </td>
      <td>
        40+ live attendees<br />
        Zero race conditions<br />
        100% event uptime
      </td>
    </tr>
    <tr>
      <td>
        <b>Cloud Scaling, Load Balancing &amp; Docker Deployment</b><br />
        <sub><code>AWS EC2</code> <code>ELB</code> <code>CloudWatch</code> <code>Docker</code> <code>Node.js</code></sub>
      </td>
      <td>
        Deployed containerised Node.js web servers on AWS EC2 with custom machine image templates, Elastic Load Balancing across instances, and CloudWatch throughput monitoring.
      </td>
      <td>
        Multi-instance scaling<br />
        Containerised rollout<br />
        Stress-tested metrics
      </td>
    </tr>
    <tr>
      <td>
        <b>Query Optimization &amp; Data Structures in C#</b><br />
        <sub><code>C#</code> <code>.NET</code> <code>Data Structures</code> <code>Algorithms</code></sub>
      </td>
      <td>
        Coded custom indexing and search structures (Skip-Lists, Heaps, and Stacks) in C# and evaluated range-query caching to replace full-list scans.
      </td>
      <td>
        Logarithmic O(log n) &amp; constant O(1) lookups
      </td>
    </tr>
  </tbody>
</table>

<hr />

### TECHNICAL STACK

<table>
  <tbody>
    <tr>
      <td width="28%"><b>Languages &amp; Core CS</b></td>
      <td width="72%">
        <img src="https://img.shields.io/badge/Python-0F172A?style=flat-square&logo=python&logoColor=38BDF8" alt="Python" />
        <img src="https://img.shields.io/badge/C%23-0F172A?style=flat-square&logo=csharp&logoColor=A855F7" alt="C#" />
        <img src="https://img.shields.io/badge/SQL-0F172A?style=flat-square&logo=postgresql&logoColor=38BDF8" alt="SQL" />
        <img src="https://img.shields.io/badge/JavaScript-0F172A?style=flat-square&logo=javascript&logoColor=FACC15" alt="JavaScript" />
        <img src="https://img.shields.io/badge/Node.js-0F172A?style=flat-square&logo=nodedotjs&logoColor=22C55E" alt="Node.js" />
        <img src="https://img.shields.io/badge/React-0F172A?style=flat-square&logo=react&logoColor=38BDF8" alt="React" />
        <img src="https://img.shields.io/badge/OOP_%26_Data_Structures-0F172A?style=flat-square" alt="OOP and Data Structures" />
      </td>
    </tr>
    <tr>
      <td><b>Data Engineering &amp; Pipelines</b></td>
      <td>
        <img src="https://img.shields.io/badge/Fivetran-0F172A?style=flat-square&logo=fivetran&logoColor=38BDF8" alt="Fivetran" />
        <img src="https://img.shields.io/badge/dbt-0F172A?style=flat-square&logo=dbt&logoColor=FF694B" alt="dbt" />
        <img src="https://img.shields.io/badge/Apache_Spark-0F172A?style=flat-square&logo=apachespark&logoColor=F97316" alt="Apache Spark" />
        <img src="https://img.shields.io/badge/Apache_Airflow-0F172A?style=flat-square&logo=apacheairflow&logoColor=38BDF8" alt="Airflow" />
        <img src="https://img.shields.io/badge/Apache_Kafka-0F172A?style=flat-square&logo=apachekafka&logoColor=white" alt="Kafka" />
        <img src="https://img.shields.io/badge/Hadoop-0F172A?style=flat-square&logo=apachehadoop&logoColor=FACC15" alt="Hadoop" />
        <img src="https://img.shields.io/badge/pandas-0F172A?style=flat-square&logo=pandas&logoColor=38BDF8" alt="pandas" />
        <img src="https://img.shields.io/badge/NumPy-0F172A?style=flat-square&logo=numpy&logoColor=38BDF8" alt="NumPy" />
        <img src="https://img.shields.io/badge/REST_APIs-0F172A?style=flat-square" alt="REST APIs" />
      </td>
    </tr>
    <tr>
      <td><b>Databases &amp; Warehousing</b></td>
      <td>
        <img src="https://img.shields.io/badge/Snowflake_(Dynamic_Tables)-0F172A?style=flat-square&logo=snowflake&logoColor=38BDF8" alt="Snowflake" />
        <img src="https://img.shields.io/badge/PostgreSQL-0F172A?style=flat-square&logo=postgresql&logoColor=38BDF8" alt="PostgreSQL" />
        <img src="https://img.shields.io/badge/PostGIS-0F172A?style=flat-square" alt="PostGIS" />
        <img src="https://img.shields.io/badge/Supabase-0F172A?style=flat-square&logo=supabase&logoColor=10B981" alt="Supabase" />
        <img src="https://img.shields.io/badge/MySQL-0F172A?style=flat-square&logo=mysql&logoColor=38BDF8" alt="MySQL" />
      </td>
    </tr>
    <tr>
      <td><b>Cloud, DevOps &amp; Systems</b></td>
      <td>
        <img src="https://img.shields.io/badge/AWS_(EC2,_ELB,_S3,_RDS,_CloudWatch)-0F172A?style=flat-square&logo=amazonaws&logoColor=F97316" alt="AWS" />
        <img src="https://img.shields.io/badge/Docker-0F172A?style=flat-square&logo=docker&logoColor=38BDF8" alt="Docker" />
        <img src="https://img.shields.io/badge/Kubernetes-0F172A?style=flat-square&logo=kubernetes&logoColor=38BDF8" alt="Kubernetes" />
        <img src="https://img.shields.io/badge/NVIDIA_Spark_Servers-0F172A?style=flat-square&logo=nvidia&logoColor=22C55E" alt="NVIDIA Spark" />
        <img src="https://img.shields.io/badge/GitHub-0F172A?style=flat-square&logo=github&logoColor=white" alt="GitHub" />
        <img src="https://img.shields.io/badge/GitLab-0F172A?style=flat-square&logo=gitlab&logoColor=F97316" alt="GitLab" />
        <img src="https://img.shields.io/badge/HubSpot_Help_Desk-0F172A?style=flat-square&logo=hubspot&logoColor=F97316" alt="HubSpot" />
      </td>
    </tr>
    <tr>
      <td><b>Machine Learning &amp; Analytics</b></td>
      <td>
        <img src="https://img.shields.io/badge/PyTorch-0F172A?style=flat-square&logo=pytorch&logoColor=EF4444" alt="PyTorch" />
        <img src="https://img.shields.io/badge/Hugging_Face_(RoBERTa)-0F172A?style=flat-square&logo=huggingface&logoColor=FACC15" alt="Hugging Face" />
        <img src="https://img.shields.io/badge/Power_BI_(DAX)-0F172A?style=flat-square&logo=powerbi&logoColor=FACC15" alt="Power BI" />
        <img src="https://img.shields.io/badge/Tableau-0F172A?style=flat-square&logo=tableau&logoColor=38BDF8" alt="Tableau" />
        <img src="https://img.shields.io/badge/Streamlit-0F172A?style=flat-square&logo=streamlit&logoColor=EF4444" alt="Streamlit" />
        <img src="https://img.shields.io/badge/Plotly-0F172A?style=flat-square&logo=plotly&logoColor=38BDF8" alt="Plotly" />
        <img src="https://img.shields.io/badge/Excel_Financial_Modelling-0F172A?style=flat-square" alt="Excel" />
      </td>
    </tr>
  </tbody>
</table>

<hr />

### EDUCATION AND VERIFIED CREDENTIALS

* **Bachelor of Computer Science (Major in Data Science)** | Deakin University (Jul 2023 to Sep 2026)
  * Achieved a **High Distinction** average across all final-year university subjects.
* **Anthropic:** Certificate of Completion in Claude Code 101 (`ID: ipd5akt2uc2j`) and Introduction to Claude Cowork (`ID: kouhf8ugmdae`)
* **Industry Simulations:** Quantium Data Analytics (`ID: YuEYhaTYGvYteqeAt`), Commonwealth Bank Intro to Data Science (`ID: Rwp63Qm38kGoyavjv`), and Deloitte Australia Data Analytics (`ID: pvLDiTzpYxhymApat`)
* **Additional Training:** LinkedIn Data Engineering Foundations, Non-Technical Skills of Effective Data Scientists, and Kaggle Python, Data Cleaning & Visualisation (5 Courses)
