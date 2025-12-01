# Linkedin-connections-cleaning
This repository contains a Jupyter notebook and analysis report for processing and analyzing 126 CSV files from a LinkedIn assignment focused on data cleaning and graph-based ranking of unique keys.

#Features
Batch CSV Cleaning: Processes multiple CSV files by standardizing columns to "First Name", "Last Name", "Company", removing empty rows, extra whitespace/quotes, and duplicate headers.

Inverse Graph Ranking: Ranks keys (e.g., names like "Ramraj Nagar" scoring 1805.09) by uniqueness, where contributions are calculated as 1/n for names appearing in 
n keys.

Graph Path Analysis: Compares pruned graph shortest paths (shorter, lower variability) against random walks (longer, higher variability) using statistical metrics and visualizations.

# Files
  linkedin_data_cleaning_code:  Python notebook with clean_row(), clean_csv_file(), and batch_clean_folder() functions for handling uncleaned CSV data from input to output folders.
  
  Linkedin-Assignment-Analysis.pdf: PDF report detailing top unique keys, ranking methodology, and pruned vs. random walk path length comparisons.

# Usage
  Place uncleaned CSV files in an UncleanedFiles folder.
  Run batch_clean_folder("UncleanedFiles", "CleanedFiles") in the notebook to generate standardized outputs.​
  Refer to the PDF for analysis insights on the processed data.

# Requirements
Python 3.x
Standard libraries: os, csv
