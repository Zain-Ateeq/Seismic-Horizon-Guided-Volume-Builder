# Seismic Horizon-Guided Volume Builder

## Overview
This project utilizes open-source F3 Seismic data (download link: https://terranubis.com/datainfo/F3-Demo-2020), including its well logs and given horizons, to generate a seismic volume using well log data, seismic horizon data, and an inverse distance approach. Unlike simple linear extrapolation, this approach preserves the trend of seismic horizons throughout the volume, ensuring a geologically consistent distribution of properties.
This project contains all the required data and it provides a method to generate a seismic volume using well log data, seismic horizon data, and an inverse distance approach. Unlike simple linear extrapolation, this approach preserves the trend of seismic horizons throughout the volume, ensuring a geologically consistent distribution of properties.

## Features
- Uses well log values at well locations to extrapolate property values across the entire seismic volume.
- Incorporates seismic horizon data to guide the extrapolation and maintain geological trends.
- Implements an inverse distance weighting approach for interpolation.
- Generates and visualizes inlines and crosslines of the new volume.
- Saves the computed seismic volume for further analysis.
- Acoustic Impedance volume generation included.

## Data Requirements
To use this project, you will need:
- **Well log data**: Containing measured petrophysical properties.
- **Seismic horizon data**: To guide the volume extrapolation.
- **Seismic volume structure**: For defining the output volume dimensions.

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/Zain-Ateeq/Seismic-Horizon-Guided-Volume-Builder.git
   cd seismic-horizon-volume-builder
   ```
2. Install necessary dependencies (if required):
   ```bash
   pip install numpy pandas glob2 random segyio seaborn matplotlib tqdm
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook Seismic-Horizon-Guided-Volume-Builder.ipynb
   ```
4. Run the notebook cells to:
   - Load well log and seismic horizon data.
   - Generate the volume using inverse distance weighting.
   - Visualize inlines and crosslines.
   - Save the final volume.

## Visualization
The notebook includes plotting functions to inspect:
- Inline and crossline sections of the computed volume.
- The impact of horizon-guided extrapolation.

## Output
- A new seismic volume file containing extrapolated Acoustic Impedance values.

## Contributions
Contributions are welcome! Feel free to submit pull requests or open issues for discussions and improvements.

## Contact
For questions or discussions, feel free to reach out via zainateeq448@gmail.com.

