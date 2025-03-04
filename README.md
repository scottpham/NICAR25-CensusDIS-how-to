## How to use CensusDis, the friendliest Python API for U.S. Census Data

This is a repo for [a workshop](https://schedules.ire.org/nicar-2025/index.html#1056) presented at the 2025 NICAR confernece.


## Installation
This repo uses Python 3.11.8 but should work for most any version 3.0+. It uses the built-in `venv` module for virtual environments. To install, clone the repo and run the following commands:

```bash
python -m venv env
source env/bin/activate  # Use venv\Scripts\activate on Windows
pip install -r requirements.txt
```

## API KEY
You'll need an API key from the U.S. Census Bureau to use this package. You can get one [here](https://api.census.gov/data/key_signup.html).


censusdis = "https://github.com/vengroff/censusdis"

## Notebooks

### 1. Basic Mapping
This notebook demonstrates how to:
1. Set up census API access
2. Download population data for Minnesota counties using censusdis
3. Create basic choropleth maps using both:
   - Static matplotlib-based plotting for county-level data
   - Work with Census tract-level geography
   - Interactive folium-based maps with explore()

### 2. Finding Tables
This notebook shows how to:
1. Explore available Census datasets and tables using censusdis
   - Search all datasets for specific terms (e.g., "assistance")
   - Filter for specific surveys (like ACS)
   - Search through available data groups
2. Find and examine specific Census tables
   - Search variables within tables
   - View table structures in tree format
3. Download and analyze public assistance data
   - Work with SNAP program data (B22002)
   - Calculate derived statistics (e.g., percentage of households receiving assistance)
   - Compare assistance rates across all U.S. states
4. Create choropleth maps to visualize public assistance data
   - Use censusdis mapping capabilities with state-level data
   - Customize maps with color schemes and styling options

### 3. Dating Pool
This notebook demonstrates how to:
1. Use the censusdis.states module for state lookups and conversions
2. Find and analyze marital status data by age (table B12002)
3. Locate specific cities ("Places") in the Census data
4. Calculate the "dating pool" for specific demographics in different cities
   - Filter for specific age ranges (e.g., 35-49 year olds)
   - Compare eligibility percentages across cities
5. Analyze the distribution of eligible singles across all U.S. cities
   - Filter for cities above a population threshold
   - Calculate and compare percentages across cities

### 4. Alternative Tables
This notebook explores how to:
1. Work with non-ACS Census datasets, specifically the Current Population Survey (CPS)
2. Search for and identify relevant variables in the CPS dataset
   - Find poverty-related variables
   - Understand variable categories and weights
3. Download and analyze poverty data by state
   - Calculate the poverty rate using person weights
   - Process and aggregate CPS microdata
4. Create choropleth maps to visualize poverty rates across the United States
   - Use censusdis mapping capabilities with state-level data

