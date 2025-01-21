## Sales and Cancellations Report Generator

This repository show a script in Python that create a charts about sales and cancellations from Google Sheet, then generate and export for PDF. 

**Key Features:**

* Reads data from a specified Google Sheet.
* Separates data into sales and cancellations.
* Creates bar charts for sales and cancellations using matplotlib.pyplot.
* Generates a PDF report with the charts using reportlab.
* Includes report title and generation timestamp in the PDF.

**Libraries Used:**

* pandas: For data manipulation and reading Excel files.
* matplotlib.pyplot: For creating and plotting charts.
* reportlab: For generating PDF documents.


**Usage:**

1. **Replace `sheets_id` with the actual Google Sheet ID.**
2. **Modify the sheet name (`'Semana_one'`) if necessary.**
3. **Run the script.**
4. The script will generate a PDF file named "output.pdf" in the same directory.

**Note:**

* This script requires the installation of the following libraries: pandas, matplotlib, reportlab.
If you using github codespace, well be necessary installing whit pip `openpyxl`.
* The Google Sheet must be publicly accessible or have appropriate sharing permissions.

