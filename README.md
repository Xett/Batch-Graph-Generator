# Batch Graph Generator
This is a template to easily load an excel file, merge all specified sheets, transform the data then graph it.

# Requirements
Install - [Anaconda3](https://www.anaconda.com/distribution/)

Launch Jupyter Notebook via Anaconda

# Usage
## Variables
Set the name of the excel file via datasetFileName omitting the file extension.

Set the column names of the dataset via columnNames.

Set the sheet names of the excel file via sheetNames.

Set any data cleaning replacements via dataCleanDict.

## Create Graph Datasets
Use selectByValue(dataset,columnName,value/s) to return select parts of the dataset. value can also be a list, for multiple values.

Use splitByColumnValue(dataset,columnName) to split the dataset by the unique values in a column.

Create 1 dataset per graph.

## Create Graph Definitions
Create as many titles as there are datasets to be graphed.

Set the x and y axis labels via xlabel and ylabel.

Set the x and y columns to be graphed via x and y.

Set the column to be the legend via hue.

Use createSetGraphDefs to create graph definitions

## Combine all Graph Definitions
Set graphDefs to be all the outputs of createSetGraphDefs added together
