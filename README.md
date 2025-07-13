# IPL-RCB-Performance-Analysis
In-depth EDA of Royal Challengers Bangalore (RCB) IPL performance (2008-2025), analyzing team trends, player stats, and strategic insights to understand their path to success.



Run
Copy code
# Royal Challengers Bangalore (RCB) IPL Performance Analysis

This repository contains a detailed Exploratory Data Analysis (EDA) of the Royal Challengers Bangalore (RCB) cricket team's performance in the Indian Premier League (IPL) from 2008 to 2025. The analysis aims to uncover key trends, player statistics, and strategic insights that could explain RCB's performance, particularly focusing on the factors that might contribute to their success in the upcoming season.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Analysis Highlights](#analysis-highlights)
  - [Overall Team Performance](#overall-team-performance)
  - [Toss Impact and Decisions](#toss-impact-and-decisions)
  - [Player of the Match Awards](#player-of-the-match-awards)
  - [Batting Performance](#batting-performance)
  - [Bowling Performance](#bowling-performance)
- [Repository Structure](#repository-structure)
- [How to View the Analysis](#how-to-view-the-analysis)
- [Tools and Libraries](#tools-and-libraries)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Royal Challengers Bangalore (RCB) has a passionate fanbase but has yet to win an IPL title. This project delves into historical IPL data to analyze various facets of RCB's game, including:

*   **Match Outcomes:** Home vs. Away performance, season-wise wins.
*   **Toss Strategy:** Impact of winning/losing the toss and decision-making (batting/fielding first).
*   **Individual Player Contributions:** Identifying top performers in batting and bowling.
*   **Batting Metrics:** Strike rates, boundary hitting, dot ball percentages, and role-based contributions.
*   **Bowling Metrics:** Wickets, economy rates, strike rates, averages, and performance across different phases of the game (Powerplay, Middle Overs, Death Overs).

A special focus is given to the **2025 season data** to identify recent trends and potential indicators for future success.

## Data Sources

The analysis is based on two primary datasets:

1.  `matches.csv`: Contains information about each IPL match, including teams, venue, toss details, and match results.
2.  `deliveries.csv`: Contains ball-by-ball data for all IPL matches, providing granular details on runs scored, wickets taken, and bowler/batter performance.

*(Note: The file paths in the notebook are local. Please adjust them if you clone the repository and run the notebook locally.)*

## Analysis Highlights

### Overall Team Performance

*   **Total Matches (2008-2025):** RCB has played a total of **255** matches.
*   **Home vs. Away Record (2008-2024):**
    *   **Home (M Chinnaswamy Stadium):** 90 matches played, 44 won (**48.89% win rate**).
    *   **Away:** 165 matches played, 79 won (**47.88% win rate**).
*   **2025 Season Performance:**
    *   **Total Matches:** 16
    *   **Home:** 6 matches played, 2 won (**33.33% win rate**).
    *   **Away:** 10 matches played, 9 won (**90.0% win rate**).
    *   *Observation: A significant improvement in away game performance in 2025.*

### Toss Impact and Decisions

*   **Toss Won, Match Won (2008-2025):** RCB won the toss 128 times and won the match 67 times.
*   **Toss Lost, Match Won (2008-2025):** RCB lost the toss 143 times and still won the match 67 times.
*   **Toss Decision Preference (2008-2024):** RCB predominantly chose to **field first** (34 times at home, 52 times away) when winning the toss, indicating a preference for chasing.
*   **Toss Decision Preference (2025):** In 2025, RCB did not win a single toss at home but chose to field first 7 times when winning the toss in away games.

### Player of the Match Awards

*   **Overall Top Performers (2008-2025):**
    *   **AB de Villiers:** 23 awards
    *   **V Kohli:** 17 awards
    *   **CH Gayle:** 17 awards
*   **2025 Season Standouts:**
    *   **Krunal Pandya:** 3 awards
    *   **Rajat Patidar:** 2 awards
    *   **Josh Hazlewood, Jitesh Sharma, Phil Salt, Romario Shepherd, Suyash Sharma, Virat Kohli:** 1 award each.

### Batting Performance

*   **Average Team Scores (2008-2024):**
    *   **1st Innings:** 171 runs
    *   **2nd Innings (Chasing):** 150 runs
*   **Probability of Scoring > 170 (1st Innings, 2008-2024):** 51.77%
*   **Average Team Scores (2025):**
    *   **1st Innings:** 189 runs
    *   **2nd Innings (Chasing):** 172 runs
*   **Probability of Scoring > 170 (1st Innings, 2025):** 83.58%
    *   *Observation: A significant increase in average scores and probability of high scores in 2025, indicating improved batting form.*
*   **Top Boundary Hitters (Overall 2008-2024):** V Kohli, AB de Villiers, and CH Gayle consistently lead in both 4s and 6s.
*   **Top Boundary Hitters (2025):** V Kohli, PD Salt, and JM Sharma are prominent in hitting boundaries.

### Bowling Performance

*   **Overall Highest Wicket Taker (2008-2024):** **YS Chahal** (139 wickets).
*   **2025 Season Highest Wicket Taker:** **JR Hazlewood** (22 wickets).
*   **Wickets in 1st Innings (2008-2024):** YS Chahal (67), HV Patel (52), R Vinay Kumar (42).
*   **Wickets in 2nd Innings (2008-2024):** YS Chahal (72), Mohammed Siraj (49), HV Patel (47).
*   **Wickets in 1st Innings (2025):** JR Hazlewood (8), KH Pandya (8), B Kumar (7).
*   **Wickets in 2nd Innings (2025):** JR Hazlewood (14), B Kumar (10), Yash Dayal (8).

## How to View the Analysis

You can view the full analysis by opening the `RCB_IPL_Analysis.ipynb` notebook directly on GitHub.

To run the analysis locally:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/RCB_IPL_Analysis.git
    cd RCB_IPL_Analysis
    ```
2.  **Install dependencies:**
    It's recommended to use a virtual environment.
    ```bash
    pip install pandas numpy seaborn matplotlib plotly scikit-learn scipy
    ```
    *(Note: The original notebook uses `plotly.express` and `plotly.graph_objs`, and `scipy.stats.shapiro` and `scipy.stats.norm`.)*
3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
4.  Open `RCB_IPL_Analysis.ipynb` in your browser.

## Tools and Libraries

*   **Python 3**
*   **Pandas:** For data manipulation and analysis.
*   **NumPy:** For numerical operations.
*   **Matplotlib & Seaborn:** For static data visualizations.
*   **Plotly:** For interactive data visualizations.
*   **SciPy:** For statistical tests (Shapiro-Wilk test for normality) and probability calculations.

## Contributing

Feel free to fork this repository, open issues, or submit pull requests if you have suggestions for improvements or find any discrepancies.

