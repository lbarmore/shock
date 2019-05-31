# shock
Data analysis for dynamic compression experiments on gas and powder guns

## How to use
For each experiment, make a json file with the shot data including:

- projectile velocity
- interferometry probe locations
- impact time at each probe
- particle velocity (from VISAR or PDV data)
- shock velocity (calculated from transit time and sample thickness)
- ambient density, sound speed, index of refraction
- uncertainties on all these values

Each of the analysis files (TiltCalculator, ErrorAnalysis) takes the values from this json file, so you just need to update the path in these files to the correct shot you want to analyze. 

Use image production files (CSVreader) to make images of wave profiles and (coming soon) stress-density and shock velocity-particle velocity plots. 

All analysis and image production files are Python 3 Jupyter notebooks.
