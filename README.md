# Project pHastCam: Measuring LED Wavelength

The Python script establishes communications with the spectroradiometer - for more info on this, check out [this python-seabreeze repo](https://github.com/ap--/python-seabreeze) and [this frugal spectroscopy repo](https://github.com/timrobinson/Frugal-Spectroscopy). Next, within the script, integration time is established within microseconds. Multiple scans are run and signal-averaged, leading to results like the spectrum below. The final cells interpolate the data, saving a two-column array to a file, with a wavelength range of 400 to 700 nm in 5 nm increments, and normalizes the counts. This interpolation is performed so that the LED data can be readily multiplied by other components of a model (such as dye spectra and camera responsivity) to analyze the effectiveness of our design for screening accuracy. 

<p align="center">
  <img src="spectrum.png" width="600">
</p>

## Installation  
1. Clone the repository
    git clone https://github.com/pHastCam/LED_Measurement.git
    cd LED_Measurement
2. Create the conda environment from YAML file
    conda env create -f environment.yml
3. Activate the environment
    conda activate LED_Measurement
4. Launch Jupyter Notebook

## Usage
1. When the environment is active, launch Jupyter Notebook 
2. Open to the notebook associated with the code in the browser interface
3. Note that several cells require changes to the local path of the files on the user's computer.

## Built with 
Python 3.9.17
Numpy 1.25.2
Pandas 1.5.3
Matplotlib 3.7.1
SciPy 1.11.1
Seabreeze 2.4.0






- Navigate to the notebook file (e.g., filename.ipynb) in the browser interface.
- Open and run cells interactively.
