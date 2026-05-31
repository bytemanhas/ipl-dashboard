# IPL Analytics Dashboard – Power BI Project Report

## Project Overview

The IPL Analytics Dashboard is a comprehensive business intelligence solution developed in Power BI to analyze Indian Premier League (IPL) performance across teams, players, venues, and seasons. The dashboard transforms raw match and ball-by-ball data into actionable insights through interactive visualizations, dynamic filtering, and advanced DAX measures.

The project is designed to provide stakeholders, cricket analysts, and sports enthusiasts with a centralized platform for understanding batting performance, bowling performance, team success trends, venue statistics, and match outcomes.

---

## Business Objective

The primary objective of this project is to analyze historical IPL data and identify key performance indicators related to:

* Team performance across seasons
* Batting excellence and Orange Cap contenders
* Bowling dominance and Purple Cap contenders
* Match-winning patterns
* Venue-wise performance
* Toss decision impact on match results

The dashboard enables users to explore player and team performance through interactive filters and drill-down analysis.

---

## Dataset Description

The project utilizes multiple datasets organized in a star-schema model:

### Fact Tables

**Fact_Match**

* Match Number
* Match Date
* Team 1
* Team 2
* Winner
* Toss Winner
* Toss Decision
* Venue
* City
* Season

**Fact_BallbyBall**

* Match ID
* Innings
* Overs
* Ball Number
* Batter
* Bowler
* Batsman Runs
* Extras
* Total Runs
* Wicket Information

### Dimension Tables

**Dim_Player**

* Player Information
* Batting Name
* Fielding Name

**Dim_Team**

* Team Name
* Team Metadata

---

## Data Modeling

A star schema model was implemented to optimize report performance and maintain analytical flexibility.

### Relationships

* Fact_Match ↔ Fact_BallbyBall via Match ID
* Dim_Team connected to match data
* Dim_Player connected through player-level analysis

The model supports season-level filtering and player-level analysis across all dashboard pages.

---

## Dashboard Architecture

### Page 1 – Executive Overview

Purpose:
Provide a high-level summary of IPL performance.

Key KPIs:

* Total Matches
* Total Runs
* Total Wickets
* Average Score
* Total Sixes
* Total Fours

Visuals:

* Toss Decision Analysis
* Most Successful IPL Teams
* Matches Hosted by Venue
* Top IPL Host Cities
* Team Performance by Season

---

### Page 2 – Batting Analytics

Purpose:
Analyze batting performance and identify top-performing batsmen.

Key KPIs:

* Total Batter Runs
* Total Batters
* Total Boundaries
* Total Sixes
* Orange Cap Runs
* Orange Cap Holder

Visuals:

* Orange Cap Leaders
* Boundary Leaders
* Runs Distribution by Overs Phase
* Dynamic Season and Batter Analysis

Features:

* Dynamic dashboard title
* Season-based filtering
* Batter-level analysis

---

### Page 3 – Bowling Analytics

Purpose:
Evaluate bowling performance and identify the most impactful bowlers.

Key KPIs:

* Total Wickets
* Total Bowlers
* Average Wickets per Match
* Dot Balls
* Purple Cap Wickets
* Purple Cap Holder

Visuals:

* Purple Cap Leaders
* Dot Ball Specialists
* Economy Rate Leaders
* Wickets by Bowling Phase

Features:

* Dynamic dashboard title
* Season and Bowler filters
* Phase-wise bowling analysis

---

## DAX Measures Implemented

Key measures created during development include:

* Total Matches
* Total Runs
* Total Wickets
* Average Runs per Match
* Total Boundaries
* Total Sixes
* Orange Cap Holder
* Orange Cap Runs
* Purple Cap Holder
* Purple Cap Wickets
* Dot Balls
* Economy Rate
* Bowling Phase Classification
* Dynamic Dashboard Titles

These measures allow the dashboard to respond dynamically to user selections and filters.

---

## Key Insights Generated

### Batting Insights

* Virat Kohli emerged as the highest run scorer across seasons.
* Boundary scoring contributes significantly to total run accumulation.
* Middle overs generate the highest run volume across teams.

### Bowling Insights

* Yuzvendra Chahal leads wicket-taking statistics.
* Certain bowlers excel through dot-ball pressure rather than wickets alone.
* Wicket distribution varies significantly across powerplay, middle, and death overs.

### Team Insights

* Mumbai Indians and Chennai Super Kings remain the most successful franchises.
* Toss decisions influence match outcomes in specific conditions.
* Venue characteristics impact scoring patterns and team performance.


---

## Tools & Technologies

* Power BI Desktop
* DAX (Data Analysis Expressions)
* Power Query
* Data Modeling
* Data Visualization
* Interactive Dashboard Design

---

## Project Outcome

The IPL Analytics Dashboard successfully consolidates match-level and ball-by-ball data into an interactive analytical platform. Through advanced DAX calculations, dynamic filtering, and a structured data model, the dashboard delivers meaningful insights into batting, bowling, team performance, and match trends.

The project demonstrates expertise in data modeling, business intelligence reporting, KPI design, DAX development, and dashboard storytelling, making it suitable for portfolio presentation, GitHub publication, and data analyst interviews.
