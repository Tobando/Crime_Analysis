# Crime Analysis in Montgomery County (2020–2024)

This project investigates patterns in reported crimes across Montgomery County, Maryland using publicly available data from dataMontgomery. The analysis explores seasonal, spatial, and temporal variations in crime with the goal of uncovering actionable insights for public safety planning and community awareness.

## Research Questions

1. Do crime rates vary by season and crime type?
2. Are violent crimes more geographically concentrated than non-violent crimes?
3. Do crime levels differ between weekends and weekdays?

## Project Structure

This project follows the Cookiecutter Data Science structure:

Crime_Analysis/
├── data/              
│   ├── raw/             <- Original Excel dataset
│   ├── interim/         <- Cleaned datasets (optional)
│   └── processed/       <- Final datasets (optional)
├── docs/                <- Optional documentation
├── models/              <- Model outputs or summaries (if applicable)
├── notebooks/           <- Jupyter notebooks with main analysis
├── references/          <- Data dictionaries, manuals, or supporting info
├── reports/
│   └── figures/         <- Visualizations and exported plots
├── requirements.txt     <- List of project dependencies
├── setup.py             <- Allows project to be installed as a package
├── src/
│   ├── data/            <- Scripts to load or transform data
│   ├── features/        <- Scripts for feature engineering
│   ├── models/          <- Modeling or testing scripts
│   └── visualization/   <- Plotting and chart functions
└── tox.ini              <- Test automation configuration

## Dependencies

The project uses the following packages:

- Python 3.9+
- pandas
- numpy
- seaborn
- matplotlib
- scipy
- jupyter
- scikit-learn

Install with:

To set up a virtual environment and install dependencies:
python3 -m venv venv
source venv/bin/activate # For Windows: venv\Scripts\activate
pip install -r requirements.txt

## Running the Notebook

To run the main analysis notebook:
jupyter notebook notebooks/MC_CrimeAnalysis.ipynb

vbnet
Copy
Edit

## Summary of Findings

- Property crimes like vandalism showed significant seasonal variation, peaking in the fall.
- Violent crimes were more geographically concentrated across zip codes (Gini coefficient = 0.5863).
- Daily crime counts were statistically higher on weekdays compared to weekends (p = 0.0035, Mann-Whitney U test).


<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
