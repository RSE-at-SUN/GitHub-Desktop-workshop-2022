# A suggested structure for tracking scripts related to a paper

Testing structure for tracking/organizing scripts that create plots/tables for publications:

* All data in a single 'data' folder (_or loaded directly by scripts in this repo from another online repository_)

* One folder for each small script that produces a plot and/or table (_keeping separate analyses separate as much as possible_), with outputs from each script kept in the same folder.

* This README file to show the figures (and links to tables) intended to go in a paper, ordered by paper section, and including the intended Title and Caption (_click on the dropdown at the topleft to get a quick overview via the TOC_).

Editing the publication draft 'body' text happens in an appropriate platform (e.g. using track changes in Word), but only links to figures/tables in GitHub[^footnote1] are included in the draft while analysis/formatting is ongoing (_i.e. avoid pasting a figure/table into the text if it might need to be changed later_).

When analysis is complete, and plots/tables are in their final form, they can then be incorporated with main text[^footnote2].


Key thing: ***every plot/table is kept with the script that made it***, so it can be inspected/corrected easily if need be (_click on the link/figure, and then open the containing folder to see - and comment on - the script that generated it_); no time wasted trying to paste every new version of a plot into the Word doc (and probably making mistakes with versions).


## Paper

_Should include details about the paper here - e.g. the running title, where to find the draft, a basic summary, etc. .. when the paper is published, this can be updated, and the repo can be made public (if desired) to share the code used in the paper._


## Datasets

_Some basic information about the data used should go here._

The results below have been generated using a sample of a full survey dataset; the dataset was suggested in this Data Carpentry lesson: https://datacarpentry.org/R-ecology-lesson/02-starting-with-data.html

The sample data is stored in the data folder, [here](data/survey_sample.csv).

The full dataset can be found [here](https://ndownloader.figshare.com/files/2292169).


## Results

### Counts of species in most diverse genera - table

Title: Counts of species observed in the three most diverse genera

[species count table](output_species_count/species_counts_table.csv)


### Counts of species in most diverse genera - plot

Title: Relative counts of species observed in three most diverse genera

Caption: Species counts were conducted as per the methodology described in the Methods section. The three genera with the most observed species were considered 'diverse', with relative counts shown here.

![species count barplot](output_species_count/species_counts_barplot.png)


[^footnote1]: To get the link to a subheading in this README, move the mouse to the left of the subheading and right-click on the chain-link icon that appears, and then select 'Copy link address'. To link directly to the figure/table, click on the appropriate figure/table link in this README (or navigate to its position in the repo), and then copy the URL from the navigation bar.

[^footnote2]: To transfer tables into Word in preparation for publication, open the csv file in Notepad (if on your computer, else look for the 'Raw' button in GitHub), copy and paste the contents into Word, and do the following: select the text that you want to convert, and then click Insert > Table > Convert Text to Table; in the Convert Text to Table box, choose the options you want. Under Table size, make sure the numbers match the numbers of columns and rows you want. 
