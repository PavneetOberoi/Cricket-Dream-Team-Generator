# Fantasy Cricket Dream Team Selection

Fantasy Cricket Dream Team Selection is a Python-based project that helps users select the best fantasy cricket team for a match based on player statistics and predictions. The project uses machine learning models to predict player performance and suggests an optimal team based on the predicted points.

## Table of Contents

- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Contributing](#contributing)

## Usage

1. Ensure that the required libraries and dependencies are installed (see Prerequisites and Installation).

2. Prepare the necessary data:
   - Create a DataFrame containing player statistics and details, such as team, role, and previous match performance.
   - Define a DataFrame that maps players to their ranks based on performance.

3. Load the data into the main script:
   - Modify the 'teams' DataFrame to include player statistics and details.
   - Create a DataFrame 'ranking' that maps players to their ranks based on performance.

4. Define and train the machine learning models for predicting player points:
   - Train linear regression models (all-rounders, batsmen, bowlers) to predict points for different player roles.
   - Save the trained models as 'all_rounders_linear_regression', 'batsmen_linear_regression', and 'bowlers_linear_regression'.

5. Execute the 'select_team' function with appropriate arguments:
   - Provide the team names, stadium, toss result, 'teams' DataFrame, 'ranking' DataFrame, and hand function for handedness mapping.
   - The 'select_team' function will output the selected dream team and their predicted points.

## Data

The project uses player statistics and details, such as team, role, and previous match performance, to predict points for fantasy cricket team selection. Ensure that the data is formatted correctly with no missing values.

## Models

The project uses three linear regression models to predict points for different player roles:
- 'all_rounders_linear_regression': Model for predicting points for all-rounders.
- 'batsmen_linear_regression': Model for predicting points for batsmen.
- 'bowlers_linear_regression': Model for predicting points for bowlers.

These models should be trained using historical player data before executing the main script.

## Contributing

Contributions are welcome! If you find any issues with the project or want to add new features, feel free to submit a pull request.
