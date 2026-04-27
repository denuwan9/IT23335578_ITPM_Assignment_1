# Sinhala Transliteration Accuracy Testing - Assignment 1

## Objective
This project evaluates the accuracy of the Chat Sinhala transliteration function on [pixelssuite.com/chat-translator](https://www.pixelssuite.com/chat-translator). It identifies 50 failure scenarios across 24 Singlish input types.

## Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

## Installation
1. Clone the repository to your local machine.
2. Install the required dependencies:
   ```bash
   pip install playwright openpyxl
   ```
3. Install the Playwright Chromium browser:
   ```bash
   python -m playwright install chromium
   ```

## Running the Tests
To run the automated test suite, ensure you have an Excel file named `IT23335578_Assignment 1 - Test cases.xlsx` or `New_Test_Cases.xlsx` in the project folder.

### 1. Basic Execution (Visible Browser)
If you want to watch the automation type the Singlish and capture the Sinhala output:
```bash
python test_automation.py
```

### 2. Headless Execution (Background)
To run the tests quickly in the background:
```bash
python test_automation.py --headless
```

### 3. Custom File Execution
To run the script on a specific Excel file:
```bash
python test_automation.py --excel "Your_Custom_File.xlsx" --headless
```

## Features
- **Automatic Header Detection**: The script automatically finds the correct columns for Input, Expected Output, Actual Output, and Status.
- **Rationale Generation**: Automatically populates the "Evidence or rationale" column based on the "Singlish input types covered" category.
- **Merged Cell Support**: Handles merged cells in Excel files commonly used in assignment templates.

## Deliverables
- `IT23335578_Assignment 1 - Test cases.xlsx`: The completed Excel report with 50 failure cases and rationales.
- `test_automation.py`: The enhanced Playwright automation script.
- `README.md`: Instructions for setup and execution.
- `Git_Link.txt`: Link to the public Git repository.

## Registration Number
IT23335578
