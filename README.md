# Adrian Malong

**Senior Data Engineer | Data Platform Engineering**

Calgary, AB | apmalong@gmail.com

## Professional Summary

- Senior Data Engineer with 19+ years of experience building and operating production data platforms, from legacy SQL Server ETL through modern cloud-native lakehouse and warehouse architectures on AWS and Snowflake.
- Deep experience in multi-tenant platform architecture and tenant data isolation, data warehouse/lakehouse migration, data governance and access control, cloud cost optimization (FinOps), and AI-enabled data infrastructure.
- Core stack: Python, SQL, T-SQL; Airflow/MWAA, dbt, Apache Iceberg, Snowflake, Redshift; AWS (S3, Glue Data Catalog, Athena, Lake Formation, EventBridge, Lambda, ECS Fargate); Terraform/Terragrunt.
- Partners directly with engineering leadership and QA to take initiatives from architecture through rollout, including co-designing data models with senior leadership and leading a phased pre-production rollout across 40+ tenants.
- Mentors eight junior and intermediate engineers, has owned architecture for every major data platform migration at StellarAlgo since 2022, and led FinOps work that cut primary AWS production spend from roughly $100K/month to $50K/month.

## Technical Skills

- **Cloud & Data Platforms:** AWS, Snowflake, Amazon S3, Athena, Glue Data Catalog, Redshift, Lake Formation, DynamoDB, EventBridge, Lambda
- **Data Engineering:** Apache Airflow, Amazon MWAA, dbt, Apache Iceberg, PySpark, AWS Glue, ECS Fargate, Parquet, ETL/ELT, incremental processing, dimensional modeling
- **Programming / DevOps:** Python, SQL, T-SQL, PowerShell, Terraform, Terragrunt, GitHub Actions, Docker, CI/CD
- **Architecture & Operations:** Multi-tenant data platforms, medallion architecture, data governance, RBAC, SLOs, observability, OpenTelemetry, FinOps, cost attribution
- **AI & Analytics:** Model Context Protocol (MCP), Amazon Bedrock, Snowflake Cortex, Power BI, Tableau, SSRS, SSIS, SSAS

## Professional Experience

### StellarAlgo | Senior Data Engineer | March 2022 - Present

**Legacy SQL Server ETL & Data Warehouse Maintenance** _(Mar 2022 - Jun 2022)_
- Maintained and resolved defects in StellarAlgo's existing SQL Server ETL and data warehouse while ramping up on the broader data platform.

**Redshift/EventBridge Data Warehouse Migration ("DLH")** _(Q3 2022 - Q3 2023)_
- As sole infrastructure engineer, migrated the legacy SQL Server warehouse to an EventBridge-driven, serverless Redshift architecture, provisioning an isolated Redshift instance per client to enforce tenant separation.
- Partnered directly with the Director of Data to design the underlying data models, translating business reporting requirements into production dimensional schemas.

