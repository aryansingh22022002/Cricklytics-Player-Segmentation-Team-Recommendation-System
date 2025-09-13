# Cricklytics-Player-Segmentation-Team-Recommendation-System
Cricklytics is a data-driven sports analytics framework that leverages machine learning to bring transparency, fairness, and objectivity to player evaluation in junior-level cricket. By analyzing ball-by-ball and match-level data, the system segments players into role-specific categories and recommends balanced team compositions, enabling evidence-based decision-making for coaches, selectors, and academies.

## Key Features

- **Comprehensive Data Processing**  
  - Utilizes ball-by-ball (278k+ deliveries) and match-level (1,169 fixtures) IPL datasets.  
  - Rigorous cleaning: standardizing team names, handling missing values, mapping venues to cities.  

- **Feature Engineering**  
  - Batting: strike rates, boundary %, dot-ball %, phase-wise contributions (Powerplay, Middle Overs, Death Overs).  
  - Bowling: economy rates, strike rates, wickets per phase.  
  - Fielding: catches, run-outs, stumpings, dismissal involvement.  

- **Player Segmentation via Clustering**  
  - K-means++ clustering with optimal k determined using the Elbow Method.  
  - Roles identified include:  
    - **Batters**: Powerplay Strikers, Anchors, Death-Over Hitters  
    - **Bowlers**: Opening Bowlers, Middle-Over Controllers, Death-Over Specialists  

- **Team Recommendation Engine**  
  - Generates role-balanced playing XI to cover all phases of a T20 match.  
  - Avoids redundancy (e.g., multiple anchors without finishers).  
  - Provides ranked player recommendations per role.  

- **Interactive Web Application (Gradio)**  
  - **Home Tab**: Overview of the system.  
  - **Player Overview**: Phase-wise performance dashboards for individual players.  
  - **Player Comparison**: Side-by-side comparison with radar charts and statistics.  
  - **Team Recommendation**: Role-based player suggestions and balanced team lineups.  
