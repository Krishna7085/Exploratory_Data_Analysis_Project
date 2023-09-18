# EDA Assignment - 01

This project is centered around exploratory data analysis techniques and presentation of results to a client.

## Data

- The King County Housing Data: This dataset contains information about home sales in King County (USA).
- Find the data in the eda schema database, access it via DBeaver. Please save the csv file in the data folder.
- Explore the dataset in DBeaver and Join the 2 tables.
- The description of the column names can be found in the `column_names.md` file.

Created a SQL Database that contains the data. In the [first notebook (Fetching_the_data)](1_Fetching_the_data_eda.ipynb) and follow the steps on how to fetch the data and save it in a csv file.

## Task

1. Create a new repo using this [template](https://github.com/spiced-academy/ds-eda-project-template).

2. Through EDA/statistical analysis above please come up with **AT LEAST 3 insights** regarding the overall data. One should be geographical.

3. In addition also come up with **AT LEAST 3 recommendations** for the client.

## Visualization

Create the visualizations with the libraries:

- matplotlib
- seaborn
- plotly and more


# My Client
 Erin Robinson is a Buyer who likes to invest in poor neighbourhoods, buying & selling, costs back + little profit, socially responsible. 
  [EDA Project](./EDA Project.pdf)

 She wants to buy old houses in the poor neighbourhood (cheap old houses) and wants to renovate them and cut extra costs (costs for only necessary changes) plus she wants to make a little profit after resale, also she wants to be socially responsible. This means her customers would be the one who looks for a lower price from the same neighbourhood.

 1. **Recommendation and Investment Strategy**:
   - Based on the analysis, provide specific recommendations to the client, Erin Robinson, regarding which neighborhoods or types of properties to target for investment.
   - Develop an investment strategy that aligns with Erin's goals of socially responsible investing in poor neighbourhoods with the aim of making a small profit.

2. **Visualization and Presentation**:
   - Create compelling visualizations to support the findings and recommendations. Visual aids can be very effective in conveying information to non-technical clients.
   - Prepare a presentation summarizing the key findings and recommendations. Use clear and concise language to explain the insights and the reasoning behind the recommendations.

By conducting these analyses and presenting the findings in a clear and actionable way, one can provide valuable insights and recommendations to Erin Robinson, helping her make informed decisions about her real estate investments in King County.



## Requirements

- pyenv
- python==3.11.3

## Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you have to create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*

### Unit testing (Optional)

If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in terminal:

```bash
pytest
```

This command will execute all the functions in your project that start with the word **test**.


### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

```bash
brew update
brew install postgresql
```

In order to install the environment you can use the following commands:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
