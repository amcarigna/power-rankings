# Power Rankings
An python application for generating power rankings for a sports league. Currently in development. Developed with using the NFL (American Football) in mind.  
At the moment it functions more like a package due to the fact that it is missing a user interface. I've been using Jupyter Notebook to run functions from it. The necessary functions are all present and work properly. The most important function is: `models.build_league()`, which will:
- take a dictionary of teams to build a league for the first time, or
- take a .json file with saved data as the season progresses.
Important public functions include:
- `models.League.game()`, which takes game results and saves them,
- `models.League.week_complete()`, which performs clean up tasks at the end of each "round" of the season and calls the power ranking function, and
- `models.League.build_csv()` and `models.League.build_xlsx()` to visualize league info.  
TODOs include:
- switch to linear model for power rankings
- functionality for team health, qb health
- make power ranking formula have options for the user (access to parameters and hyperparameters)
- make models flexible to change those options easily
- doc strings for public functions
- main script for user interface
- graphical options (matplotlib for team series data)?
- matchup predictor

