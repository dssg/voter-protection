## What's In the Folder?
* (LIVE) Voter Risk Toolkit.xlxs : Main spreadsheet for Tableau and Excel analysis
* risk_processing_public.ipynb: Jupyter markdown that cleans and processes data sources into single csv with county as the unit of analysis
* get_census.ipynb: Markdown to retrieve relevant Census data (using the censusdata package)

Sheets Included:

* Methodology: Details about how the spreadsheet works
* Data with Headers: Data with Helpful headers
* Data with No Headers (DEFAULT for Tableau)
* Actions and Urgency: Decision Matrix for recommended action
* All States Risk Data: Extended, raw data for 42 states (to be expanded at later update)
* NA Summary


## How Can I Modify This?

* ***Do you like our data, but have different actions?***
  * Navigate to  the Actions and Urgency Sheet
  * Update the Decision Matrix based on your interventions 
  * VLOOKUP will automatically populate the  recommended actions based on your entries

* ***Interested in other county data?*
  * Scroll to far right of sheet to see if any of the additional data suits you:
    * "Additional Context" section includes more voter, demographic, and county data which is available for plug-and-play
    * Can also join data to this file using five-digit FIPS Code
  * Substitute columns if desired, change metrics of interest, and adjust formulas if needed to account for new categories
  * In Tableau, change the variables selected in each sheet accordingly

* ***"My data is at precinct level  /  I have better data than you."*
  * Reference the Python script to use, change, and modify what we have to suit your needs. 
  * Fuller FIPS Code data also available
  * Amend the keep_vars list at the end of the markdown to change what columns are ultimately selected
  

* ***"Excel formulas irk me. I would rather generate these entire csvs using Python scripts."*
  * Full processing script will be shared for easier plug-and-play on August 14th.

* ***"When can we expect the template for  all states?"
  * Next update loosely scheduled for August 14th.
  
* ***"Show me the data."*
You got it. The toolkit itself can be directly downloaded from the Toolkit link.


| Data Source | Description | Years | Link
| --- | --- | --- | --- |
| Election Administration and Voting Survey (EAVS) | Provides county-level election data about the resources, local characteristics, and infrastructure for U.S. elections. | 2016 | https://www.eac.gov/research-and-data/datasets-codebooks-and-surveys |
| The Cooperative Congressional Election Study (CCES) | Provides information about political attitudes and voter election experience | 2016 | https://cces.gov.harvard.edu/data 
| American Community Surveys (ACS) | Provides community characteristics of U.S. residents. | 2018 |  https://www.census.gov/
