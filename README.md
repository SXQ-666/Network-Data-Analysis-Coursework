# Network Data Analysis Coursework

This repository contains the complete code, environment configuration, and data documentation for Part 1 and Part 2 of the Network Data Analysis module.

## Project Structure
- `Part1_Wikidata.ipynb`: Analysis of the Wikidata editor social network, focusing on specific community interaction patterns.
- `Part2_Leeds_Spatial.ipynb`: Spatial network analysis of Leeds, including accident pattern detection and marathon route planning.
- `environment.yml`: Conda environment file containing all necessary libraries (such as `OSMnx`, `Spaghetti`, and `PySAL`) required to run both parts of the analysis.

## Data Sources & Documentation
To ensure the reproducibility of the results, the following datasets were used:

### Part 1: Wikidata Social Network
The analysis for Part 1 was conducted using a subset of the Wikidata editor interaction data provided by the module. I specifically selected and analyzed the following three datasets:
1. `BOT_REQUESTS`
2. `PROJECT_CHAT`
3. `REQUEST_FOR_DELETION`

### Part 2: Leeds Road Safety & Spatial Network
- **Source**: Road Traffic Accidents data obtained from the official UK Government Open Data portal ([data.gov.uk](https://www.data.gov.uk/dataset/6efe5505-941f-45bf-b576-4c1e09b579a1/road-traffic-accidents)).
- **Time Period**: 2013, 2014, 2015, and 2016.
- **File Naming Note**: For clarity and to match the paths defined in the Jupyter Notebook, the raw CSV files were renamed upon download as follows:
  - `Road traffic accidents_2013.csv`
  - `Road traffic accidents_2014.csv`
  - `Road traffic accidents_2015.csv`
  - `Road traffic accidents_2016.csv`
- **Network Data**: Real-time road network topology extracted from OpenStreetMap (OSM) via the `OSMnx` library.

## How to Reproduce the Analysis
1. **Prepare Data**: Ensure the Part 2 `.csv` files are present in the working directory and named according to the convention listed above.
2. **Setup Environment**: Use the provided `environment.yml` to create a matching Conda environment:
   ```bash
   conda env create -f environment.yml
