# Wavelength-Amplitude data visualization, and Wavelength Shift Calculation Code written by Necati Buhur

## Code Requirements

```python
#All Python code v 3.0 Google Compute Engine - Google Colab
#Dependencies:
import os
import csv
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from scipy.signal import find_peaks
from sklearn.preprocessing import RobustScaler
from sklearn.linear_model import LinearRegression

#Installation of dependencies:
pip install pandas numpy matplotlib scipy scikit-learn
```

## Usage
After the depencies are installed:
### Running the code in Google Colab

1. Open Google Colab ([colab.research.google.com](https://colab.research.google.com/)).
2. Go to "File" > "Open notebook" > "GitHub".
3. Paste the URL of your GitHub repository (e.g., `https://github.com/nicobuhur/ring-resonator-wave-shift`).
4. Select the notebook file (e.g., `waveform_resonator_colab.ipynb or waveform_resonator_local.ipynb`) you want to run.
5. Follow the instructions in the notebook to execute the code cells.

## Compatibility
Functions are designed for data acquired from Micro Ring Resonator experiments, and software "PicoScope 7 T&M" is used to read electric signals. Software crates waveforms which are written into csv files. In data, voltage over time is exhibited, and time parameters is turned into wavelength with programming. Example data is provided in repository. 