**Single-Tenant Platform Migration** _(Q4 2023 - Q1 2024)_
- As sole developer, migrated a customized, feature-limited branch of "Kernel" (StellarAlgo's Airflow/MWAA, Glue Data Catalog, S3, and Athena-based ELT platform) into an isolated AWS account for a $600K/year client requiring full data separation from other tenants.
- Scoped the customization to run on roughly $25K/year in infrastructure costs with only about 4 hours per month of ongoing data engineering support, well below the overhead of a standard multi-tenant deployment.

**Glue PySpark Ingestor** _(Q1 2024 - Q2 2024)_
- Replaced an underperforming Python-based ingestor with a PySpark job on AWS Glue after it proved too slow for the client's initial historical load, enabling ingestion of 5B+ rows into Kernel within a practical timeframe.

**Kernel Platform Operations** _(Q3 2024 - Q2 2025)_
- Joined the Kernel platform team to support day-to-day operations of StellarAlgo's core Airflow/MWAA, Glue Data Catalog, S3, and Athena-based ELT pipelines.

**Multi-Tenant Pre-Production Environment (Lake Formation)** _(Q3 2025)_
- Designed and implemented a Lake Formation-based pre-production environment for roughly 40 tenants, using multi-dialect views to grant cross-account read access to dev or production data without provisioning direct cross-account permissions.
- Configured a 90/10 dev/production data split across tenants to validate the deployment pipeline under realistic conditions ahead of each release, increasing confidence in production readiness.

**Infrastructure Unification (Terraform)** _(Q4 2025 - Jan 2026)_
- Migrated all data pipeline and ETL infrastructure, Airflow/MWAA, S3, Glue Data Catalog, Athena, Lambda, ECS Fargate, and Lake Formation, across dev, pre-production, and two production environments onto a single, unified Terraform module.
- Migrated the customized single-tenant branch back into the primary Kernel codebase, eliminating a parallel maintenance path.

**Prime: Greenfield Snowflake ELT Platform** _(Q1 2026 - Present)_
- Architected and led development of Prime, a greenfield ELT platform sourcing from Kernel via Snowflake's native Iceberg integration, orchestrated with Airflow/MWAA and organized around a medallion (bronze/silver/gold) architecture with semantic-layer views for downstream consumers.
- Built a modified OpenTelemetry-based observability model to calculate SLOs and capture DAG-level metadata across the platform.
- Designed governed data-access patterns using IAM, Lake Formation, Snowflake RBAC, and row-level security to control access to sensitive and tenant-specific data.
- Designed and drove MCP and AI-enabled data platform capabilities, creating controlled interfaces between LLM applications and governed enterprise data using Amazon Bedrock and Snowflake Cortex.

**Agentic Chat Interface (Pre-Production)** _(Q2 2026)_
- Built an agentic chat interface on StellarAlgo's CDP platform, sourcing from Prime, that performed intent routing, generated Snowflake queries, retrieved and summarized results, produced recommendations, and generated charts when appropriate.
- Instrumented the full agentic workflow with step-level observability, capturing system/user prompts, per-step LLM cost, and elapsed time per span; used this to reduce per-query cost from $2.00 to $0.15 during development.
- Reached QA red-teaming in the development environment before the project was discontinued ahead of a production release.

**Cloud Cost Optimization (FinOps)** _(Q2 2026 - Present)_
- Leading infrastructure cost-reduction efforts across the platform, cutting primary AWS production spend from approximately $100K/month to $50K/month, with additional savings across other environments.
- Designed and built a cloud cost analytics warehouse combining AWS billing, infrastructure, storage, query, and Snowflake data to attribute spend, identify cost growth, investigate anomalies, and prioritize optimization work.
- Throughout tenure: built and maintained integrations with 30+ source systems across REST APIs, relational databases, SaaS platforms, customer data warehouses, and object storage; mentor approximately eight junior and intermediate engineers on architecture, troubleshooting, and development practices.

### Business Intelligence & Database Consultant | Multiple Organizations | 2012 - 2021

_Selected engagements: Trimac Transportation, Mawer Investment Management, National Energy Board, and Teck Resources_

- Designed and maintained ETL and data integration pipelines connecting operational, financial, ERP, telemetry, SaaS, API, and external sources to enterprise warehouses and data marts.
- Integrated JSON API and telemetry data from six vendors for a fleet of 1,000+ commercial vehicles, supporting reporting and analytics across dozens of customers.
- Supported large-scale warehouse modernization initiatives, including migration and validation of 200+ reports and dependent database objects from legacy data marts to new enterprise platforms.
- Designed dimensional models including fact tables, dimensions, star schemas, snowflake schemas, OLAP structures, and analytical data marts.
- Built ETL, reconciliation, automated testing, and data-quality processes using SQL Server, T-SQL, SSIS, PowerShell, SSAS, and SSRS.
- Developed analytics and reporting solutions with Power BI, Tableau, and Microsoft BI technologies for finance, investment management, HR, logistics, mining, maintenance, and executive teams.
- Integrated enterprise systems including PeopleSoft, Microsoft Dynamics AX, Charles River, Advent Portfolio Exchange, Bloomberg, Capital IQ, and industrial mining platforms.
- Worked directly with business stakeholders, developers, infrastructure teams, and project managers to translate operational requirements into maintainable data solutions.

## Earlier Experience

**Checkwell Decision Corporation** | Reports Analyst / Database Developer | 2007 - 2012

Designed and optimized SQL Server databases, ETL pipelines, data marts, and reporting infrastructure. Built an enterprise SSRS environment containing 300+ reports used by 100+ business users. Developed schemas, stored procedures, views, indexes, integration routines, performance-tuning processes, and automated data-quality controls. Partnered with .NET development teams on database design, SQL performance, and application integration.

**Thomson Technology** | Database Programmer | 2001 - 2004

Developed and supported database applications and reporting solutions for Sales, Purchasing, and Finance teams in a manufacturing environment. Maintained Microsoft Access applications integrated with the Visual Manufacturing ERP platform.

## Education

**Simon Fraser University** | Management and Systems Science

Interdisciplinary coursework in Mathematics, Computer Science, Statistics, Economics, and Business.

## Additional Training

**SQL Server Business Intelligence Application Development** | Hands On IT Training
