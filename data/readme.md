## What's In the Folder?

* [risk_processing_public.ipynb](risk_processing_public.ipynb): Jupyter notebook that cleans and processes data sources into single csv with county as the unit of analysis
* [get_census.ipynb](get_census.ipynb): Jupyter notebook to retrieve relevant Census data (using the censusdata package)
* [risk_scoring_for_toolkit.ipynb](risk_scoring_for_toolkit.ipynb): Script to select metrics, indicators, and states to generate scores for Tableau
* [(LIVE) Voter Risk Toolkit.xlsx] : Default (interactive) spreadsheet generated for Voter Protection  Corp (limited changeability).

Sheets Included in the excel spreadsheet:

* Methodology: Details about how the spreadsheet works
* Data with Headers: Data with Helpful headers
* Data with No Headers (DEFAULT for Tableau)
* Actions and Urgency: Decision Matrix for recommended action
* All States Risk Data: Extended, raw data for 42 states (to be expanded at later update)
* NA Summary: Summary of what data is available for each state


## How Can I Modify This?
To use the toolkit in Tableau, edit your Data Connection to link to the downloaded (ANALYSIS) spreadsheet.

* ***Do you like our data, but have different actions?***
  * Navigate to  the Actions and Urgency Sheet
  * Update the Decision Matrix based on your interventions 
  * VLOOKUP will automatically populate the  recommended actions based on your entries

* ***Interested in other county data?***
  * Scroll to far right of sheet to see if any of the additional data suits you:
    * "Additional Context" section includes more voter, demographic, and county data which is available for plug-and-play
    * Can also join data to this file using five-digit FIPS Code
  * Substitute columns if desired, change metrics of interest, and adjust formulas if needed to account for new categories
  * In Tableau, change the variables selected in each sheet accordingly

* ***"My data is at precinct level  /  I have better data than you."***
  * Reference the Python script to use, change, and modify what we have to suit your needs. 
  * Fuller FIPS Code data also available
  * Amend the keep_vars list at the end of the markdown to change what columns are ultimately selected
  

* ***"Excel formulas irk me. I would rather generate these entire csvs using Python scripts."***
  * See the risk_scoring_toolkit markdown 

* ***"When can we expect the template for  all states?"***
  * States to be added:  Alaska, Connecticut, Illinois, Massachussetts, Maine, New Hampshire, Rhode Island,  South Dakota,  and Vermont
  
* ***"Show me the data."***

[You got it.](https://dssg.github.io/voter-protection/toolkit.html)


| Data Source | Description | Years | Link
| --- | --- | --- | --- |
| Election Administration and Voting Survey (EAVS) | Provides county-level election data about the resources, local characteristics, and infrastructure for U.S. elections. | 2016 | https://www.eac.gov/research-and-data/datasets-codebooks-and-surveys |
| The Cooperative Congressional Election Study (CCES) | Provides information about political attitudes and voter election experience | 2016 | https://cces.gov.harvard.edu/data 
| American Community Surveys (ACS) | Provides community characteristics of U.S. residents. | 2018 |  https://www.census.gov/
