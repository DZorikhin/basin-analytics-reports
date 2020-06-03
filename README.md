# US shale basins activity interactive reports

The reports created by this script analyze USL48 basin oil &amp; gas assets, operating companies, production, capex, rigs deployed, and the number of new wells brought online, looking back at the past four quarters and looking forward to the next four quarters. 

There are 8 onshore shale basins under analysis: Permian, Appalachia, Eagle Ford, Williston, DJ Basin, Mid Continent, East TX/Haynesville, Rockies.

Check attached files to see the example data.

General automated ETL process for report creation:
1. Download datasets from AWS S3 bucket
2. Data manipulation and preparation
3. Uploading back to AWS S3:
  - data files in **_.xlsx_** format to be attached to report
  - **_html_** template to be pasted in the report to display interactive Plotly graphs
  - **_JavaScript_** code to be used by html template
  - **_PDF_** files with graphs for general metrics and all companies to be attached to report
4. Create interactive report using cloud-native platform and prepared data
