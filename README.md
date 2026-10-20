# Data Science Project: Geospatial Visualization with Geoplotlib

## Problem / Research Question
How can we use geospatial visualization libraries to reveal geographic patterns in public datasets, and how do custom interactive layers extend static maps into exploratory tools?

## Dataset Source and Usage Permissions
- **us_states.json**: US states GeoJSON from the US Census Bureau. Fields include `NAME` and `CENSUSAREA` (land area in square miles). Public domain, free for educational use.
- **flight_tracking.csv**: ADS-B aircraft tracking data around Leeds, UK (September 2017). Fields: `hex_ident`, `altitude`, `lat`, `lon`, `date`, `time`, `angle`, `distance`, `squawk`, `ground_speed`, `track`, `callsign`. Provided as course material for CISC7204, free for classroom use.

## Methods and Tools Used
- **Language**: Python 3.14
- **Libraries**: `geoplotlib`, `pandas`, `matplotlib`, `scipy`, `pyglet`
- **Visualizations**: Choropleth map of US states; animated aircraft tracking layer around Leeds.

## Key Findings and One Limitation
- **Findings**: Western US states (Texas, California, Montana) have the largest land area. Aircraft points cluster along flight corridors between Leeds, Bradford, and Wakefield.
- **Limitation**: The choropleth uses only census area, not population or economic data. The flight dataset covers only a small region and time window.

## Instructions for Running the Analysis
1. Install dependencies: `pip install -r requirements.txt`
2. Open `mc653871_Exercise8.02.ipynb` in Jupyter and run all cells.
3. Open `mc653871_Exercise8.04.ipynb` and run all cells; the final cell opens an animation window.
4. If the animation does not open, run `python run_ex804.py` from the command line.
