# AD699 Semester Project - Zurich Airbnb Analysis

## Project Overview

This is a comprehensive data mining project analyzing Airbnb rental data from Zurich, Switzerland. The analysis covers:

- Data preparation & exploration
- Prediction using linear regression
- Classification using k-NN, decision trees, and text models
- Clustering analysis
- Conclusions and business insights

## Setup Instructions

### Prerequisites

- Python 3.12 or higher
- [uv](https://docs.astral.sh/uv/) package manager

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/samarthya/METAD699-Project.git
   cd METAD699-Project
   ```

2. **Install dependencies using uv**

   ```bash
   uv sync
   ```

3. **Activate the virtual environment**

   ```bash
   source .venv/bin/activate  # On Linux/Mac
   ```

4. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook zurich_airbnb.ipynb
   ```

### Project Structure

```
METAD699-Project/
├── data/                          # Dataset files
│   ├── zurich_listings.csv
│   ├── geneva_listings.csv
│   ├── vaud_listings.csv
│   └── Inside Airbnb Data Dictionary.csv
├── output/                        # Generated visualizations and maps
├── zurich_airbnb.ipynb           # Main analysis notebook
├── pyproject.toml                # Project dependencies
└── README.md                     # This file
```

## Data Organization

The downloaded CSVs are available in the local `data/` folder

## Running the Analysis

Open `zurich_airbnb.ipynb` in Jupyter and run cells sequentially. The notebook will:

- Load and clean the Airbnb data
- Generate statistical summaries
- Create visualizations (saved to `output/` folder)
- Build predictive models
- Perform clustering analysis

All generated figures and interactive maps are automatically saved to the `output/` directory.
