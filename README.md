README
# Module 5 Challenge<br>

* In this assignment, we were tasked with generating tables and figures needed for the technical report of an animal study on the performance of Pymaceuticals’ drug, Capomulin, against the other treatment regimens on 249 mice. Over the course of 45 days, tumor development was observed and measured. Included is my python code and analysis. <br>
* I utilized previous class activites as well as these websites https://www.geeksforgeeks.org/matplotlib-pyplot-gca-in-python/ and https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.agg.html in order to write my code. <br>

# Instructions<br>
This assignment is broken down into the following tasks:<br>

## Prepare the data.<br>
* Generate summary statistics.<br>
* Create bar charts and pie charts.<br>
* Calculate quartiles, find outliers, and create a box plot.<br>
* Create a line plot and a scatter plot.<br>
* Calculate correlation and regression.<br>
* Submit your final analysis.<br>
* Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.<br>

* Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.<br>

* Display the updated number of unique mice IDs.<br>

## Generate Summary Statistics<br>
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.<br>

Your summary statistics should include:<br>

* A row for each drug regimen. These regimen names should be contained in the index column.<br>

* A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.<br>

## Create Bar Charts and Pie Charts<br>
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.<br>

* Create the first bar chart with the Pandas DataFrame.plot() method.<br>

* Create the second bar chart with Matplotlib's pyplot methods.<br>

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.<br>

* Create the first pie chart with the Pandas DataFrame.plot() method.<br>

* Create the second pie chart with Matplotlib's pyplot methods.<br>

## Calculate Quartiles, Find Outliers, and Create a Box Plot<br>
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:<br>

* Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.<br>

* Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.<br>

* Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.<br>

* Determine outliers by using the upper and lower bounds, and then print the results.<br>

* Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.<br>


## Create a Line Plot and a Scatter Plot<br>
* Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.<br>

* Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.<br>

## Calculate Correlation and Regression<br>
* Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.<br>

* Plot the linear regression model on top of the previous scatter plot.<br>




