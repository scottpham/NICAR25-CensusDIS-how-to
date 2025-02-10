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


censusdis = "https://censusreporter.org/topics/housing/"

## Notebooks

### 1. Basic Mapping
This notebook demonstrates how to:
1. Set up census API access
2. Download housing data for Minnesota counties using censusdis
3. Create basic choropleth maps using both:
   - Static matplotlib-based plotting
   - Interactive folium-based maps with explore()

### 2. Finding Tables
This notebook shows how to:
1. Explore available Census datasets and tables using censusdis
   - Search all datasets for specific terms (e.g., "migration")
   - Filter for specific surveys (like ACS)
   - Search through available data groups
2. Find and examine specific Census tables
   - Search variables within tables
   - View table structures in tree format
3. Download and combine data from multiple tables
   - Work with transportation (B08301) and housing (B25071) data
   - Calculate derived statistics (e.g., percentage of public transport usage)
   - Filter for specific geographic areas (demonstrated with Hennepin and Ramsey counties)

