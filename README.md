
Project Title
A High-Quality and Robust Electro-Intravascular Myography (EiMG) Acquisition Method for Dynamic States

Project Overview
This project provides a comprehensive Python code suite for analyzing Electro-Intravascular Myography (EiMG) and surface electromyography (sEMG) signals. It supports batch processing, analysis, and visualization of multiple features under both dynamic (walking, movement) and static (standing, rest) conditions, including signal preprocessing, time/frequency domain feature extraction, sliding window analysis, clustering, and energy analysis.

The code is suitable for applications in bioelectrical signal research, EMG data mining, biomedical engineering, machine learning, and more.

Main Features
Batch reading and concatenation of EiMG/sEMG signals across multiple days and states

Signal preprocessing (filtering, normalization, etc.)

Time-domain analysis (e.g., RMS, MAV, kurtosis, KR, etc.)

Frequency-domain analysis (PSD, multi-band energy, and energy ratio calculations)

Sliding window feature extraction and clustering analysis

Analysis of correlations between EMG signals

File Structure
(To be supplemented)

yaml
├── src/                    # Source code directory
│   ├── load_and_concatenate_emg.py      # Data reading and concatenation
│   ├── feature_extraction.py            # Feature extraction functions
│   ├── psd_band_ratio_analysis.py       # Frequency domain analysis
│   ├── ...
├── data/                   # Data directory (recommended structure: data/state/date/file)
│   ├── Steady/
│   │   ├── 0918/0918_i.xlsx
│   │   └── ...
│   └── Walk/
│       └── 0920/0920_s.xlsx
├── results/                # Output directory for analysis results
│   ├── features/
│   ├── plots/
│   └── ...
├── requirements.txt        # Python dependencies
├── README.md
Dependencies
Python >= 3.7

pandas

numpy

scipy

matplotlib

openpyxl

tqdm

Install with:

bash
pip install -r requirements.txt
How to Use
Prepare Data
Place your EMG data (EiMG, sEMG) in .xlsx format into the designated data/ directory. The recommended directory structure is:

bash
state/date_i.xlsx and date_s.xlsx
View Results
Analysis results are automatically saved in the results/ directory.

Notes
Data files must be in .xlsx format, with the first column as the signal data.

For parameters of each feature analysis function, please refer to the docstring at the top of each .py script.

For custom features or grouping requirements, modify the relevant scripts as needed.

Contact
For questions, please contact the project lead:

Name: Ying Du

Email: 2120230491@nankai.edu.cn

Acknowledgements
Thanks to the experimental team and data contributors for their support.
