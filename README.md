# Cuckoo Filter Implementation with Machine Learning for Fraudulent Transaction Detection

## Introduction

This project implements a Cuckoo filter from scratch and integrates machine learning to detect fraudulent transactions using financial data. The Cuckoo filter is a probabilistic data structure used for efficient set membership tests. In this context, it helps identify whether a user is legitimate or potentially involved in fraudulent activities.

## Usage

Follow the steps below to use the implementation:

1. **Update File Paths:**
   - Open the `test.py` file.
   - Change the paths of the following files:
     - `X_1.csv` file: Input financial data.
     - `random_forest_model.joblib`: Pre-trained machine learning model file.
     - `top_50_legitimate_users.txt`: File containing information about the top legitimate users.

2. **Run the Script:**
   - Execute `test.py` in your command line or terminal.
   - If prompted, enter a user to check if they are a legitimate user or not.
   - If no user input is provided, just press Enter, and the script will run a default example with test data.

## Example

```bash
python test.py
```

## Repository Structure

- **`cuckoo_filter.py`**: Contains the implementation of the Cuckoo filter.
- **`machine_learning.py`**: Implements the machine learning model for fraudulent transaction detection.
- **`test.py`**: The main script to test the Cuckoo filter and machine learning integration.
- **`X_1`**: Input financial data file.
- **`model_file`**: Pre-trained machine learning model file.
- **`top_50_legitimate_users`**: File containing information about the top legitimate users.

## Requirements

- Python 3.x
- NumPy
- Scikit-learn
- Other dependencies as mentioned in the script.

## Notes

- Ensure that the required dependencies are installed before running the script.
- The provided example assumes default file names; update as needed.

Feel free to explore and adapt this project for your specific use case.
