# GDPR Cookie Compliance Checker for .edu Domains

This open-source tool analyzes a list of website URLs (e.g., .edu domains) to detect and report on GDPR cookie-consent compliance.

## Features

- Automated crawling and detection of cookie banners
- Input and output through CSV files
- Designed for reproducibility and practical use by researchers or university IT staff
- Lightweight, configurable, and easy to run

---

## How to Use

Follow these steps to set up and run the tool:

### 1. Download the Code

Download this repository as a ZIP file and extract it, or clone it using Git.

### 2. Install Python and a Code Editor

Ensure that Python 3.8 or higher is installed on your machine.  
You can use any Python-compatible code editor such as Visual Studio Code.


### 3. Download ChromeDriver

- Download the Chrome WebDriver that matches your installed version of Google Chrome.
- After downloading, extract the file and locate the full path to `chromedriver.exe`.

### 4. Prepare Your Input File

Create a `.csv` file (e.g., `urls.csv`) containing the list of URLs you want to analyze, with one URL per line. Example:
http://harvard.edu
http://mit.edu
http://psu.edu


### 5. Update Paths in the Script

In the Python script (e.g., `analyze_urls.py`), update the following variables:

- `chrome_driver_path`: full path to your `chromedriver.exe` file
- `input_file_path`: path to your input `.csv` file
- `output_file_path`: path to save the output results file

### 6. Run the Tool







