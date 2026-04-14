# Network Data Analysis Coursework

This repo contains all the code, environment setup, and data notes for Part 1 and Part 2 of my Network Data Analysis module.

1. Part1_wikidata.ipynb : Looks at the social network of Wikidata editors, focusing on how certain communities interact with each other.
2. Part2_Leeds_Spatial.ipynb : Does some spatial network analysis on Leeds – finding accident hotspots and planning a marathon route.
3. environment.yml : A Conda environment file that lists all the libraries I used (like OSMnx, Spaghetti, PySAL). You'll need this to run my code.
4. **How to run these codes**: 
   - Get the data ready: Make sure the four CSV files for Part 2 are in the same folder as the notebooks, and named exactly as above.
   - Set up the environment: Use the `environment.yml` file to create a Conda environment. Run this command in your terminal: `conda env create -f environment.yml`

## Data sources & notes

To make sure my results can be reproduced, I used the following datasets:

### Part 1: Wikidata social network

I used a subset of the Wikidata editor interaction data provided by the module. I picked three specific datasets to analyse:
- `BOT_REQUESTS`
- `PROJECT_CHAT`
- `REQUEST_FOR_DELETION`

### Part 2: Leeds road safety & spatial network

- **Accident data**: Downloaded from the UK Government open data portal ([data.gov.uk](https://www.data.gov.uk/dataset/6efe5505-941f-45bf-b576-4c1e09b579a1/road-traffic-accidents)), covering 2013, 2014, 2015 and 2016.
- **File names**: I renamed the raw CSV files after downloading so they match the paths in my notebook:
  - `Road traffic accidents_2013.csv`
  - `Road traffic accidents_2014.csv`
  - `Road traffic accidents_2015.csv`
  - `Road traffic accidents_2016.csv`
- **Road network data**: Extracted live from OpenStreetMap using the `OSMnx` library.
