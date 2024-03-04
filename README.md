Dependency Graphs
========
For GDP dag -


https://github.com/muskangupta4/astro-example-dags/assets/65766138/ddc671fc-8508-4337-a906-262ee0109194


For titanic dag -



https://github.com/muskangupta4/astro-example-dags/assets/65766138/06c83e75-74ce-4375-bea3-0d33d3b824ad



Overview
========

This pipeline demonstrates how to use the Astro Cloud IDE. It loads the Titanic dataset, filters out passengers under 18, and aggregates the data by survival and class.

The pipeline is composed of four cells:

load: Loads the Titanic dataset from Seaborn's GitHub repository.

over_18: Filters out passengers under 18.

aggregate_sql: Aggregates the data by survival and class, using SQL.

aggregate_python: Aggregates the data by survival and class, using Python.

Note that each cell returns a value that can be referenced in subsequent cells using the {{cell_name}} syntax in SQL and cell_name syntax in Python.

Datasets Used
========
https://raw.githubusercontent.com/plotly/datasets/master/gapminderDataFiveYear.csv

Project Contents
================

Your Astro project contains the following files and folders:

- dags: This folder contains the Python files for your Airflow DAGs. 
- Dockerfile: This file contains a versioned Astro Runtime Docker image that provides a differentiated Airflow experience. If you want to execute other commands or overrides at runtime, specify them here.
- include: This folder contains any additional files that you want to include as part of your project. It is empty by default.
- packages.txt: Install OS-level packages needed for your project by adding them to this file. It is empty by default.
- requirements.txt: Install Python packages needed for your project by adding them to this file. It is empty by default.
- plugins: Add custom or community plugins for your project to this file. It is empty by default.
- airflow_settings.yaml: Use this local-only file to specify Airflow Connections, Variables, and Pools instead of entering them in the Airflow UI as you develop DAGs in this project.
