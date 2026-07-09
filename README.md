# CLI Data Analyzer

A command-line tool to instantly analyze any CSV dataset — get column info, statistics, and categorical breakdowns without opening Excel or writing a single line of analysis code.


## Features

- Instant summary of any CSV — shape, column types, missing values
- Statistics for all numeric columns — mean, median, min, max, standard deviation
- Value counts with bar chart for categorical columns
- Configurable row preview
- Export summary to a text file
- Clean error handling for missing files

## Installation

```bash
git clone (https://github.com/Satya-Gogia/CLI-data-analyzer-with-stats-and-argparse)
cd cli-analyzer
pip install pandas tabulate
```

## Usage

```bash
# Basic analysis
python analyzer.py data.csv

# Show 10 rows instead of 5
python analyzer.py data.csv --rows 10

# Skip the stats section
python analyzer.py data.csv --no-stats

# Skip the row preview
python analyzer.py data.csv --no-preview

# Export summary to a file
python analyzer.py data.csv --export summary.txt
```

## Tech Stack

- Python 3
- pandas — data loading and analysis
- tabulate — formatted terminal output
- argparse — CLI interface

## What I Learned

- Reading and parsing CSV files with pandas
- Separating numeric vs categorical columns programmatically
- Building a proper CLI with argparse flags
- Handling edge cases — missing files, empty columns, no numeric data

## Sample Data

A `sample.csv` is included so you can test the tool immediately after cloning
