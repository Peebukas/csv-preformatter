# csv-preformatter

Project Structure
Repository Setup: Initialize your GitHub repository with a clear directory structure.

src/: Contains all the PHP source code.
data/: For storing input CSV files from suppliers.
output/: Where the processed supplier.csv files will be stored.
logs/: To keep track of the operations performed on the CSV files.
tests/: For unit tests and integration tests.
docs/: Documentation of the project.
README.md: Update the README.md in your repository to include:

Project description.
Setup instructions.
Usage guide.
Contribution guidelines.
.gitignore: Include paths like /vendor/, /output/, /logs/, etc., to prevent unnecessary files/folders from being tracked.

Core Components
CSV Parser and Formatter:

PHP classes to read various CSV formats.
Methods to normalize data into a uniform format.
Functions to handle special cases (like merging multiple CSVs from a single supplier).
Orchestration File:

A PHP script (e.g., orchestrator.php) that will be the entry point.
This file will call the necessary functions from the CSV Parser and Formatter based on the configuration or input parameters.
Configuration Management:

A configuration file (e.g., config.json or config.php) to manage supplier-specific rules and formats.
This could include mapping of columns, data transformation rules, etc.
Logging System:

Implement logging for each operation (e.g., file read, data transformed, file written).
Store logs in a structured format in the logs/ directory.
Error Handling and Validation:

Robust error handling for issues like file not found, format mismatch, etc.
Data validation to ensure the integrity of the CSV files.
Cron Job Setup for Automation:

Instructions or scripts to set up cron jobs for regular processing of CSV files.
This includes fetching files from suppliers (if applicable), running the orchestrator, and storing the output.
Development Steps
Initial Setup:

Set up the basic directory structure in your GitHub repository.
Create a basic version of orchestrator.php.
CSV Parsing and Formatting:

Develop the CSV parser and formatter classes.
Start with a single supplier format and gradually add more.
Configurations and Rules:

Implement the configuration management system.
Define the rules for the first few suppliers.
Logging and Error Handling:

Implement the logging system.
Add comprehensive error handling.
Testing:

Write unit tests for each component.
Perform integration testing with actual supplier CSV files.
Cron Job Automation:

Write a guide or script for setting up cron jobs.
Test the automation process.
Documentation:

Document each part of the system.
Update README.md with comprehensive instructions.
Iterative Improvements:

Gradually add support for more suppliers.
Refine the system based on feedback and testing.
Next Steps
Initial Repository Setup: If you haven't already, set up the basic directory structure and initial files in your GitHub repository.
First Component Development: Start with developing the CSV parser and formatter for a single supplier format.
