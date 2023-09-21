# README.md

This is a Python script that reads CSV and image files, merges the CSV data into a workbook, and inserts images from the image files. The resulting workbook has multiple worksheets, where each worksheet represents a different run or image type.

## Prerequisites

* Python 3.x
* pandas
* openpyxl

## Getting started

To use this script, first clone the repository to a local directory. You can do this by running the following command in your terminal:

```
git clone https://github.com/<username>/csv_image_workbook.git
```

After cloning the repository, navigate to the `csv_image_workbook` directory and run the following command to install the required dependencies:

```
pip install -r requirements.txt
```

## Usage

To use this script, run the following command in your terminal:

```
python main.py
```

The script reads CSV and image files from the `data` directory, merges the CSV data into a workbook, and inserts images from the image files. The resulting workbook is saved as `merged_data.xlsx` in the `output` directory.

## How it works

1. The script reads the CSV files in the `data` directory and creates a pandas DataFrame for each file.
2. The script reads the image files in the `data` directory and creates a dictionary of PIL Image objects, where the keys are the filenames without extensions.
3. The script loops through each image in the dictionary and adds it to the corresponding worksheet in the workbook.
4. The script saves the workbook to the `output` directory.
