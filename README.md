# MS_Spectrum_SNR
======================

A graphical application for analyzing mass spectral data and calculating Signal-to-Noise Ratio (SNR).

[![Python Version](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Overview
--------

The MS_Spectrum_SNR provides an intuitive interface for loading and analyzing mass spectrometry data. It features:

* CSV file loading for mass spectral data
* Interactive SNR calculation
* Real-time visualization
* Error handling and validation

## Installation
------------

```bash
pip install numpy pandas matplotlib scipy
```

## Features
--------

### Data Loading
* Supports CSV files with m/z and intensity values
* Automatic data validation
* Error handling for invalid files

### Analysis
* SNR calculation with customizable window size
* Real-time spectrum visualization
* Peak detection and marking

### Visualization
* Interactive matplotlib plots
* Clear peak and noise region highlighting
* Detailed result display

## Usage
-----

### Basic Usage

```python
import tkinter as tk
from mass_spectrum_analyzer import MassSpectrumAnalyzer

root = tk.Tk()
app = MassSpectrumAnalyzer(root)
root.mainloop()
```

### Example Workflow

1. Load CSV file containing mass spectral data
2. Enter target m/z value
3. Set window size (default: 50 Da)
4. Click "Calculate SNR"
5. View results in the visualization window

## Technical Details
-----------------

### SNR Calculation

The SNR is calculated using the formula:

SNR = Signal Height / Noise Standard Deviation

Where:
- Signal Height: Intensity at the target m/z value
- Noise Standard Deviation: Standard deviation of intensities outside the specified window

### Implementation Notes

* Uses NumPy for efficient numerical operations
* Matplotlib for visualization
* Tkinter for GUI components
* Error handling for invalid inputs and edge cases

## Output Example

![image](https://github.com/user-attachments/assets/313e5c49-99c5-4f36-b8bd-d0fa28e07279)




## Contributing
------------

Contributions are welcome! Please submit pull requests with:

1. Clear documentation of changes
2. Updated tests if applicable
3. Consistent code style

## License
-------

MIT License

Copyright (c) [2025] [Rohith Krishna]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
