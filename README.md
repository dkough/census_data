# census_data

Note:  1. You must have your own Census API key, I have removed mine from the uploaded notebooks.         
       2. Create a folder called "excel" and another called "acs5_data" in the directory where you store the notebooks, or change the filepaths however you see fit.
       
These notebooks gather demographic, income, education, and business data at the zip code and county level using Census APIs as well as scraping zip-codes.com.  
The variables are defined in a text document I've uploaded.
Not all of the variables are used, and not all of them may be of interest to you.

How it works is, you select the zip codes you wish to gather information on, and enter them into the zip code txt files, "chosen_zips.txt" and "chosen_zips_2000.txt".
The reason there are two files is that I've found many zip codes have been created since the year 2000, which causes errors.

Then, you select the variables you wish to use and paste them into the "variables_2013.txt" and "variables_2018.txt" files.  Some variable codes are the same however
they do change between APIs, scroll down and see the heading 'Variable Changes' here https://www.census.gov/data/developers/data-sets/acs-5year.html.
Only place one zip code or variable per line.  Do not leave any empty lines.

The town_names file is where you input the names of the geographies and locations the zip codes encompass. 

The webscraping does not use variables but instead looks for matching text.  The tables on zip-codes.com do not have unique identifiers, which is why this webscrape takes
the entire page, and is very slow.

I hope this helps you complete whatever project you're working on.
