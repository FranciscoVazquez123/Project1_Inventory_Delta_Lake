# Project 1 — Centralized Inventory with Delta Lake

## Overview
First project of my Databricks learning roadmap, focused on Supply Chain analytics.  
Built a Medallion Architecture (Bronze → Silver → Gold) using a real supply chain dataset.

## Dataset
**SCMS Delivery History Dataset** — USAID  
10,324 shipment records across 15+ countries | 33 columns

## What I Built

| Layer | Description |
|-------|-------------|
| Bronze | Raw data ingested and stored as a Delta table |
| Silver | Data cleaning: date parsing, type casting, invalid values handled |
| Gold | Analytical tables with supply chain KPIs |

## KPIs Calculated
- Lead time by country and product group
- Freight cost per unit by product
- Shipment mode mix (% Air / Ocean / Truck) by country

## Tools
- Databricks Free Edition
- PySpark
- Delta Lake
- Spark SQL

## Key Learnings
- Delta Lake requires clean column names — no special characters or spaces
- Real datasets have multiple date formats across columns
- The importance of following a Medallion Architecture
