This folder contains three jupyter notebooks and two excel files which used together enable the user to calculate the consumption intensity of the representative products considered in the Mobility Basket of Products (BoP) within the average european citizen consumption footprint by country project.

data_inputs.ipynb: It contains four functions: read_file, filter_file, inventory_dtype and population, which are to be use for loading additional information from sources different from PRODCOM and COMEXT for which the pyhton package eurostat will be used.

        -> read_file, filter_file and inventory_dtype are focused on excel and csv files.
        -> population extracts information on population per country and year from EUROSTAT.
        
predownload.ipynb: It contains five functions which perform a number of operations (e.g filtering names, checking repeted product codes, converting country codes from one system to another etc) that take place before the actual downloading the data from EUROSTAT (for FAO data a different set of functions is used). These functions are therefore never to be run alone but within other functions.

mob_frame.xlsx: A frame table with the transport groups and subgroups and their features and which fields are to be filled out by the bop_mobility.ipynb.


pb2019-section23.xls: One of the sections of the EC Mobility and Transport Statistical Pocketbook (https://ec.europa.eu/transport/facts-fundings/statistics/pocketbook-2019_en) from which bop_mobility.ipynb will extract data.

bop_mobility.ipynb: script containing the functions required to calculate the Mobility BoP products consumption intensity.

