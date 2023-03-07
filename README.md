# cofactor-figure-data
files containing the data and code to reproduce the figures in the review.
Requires the following dependencies:
```
pip install pandas
pip install plotly 
pip install rpy2
```
NOTE: 
the file containing all data including all the GO terms called `uniprot-all-GO-2023.02.14-14.57.31.27.tsv` 
has not been added due to the fact that its filesize exceeds the github limit of 50Mb.
if you want to reprocess the data, the file can be recreated by searching (reviewed:true) on the uniprot database and downloading all proteins as a .tsv,
making sure Entry name, EC number, GO terms and and cofactor are included as columns.  
replace `uniprot-all-GO-2023.02.14-14.57.31.27.tsv` in the script with your new filename. The other files can similarly be recreated. The uniprot search terms on which they are based are included as comments in the notebook. 

the figures can still be created by skipping the third cell where the processing is done and just loading in the processed dataframe using the cell below
