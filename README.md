## Sales and Cancellations Report Generator

This repository show a script in Python that create a charts about sales and cancellations from Google Sheet, then generate and export for PDF.

![cancellations](https://github.com/User-Felix/Spreadsheet_analysis/blob/main/cancellations_chart.png?raw=true)

![Sales](https://github.com/User-Felix/Spreadsheet_analysis/blob/main/sales_chart.png?raw=true)


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

**Permissin for access**


Follow the examples below:

Access for anyone

![Acces for anyone](https://github.com/User-Felix/Spreadsheet_analysis/blob/main/projects_images/permission-00.png?raw=true)


Access for read and write

![Acces for read and write](https://github.com/User-Felix/Spreadsheet_analysis/blob/main/projects_images/permission.png?raw=true)

To access for the link, separate the URL:

`https://docs.google.com/spreadsheets/d/158i3c_YcNS2x8qxNv0YselYRqNVvG1gXjaFgkddHgvg/edit?pli=1&gid=1783891337#gid=1783891337`, this is the URL without changing.
Now let's look for code ID:
`158i3c_YcNS2x8qxNv0YselYRqNVvG1gXjaFgkddHgvg`, this part we put in the variable to shearch within the spreadsheet.

```python

    sheets_id = "158i3c_YcNS2x8qxNv0YselYRqNVvG1gXjaFgkddHgvg"
    
    xsl = pd.ExcelFile(f"https://docs.google.com/spreadsheets/d/{sheets_id}/export?format=xlsx")

```
