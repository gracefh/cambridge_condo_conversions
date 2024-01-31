# data-vis-society-data-cleaning

Contains data for looking at condo conversions in the greater Boston area from 2015 to 2024.

The parcel data folder contains information from [Cambridge GIS](https://github.com/cambridgegis/cambridgegis_data/tree/main/Assessing), and each corresponding file's README also contains information about the data fields. 

For example you can find the readme.md data for FY2015 [here](https://github.com/cambridgegis/cambridgegis_data/tree/main/Assessing/FY2015/FY2015_Parcels). The raw data that we used for FY2015 can be found [here](https://github.com/cambridgegis/cambridgegis_data/blob/main/Assessing/FY2015/FY2015_Parcels/ASSESSING_PropertyDatabase_FY2015.csv). We also included all the datasets in the folder parcel data in this github repo. 

We counted condo conversions as addresses that had one parcel associated with it in one year but multiple parcels associated with it in the next year. For example, if an address had 1 entry in 2015's parcel data but 13 in 2016's parcel data, it is counted as a condo conversion. We also only kept the first entry of the convered condos, i.e. out of the 13 entries in 2016 parcel data, we only keep the top entry (without having sorted in anyway). 

Relevant files:
* `condo_conversions.csv`: Uses above logic to merge information about condo conversions with geographic information about each address.
* `identify_condo_conversion.ipynb`: Contains all the code with comments for doing the data wrangling



