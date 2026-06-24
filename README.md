# ATP Tennis Data Warehouse

This repository contains the project developed for the **Data Warehouse and Visualization** course at the **University of Calabria**.

## Project Description

The objective of the project is the design and implementation of a data warehouse for the analysis of ATP tennis matches.

Starting from the *ATP Tennis Daily Pull* dataset, the project follows the complete data warehouse development process, including data reconciliation, data quality assessment, conceptual design, logical design and ETL implementation.

The main analytical focus is the study of match outcomes and upset events, where an underdog defeats the favourite according to pre-match betting odds.

## Data Source

Dataset: **ATP Tennis Daily Pull**

Source: Kaggle

https://www.kaggle.com/datasets/dissfya/atp-tennis-2000-2023daily-pull/data

The dataset contains 67,512 ATP matches played between January 2000 and April 2026, including information about tournaments, rounds, players, rankings, ATP points, playing conditions and betting odds.

## Repository Contents

* `Data_Management_Luca_Scanga.ipynb`
  Notebook containing data quality assessment, cleaning decisions, ETL implementation and final validation.

* `tennis_project.db`
  SQLite database containing both the reconciled schema and the dimensional model.

* `atp_tennis.csv`
  Original source dataset.

* `report/`
  Project report describing the complete design process, from source analysis to the final star schema.

* `Luca Scanga Projcet.twbx`
  Tableau packaged workbook containing the dashboards and interactive visualizations developed for the analysis of ATP matches, match outcomes and upset events.

## Data Warehouse Model

The dimensional model is centred on the fact table **FACT_MATCH**.

The warehouse includes the following dimensions:

* DIM_DATE
* DIM_TOURNAMENT
* DIM_ROUND
* DIM_SURFACE
* DIM_COURT
* DIM_BEST_OF
* DIM_PLAYER

The player dimension is used as a role-playing dimension to represent winners, losers, favourites and underdogs.

## Technologies

* Python
* SQLite
* Pandas
* Google Colab
* Tableau
* DBeaver

## Author

**Luca Scanga**

Data Warehouse and Visualization

University of Calabria

Academic Year 2025–2026
