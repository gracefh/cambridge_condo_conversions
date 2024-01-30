# data-vis-society-data-cleaning

Contains data for looking at condo conversions in the greater Boston area from 2015 to 2024.

The parcel data folder contains information from [Cambridge GIS](https://github.com/cambridgegis/cambridgegis_data/tree/main/Assessing), and each corresponding file's README also contains information about the data fields. ([TODO] add this to this GitHub as well)

We counted condo conversions as addresses that had one parcel associated with it in one year but multiple parcels associated with it in the next year. For example, if an address had 1 entry in 2015's parcel data but 13 in 2016's parcel data, it is counted as a condo conversion in 2015.

Relevant files:
* `condo_conversions.csv`: Uses above logic to merge information about condo conversions with geographic information about each address.
* `data_cleaning.ipynb`: Contains all the code for doing the data wrangling

