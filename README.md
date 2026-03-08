# GoodThought NGO Data Analysis

## Project Overview
GoodThought NGO has been a catalyst for positive change, focusing its efforts on education, healthcare, and sustainable development to make a significant difference in communities worldwide. With this mission, GoodThought has orchestrated an array of assignments aimed at uplifting underprivileged populations and fostering long-term growth.

This project offers hands-on data-driven insights to direct and enhance humanitarian efforts. It involves analyzing the GoodThought PostgreSQL database, which encapsulates detailed records of assignments, funding, impacts, and donor activities from 2010 to 2023.

## Dataset Description
The PostgreSQL database contains the following comprehensive tables:
- **`Assignments`**: Details about each project, including its name, duration (start and end dates), budget, geographical region, and impact score.
- **`Donations`**: Records of financial contributions, linked to specific donors and assignments, highlighting how financial support is allocated and utilized.
- **`Donors`**: Information on individuals and organizations that fund GoodThought’s projects, including donor types.

*(Refer to `erd.png` or `erd_flow.png` in the repository for a visual representation of the relationships between these data tables.)*

## Objectives
The primary objective of this project is to execute complex SQL queries to extract meaningful insights from the NGO's data. Specifically, answering the following questions:
1. **Highest Donation Assignments**: Identifying top assignments based on total donation amount and the type of donor.
2. **Top Regional Impact Assignments**: Determining the highest impact assignment for each geographical region along with the total number of donations it received.

## Key SQL Concepts Utilized
- **Common Table Expressions (CTEs)**
- **Window Functions** (`ROW_NUMBER() OVER (PARTITION BY ... ORDER BY ...)`)
- **Aggregation Functions** (`SUM()`, `COUNT()`, `ROUND()`)
- **Joins** (`JOIN`), **Grouping** (`GROUP BY`)

## Project Structure
- `notebook.ipynb`: The main jupyter notebook containing the SQL queries and output tables.
- `ngo_project_image.jpg`: Contextual image for the project background.
- `ERD.png` / `erd_flow.png`: Entity-Relationship Diagrams outlining the relational database schema.

## Results & Insights
- Extracted the top 5 assignments with the highest total donations, and explored the distinction between Individual and Organization contributors.
- Highlighted the top impactful assignments partitioned by region (East, West, North, South) with their respective perfect/near-perfect impact scores (e.g., 9.99, 10.0) and total associated donation counts.
