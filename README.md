# CSV Data Processing Script

## Description

This Python script processes a CSV file containing user data, performing extraction, transformation, and loading (ETL) operations. It cleans and validates the data, handles missing values, detects duplicates, and logs the processing steps. The script splits the cleaned data into multiple files and merges them into a final output file.

## Features

- Extracts data from a semi-colon delimited CSV file.
- Cleans and validates email addresses.
- Handles missing data and duplicates.
- Splits the output into multiple chunks for easier management.
- Logs the processing steps and errors for tracking.
- Merges cleaned chunks into a final output file.

## Requirements

- Python 3.x
- pandas library
- re (regex library, included in standard Python library)
- os (operating system library, included in standard Python library)
- logging (included in standard Python library)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
   ```

2. Install the required libraries:

   ```bash
   pip install pandas
   ```

## Usage

1. Place your input CSV file in the desired directory and update the `input_file` variable in the script with the path to your input file.
2. Customize the `output_file` and `garbage_file` variables as needed.
3. Run the script:

   ```bash
   python your_script_name.py
   ```

4. After execution, you will find:
   - A cleaned output file named as specified in the `output_file` variable.
   - A garbage file containing records with issues.
   - Temporary chunk files created during processing (optional to remove).

## Logging

The script logs significant events such as:
- Successful extraction of data.
- Errors encountered during processing.
- Saving of cleaned data and invalid records.

Log messages will be printed to the console and can be reviewed for tracking the processing flow.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any enhancements or bugs.

1. Fork the repository.
2. Create a new branch for your feature/bug fix.
3. Make your changes and commit them.
4. Push to your branch and open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
