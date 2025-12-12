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

If you don't have `uv` installed, install it with:

```bash
# On macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# On Windows
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"

# Alternative: Install via pip
pip install uv
```

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/samarthya/METAD699-Project.git
   cd METAD699-Project
   ```

2. **Set up the environment with uv**

   ```bash
   # This creates a virtual environment and installs all dependencies
   uv sync
   ```

   The `uv sync` command will:
   - Create a `.venv` virtual environment if it doesn't exist
   - Install Python 3.12 if needed
   - Install all project dependencies from `pyproject.toml`
   - Lock dependencies in `uv.lock` for reproducibility

3. **Run Jupyter Notebook**

   **Option A: Using uv (recommended - no activation needed)**

   ```bash
   uv run jupyter notebook zurich_airbnb.ipynb
   ```

   **Option B: Activate virtual environment first**

   On Linux/Mac:
   ```bash
   source .venv/bin/activate
   jupyter notebook zurich_airbnb.ipynb
   ```

   On Windows (Command Prompt):
   ```cmd
   .venv\Scripts\activate
   jupyter notebook zurich_airbnb.ipynb
   ```

   On Windows (PowerShell):
   ```powershell
   .venv\Scripts\Activate.ps1
   jupyter notebook zurich_airbnb.ipynb
   ```

### Project Structure

```bash
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
