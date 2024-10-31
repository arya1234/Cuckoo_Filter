# Cuckoo Filter Implementation with Machine Learning for Fraudulent Transaction Detection

## Overview

This project combines a custom-built **Cuckoo filter** with a machine learning model to efficiently identify potentially fraudulent transactions within financial data. The Cuckoo filter is a probabilistic data structure that enables fast set membership checks, particularly useful for distinguishing between legitimate and suspicious users based on transaction history. With the added integration of a pre-trained machine learning model, this project provides a powerful tool for fraud detection in real-world financial datasets.

## Features
- **Custom Cuckoo Filter**: Implements a from-scratch Cuckoo filter to perform efficient lookups.
- **Machine Learning Integration**: Leverages a pre-trained Random Forest model to classify transactions as fraudulent or legitimate.
- **Flexible User Interface**: Allows manual input to check specific users or runs automatically with test data.

## Installation

1. **Clone this repository**:
   ```bash
   git clone <repository-url>
   cd cuckoo-filter-fraud-detection
   ```
   
2. **Download and Prepare Data**: Ensure that your dataset and model files are downloaded and placed in the correct directories as specified in `test.py`.

## Usage

To use this implementation, follow these steps:

### Step 1: Update File Paths
- Open `test.py` and update the file paths as needed:
  - **`X_1.csv`**: Path to the input financial transaction data.
  - **`random_forest_model.joblib`**: Path to the pre-trained machine learning model.
  - **`top_50_legitimate_users.txt`**: Path to the list of known legitimate users.

### Step 2: Run the Script
Execute the script to test the Cuckoo filter and machine learning model:

```bash
python test.py
```

- When prompted, you can enter a specific user ID to check their legitimacy.
- If no input is provided, the script will default to running a test example with sample data.

## Example Workflow

1. **User Check**: Run the script to enter a user ID and determine if the user is flagged as legitimate or potentially fraudulent.
2. **Automated Test**: Run the script without input to see default behavior with test data.

## Repository Structure

```
├── README.md                               # Project documentation
├── test.py                                 # Main script for testing Cuckoo filter and model integration
├── X_1.csv                                 # Input financial data file
├── random_forest_model.joblib              # Pre-trained ML model for fraud detection
└── top_50_legitimate_users.txt             # List of top legitimate users
```

## Requirements

- **Python 3.x**
- **NumPy**
- **Scikit-learn**
- Other dependencies as listed in `requirements.txt`.

## Implementation Details

- **Cuckoo Filter**: The filter is implemented to store hashes of legitimate users for rapid membership testing.
- **Random Forest Model**: The model predicts the likelihood of fraudulent activity based on transaction features.
- **Integration**: Combines Cuckoo filter results with the model’s output for robust fraud detection.

## Notes

- Ensure all dependencies are installed before running the script.
- Default paths are set in the `test.py` script; modify them according to your file locations.
- This project is flexible for use cases with similar financial datasets and can be adapted for other domains requiring efficient membership testing and fraud detection.

---

Feel free to customize and extend the project to meet your specific requirements!
