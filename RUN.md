# Running the ETL Pipeline with Logging

## Prerequisites
- Python 3.7 or higher
- Jupyter Notebook or JupyterLab installed
- All required dependencies installed

## How to Run

### Method 1: Run the Jupyter Notebook
```bash
# Start Jupyter from the repository root
jupyter notebook

# Navigate to and open: logs/lab_2_4_repro_logging.ipynb
# Run all cells (Ctrl+A, then Shift+Enter)
```

### Method 2: Run as a Python Script
```bash
# Extract the notebook code and run it directly
python logs/lab_2_4_repro_logging.ipynb
```

## Expected Output

The logging setup will:
1. Configure a logger with both console and file output
2. Display logs in the terminal with format: `TIMESTAMP | LEVEL | MESSAGE`
3. Write logs to a file named `run_YYYYMMDD_HHMM.log` in the same directory

### Log Output Example
```
2026-01-18 10:30:45,123 | INFO | Hello World
```

## Output Files
- **Log File**: `run_YYYYMMDD_HHMM.log` - Contains all logging output

## Notes
- The file handler creates a timestamped log file for record-keeping
- Console output is also configured for immediate visibility
- Both handlers use the same format for consistency
