# Clearwater-Hurricane-Response


Clearwater Address Geocoding and Mapping
This Jupyter Notebook project automates the geocoding of addresses in an Excel file by generating latitude and longitude coordinates using the geopy library. The resulting data, enriched with geolocation information, is then saved to a new Excel file. This project is useful for location-based data analysis, mapping, and field inspection planning.

Features
Automated Geocoding: Reads addresses from an Excel file, converts them into geographic coordinates, and appends these as new columns.
Error Handling & Logging: Implements detailed logging and error handling to monitor each step of the geocoding process.
Data Export: Saves the updated data, complete with latitude and longitude coordinates, to a new Excel file for easy access and further analysis.
Getting Started
Prerequisites
Make sure you have the following installed:

Python 3.7+
Jupyter Notebook
Required Python libraries:
geopy
pandas
openpyxl
logging
Install the necessary libraries using the following command:

bash
Copy code
pip install geopy pandas openpyxl
Installation
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/yourusername/clearwater-geocoding.git
cd clearwater-geocoding
Open the Jupyter Notebook:

bash
Copy code
jupyter notebook Clearwater_Geocoding.ipynb
Update the file_path variable with the path to your Excel file (or place your file in the same directory and adjust the code accordingly).

Usage
Load the Notebook: Open the notebook in Jupyter and run each cell sequentially.
Specify the File Path: Update the file_path variable in the notebook with the correct path to your Excel file containing the addresses.
Run the Geocoding Process: Execute the geocoding function to generate latitude and longitude columns based on the address data.
Save the Output: The notebook will save the updated file with geolocation data to your specified output path.
Example File Structure

plaintext
Copy code
├── Clearwater_Geocoding.ipynb
├── Scrubbed_Helene_Data_PRINT.xlsx  # Input Excel file with addresses
└── Geocoded_Data.xlsx               # Output Excel file with coordinates


Troubleshooting
KeyError for Missing Columns: Ensure the column name in the Excel file matches the one specified in the code (address_column variable).
Rate Limiting: If the geocoding process is rate-limited, adjust the delay in the add_geocode_data function.

Contributing
Feel free to open issues or submit pull requests for new features or bug fixes.

License
This project is open-source and available under the MIT License.

Acknowledgments
The geopy library for geocoding services.
Jupyter Notebook for interactive code execution and visualization.
