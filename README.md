```sql
dhruv@melbourne:~$ psql -d career_prod -c "SELECT role, focus, location, work_rights FROM profile;"

             role              |                 focus                  |   location    |         work_rights          
-------------------------------+----------------------------------------+---------------+------------------------------
 Data & Systems Engineer       | ETL Pipelines, SQL, BI & Cloud Systems | Melbourne, AU | Full Working Rights (485)
(1 row)
```

### Hey, I'm Dhruv.

I'm a Computer Science graduate from Deakin University (Data Science major, Distinction) and currently work as an **AI & Data Systems Administrator** at **Natural Velocity** in Docklands, Melbourne.

Most of my work sits between pulling messy data out of external APIs, modelling it cleanly in PostgreSQL or Snowflake, building Power BI and Tableau views for decision-makers, and keeping production systems and client networks running smoothly.

* **Current day-to-day:** Hybrid cloud & network administration, Datto pipeline monitoring, HubSpot & GitLab Kanban operations (supporting The District Docklands), and Python/SQL data prep.
* **Core stack:** `Python` `SQL (PostgreSQL / PostGIS / MySQL)` `dbt` `Snowflake` `Power BI` `Tableau` `AWS` `Git`
* **Outside of tech:** Middle-order batsman for Deakin University at the Australian University Nationals Cricket Championships.
* **Links:** [Portfolio Website](https://dhruv-surti.github.io/) · [LinkedIn](https://www.linkedin.com/in/dhruv-surti-73b782390/) · [youhavereacheddhruv@gmail.com](mailto:youhavereacheddhruv@gmail.com)

<br>

### Selected Engineering & Analytics Work

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/dhruv-surti/Residential-Energy-Analytics-Margin-Assurance">Residential Energy Analytics & Margin Assurance</a></h4>
      <a href="https://github.com/dhruv-surti/Residential-Energy-Analytics-Margin-Assurance">
        <img src="https://dhruv-surti.github.io/final_dashboard.png" alt="Residential Energy Analytics Dashboard" width="100%">
      </a>
      <p><sub><b>SQL (MySQL) · Excel Financial Modelling · Tableau</b></sub></p>
      <p>Simulated power usage and tariff margins across 10,000 Australian households. Resolved 150 data anomalies in SQL, modelled plan economics in Excel, and built an executive Tableau view comparing EV, Solar, and Standard tariffs ($218K revenue analysed).</p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/dhruv-surti/coles-sales-dashboard">Coles Retail Sales Performance Dashboard</a></h4>
      <a href="https://github.com/dhruv-surti/coles-sales-dashboard">
        <img src="https://dhruv-surti.github.io/coles_dashboard.png" alt="Coles Sales Performance Dashboard" width="100%">
      </a>
      <p><sub><b>Power BI · DAX · Power Query · Star Schema</b></sub></p>
      <p>Store-level performance dashboard tracking $28,577M in gross sales, revenue per staff member, and forecast-vs-actual variance across six Australian states over two quarters so regional managers can spot underperforming stores quickly.</p>
    </td>
  </tr>
</table>

<br>

### Data Pipelines, Systems & Research Repositories

| Project & Repository | Stack | What I Built & Why It Matters |
| :--- | :--- | :--- |
| **[clinical-data-pipeline](https://github.com/dhruv-surti/clinical-data-pipeline)** | `Python` `PostgreSQL` `dbt` `psycopg2` | Pulls live clinical trial records from the ClinicalTrials.gov REST API (v2), flattens nested JSON with safe null defaults, and runs transactional `ON CONFLICT DO UPDATE` upserts with 4 automated dbt test suites. |
| **FireFusion Spatial Data Platform** *(Deakin Capstone Lead)* | `Python` `PostGIS` `Supabase` `Git` | Led a 17-person data engineering stream. Built 3 automated ETL pipelines unifying 500,000+ BOM and NASA records into a Hub-and-Spoke spatial-temporal database, cutting query response times by ~40%. |
| **[NVIDIA-Brev-Code-Portal](https://github.com/dhruv-surti/NVIDIA-Brev-Code-Portal)** | `Apps Script` `JS` `HTML/CSS` | Live QR credential lookup system built for a 40+ attendee NVIDIA developer workshop. Switched from dynamic claiming to deterministic pre-assigned lookups to eliminate concurrency race conditions (0 failed lookups). |
| **[bushfire-tweet-domain-shift-nlp](https://github.com/dhruv-surti/bushfire-tweet-domain-shift-nlp)** | `Python` `PyTorch` `RoBERTa` | ACM `sigconf` research paper (graded High Distinction) comparing 6 model families on Australian bushfire emergency tweets. Fine-tuned RoBERTa (0.886 F1) beat a zero-shot 1.3B LLM. |

<br>

<details>
<summary><b>Engineering notes: how I design pipelines and systems (click to expand)</b></summary>
<br>

* **Idempotency first:** Pipelines fail in production. In [`clinical-data-pipeline`](https://github.com/dhruv-surti/clinical-data-pipeline), every load uses primary-key conflict resolution (`ON CONFLICT (nct_id) DO UPDATE`) and raw JSON snapshots so re-running a job never duplicates rows or corrupts state.
* **Defensive parsing over silent bad data:** Public APIs often omit fields (like missing enrollment counts in observational trials). Rather than coalescing missing integers to `0` and skewing downstream averages, my extraction scripts preserve explicit `NULL` states and validate boundaries in dbt.
* **Spatial-temporal alignment at scale:** In **FireFusion**, joining raw coordinates from fire, weather, terrain, and vegetation feeds caused slow queries and misaligned points. Designing a universal `Location_Registry` (60 Victorian grid cells) and `Time_Registry` (7,320 hourly periods) with a custom Python `GridSnapper` utility cut query latency by ~40% and allowed 78,691 MVP rows to pass validation with zero dropped records.
* **Operational discipline:** At **Natural Velocity**, every support and infrastructure change for internal networks and external clients runs through scoped GitLab Kanban checklists and strict zero-secrets hygiene.

</details>
