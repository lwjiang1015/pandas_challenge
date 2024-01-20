# pandas_challenge

## Preparation 
Following the instructions, (1) a new repository called "pandas challenge" was created and cloned to my laptop (2) a folder named "PyCitySchools" was created in the local Git repo; (3) The Jupyter notebook for this project named "mainscript" was added into the repo; (4) all the above had been pushed to GitHub before the analysis was started.

The zipped files were downloaded and the data files were added in the folder "Resource" in the local Git repo.

## The Process for the Analyses

Used the code starter as a guide, set up the dependencies, read and merge the csv data files.

### Local Government Area Summary
Calculated the following: "Total number of unique schools", "Total students", "Total budget", "Average maths scores", "Average reading scores", "% passing maths", "% passing reading", "% overall passing".

Created a new DataFrame for the above calculations called "area_summary"

### School Summary
Use the school complete dataset to get the variables school type and total student count (size). 

Calculated the following: the per capita spending, the average test scores per school, the number of students with maths scores of 50 or higher by school, the number of students with reading scores of 50 or higher by school, the number of students that passed both maths and reading by school, and thereof, the passing rates.

Created a new DataFrame "finalmerged_school_summary"

Tided up the finalmerged_school_summary to match the screenshot in the starter script by deleting the unpresented columns (numberpassingmaths, numberpassingreading and numberpassingoverall) and sort by school_name

The final school summary DataFrame after formatting the column names called "formatted_school_summary_sorted"


### Highest-Performing Schools by Percentage of Overall Passing

Sorted the schools in the "per_school_summary" by % Overall Passing in descending order and saved the results to a DataFrame "top_schools"

Displayed the first 5 rows

### Lowest-Performing Schools by Percentage of Overall Passing

Sorted the schools in the "per_school_summary" by % Overall Passing in ascending order and saved the results to a DataFrame "bottom_schools"

Displayed the first 5 rows

### Maths Scores by Year

Used codes to seprate the data by year
Grouped by "school_name" and take the mean of each
Used the code to select only the maths_score
Combined each of the scores by year into single DataFrame "maths_scores_by_year"

### Reading Scores by Year
Used codes to seprate the data by year
Grouped by "school_name" and take the mean of each
Used the code to select only the reading score
Combined each of the scores by year into single DataFrame "reading_scores_by_year"

### Scores by School Spending

Used pd.cut to bin the data by the spending ranges given
Used the code provided to calculate the averages
Created the DataFrame "spending_summary" using the binned and averaged spending data

### Scores by School Size

Used pd.cut to bin the data by the school sizes provided
Used the code provided to calculate the averages
Created the "size_summary" DataFrame using the binned and averaged size data

### Scores by School Type
Grouped the per_school_summary DataFrame by "School Type" and averaged the results
Used the code to selet the new column data
Created a new DataFrame "type_summary" for the new data

### Written Report
summarised the analysis
drew two most strking conclusion from the analysis with the limitation acknowledged

## References/acknowledgement
This assignment has been completed primarily with reference to the course materials for Module 4. The help from the teaching team and from the Xpert Learning Assistant at Datacampspot are acknowledged. 
