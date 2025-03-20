# data-tools

## Data Transformer 

The 'shape' of data preferred for larger data-sets is commonly different to that used for spreadsheets.  This tool is built to transform a structure preferred by data analysis tools (like PowerBI, Looker Studio, Tableau etc) into a structure that is easier to work with in spreadsheets (like Excel, Google Sheets etc).

Data analysis typically uses a modelling approach where columns represent dimensions and measures and rows are instances. A dimension is an attribute of an event in the table such as a location or some other descriptive identifier. A measure is the numeric value (fact) of the event that we will be performing a mathematical calculation on (e.g. summing).  A [deeper overview of dimensional modelling](https://www.kimballgroup.com/data-warehouse-business-intelligence-resources/kimball-techniques/dimensional-modeling-techniques/) is not hard to find. 


In regular spreadsheets this sort of modelling is harder to lay out. Typically in a spreadsheet table you have a column for one of the x and y axis, and a column per series for the alternate axis. For a time-series data-set one of those columns will be for the time of each event which only leaves a single column per series for the measure. The possibility to have descriptive or shared data between series is harder to achieve.

In the transformation this tool provides the dimensions are used to construct the series names which become permutations of each combination of dimension. You can copy this into a spreadsheet, highlight the cells and the auto-chart workflow should work easily enough.

An online usable demonstration of this is available here: 
[https://toobstar.github.io/data-tools/](https://toobstar.github.io/data-tools/)
