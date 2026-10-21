# dbt and Google BigQuery Data Transformation Project

## Project Overview

This project demonstrates how to use **dbt (Data Build Tool)** with **Google BigQuery** to build, transform, and test SQL-based data models.

It covers the setup of a local dbt environment, connecting dbt to BigQuery, developing data models, loading seed data, validating data quality, and generating project documentation.

## Objectives

- Configure a local dbt environment.
- Connect dbt to Google BigQuery.
- Build SQL models to transform customer and order data.
- Load CSV seed data into BigQuery.
- Validate data using dbt tests.
- Generate and explore dbt documentation.
- Organize SQL models and project files using dbt conventions.

## Technologies Used

- **dbt Core** — data transformation and model management
- **Google BigQuery** — cloud data warehouse
- **SQL** — data transformation and querying
- **Python** — local development environment
- **Git and GitHub** — version control and project hosting

## Project Structure

```text
dbt_bigquery_course/
├── analyses/
├── macros/
├── models/
│   └── example/
│       ├── customers.sql
│       ├── my_first_dbt_model.sql
│       ├── my_second_dbt_model.sql
│       └── schema.yml
├── seeds/
│   └── stadiums.csv
├── snapshots/
├── tests/
├── dbt_project.yml
├── README.md
└── .gitignore
```

*The structure above represents the main project files. Keep only folders and filenames that actually exist in your local project.*

## Workflow

1. Configure dbt and connect it to Google BigQuery.
2. Develop SQL models for transforming data.
3. Load available CSV seed files into BigQuery.
4. Run dbt models to create or update tables and views.
5. Execute data quality tests.
6. Generate documentation to explore models and their dependencies.

## Useful Commands

Run these commands from the directory containing `dbt_project.yml`, with your virtual environment activated.

```bash
dbt debug
dbt seed
dbt run
dbt test
dbt docs generate
dbt docs serve --port 8082
```

Run `dbt seed` when seed files are available. The other commands should be run according to the project workflow and configuration.

## Configuration and Security

The BigQuery connection profile is stored separately from the project in the local dbt configuration directory.

**Never commit service-account JSON credentials, private keys, passwords, or other secrets to GitHub.** Use a secure local configuration and appropriate access controls.

## Learning Outcomes

Through this project, I practiced configuring dbt, developing SQL data models, working with BigQuery, testing transformations, loading seed data, and generating data-model documentation.

## Acknowledgements

This project was developed as a hands-on learning project based on a dbt and BigQuery tutorial, with practical configuration and troubleshooting during implementation.
