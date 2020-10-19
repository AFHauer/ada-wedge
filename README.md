# Applied Data Analytics
## Wedge Project
Created with Python v 3.8.3 in Jupyter Notebook

### Task 1
Files:
	Task1_a_Wedge-Full-Clean.ipynb
	Task1_b_Wedge-Upload-GBQ.ipynb

Builds a Reporting Database in Google Big Query

Task 1 a:
	Cleans the Wedge Zip files

Notes:
	The Task1_a_Wedge-Full-Clean.ipynb this program unzips Wedge data after the initial data is unzipped into 
	a WedgeZipFiles directory. The unzipped data is then cleaned and consitent comma dilineators are installed.
	The headers are consistently created across all Wedge csv files.

Task 1 b:
	Uploads cleaned Wedge files to Google BiqQuery for SQL evaluation
	
Notes:
	The Task1_b_Wedge-Upload-GBQ.ipynb program sets up the Python connection to GBQ and uploads the cleaned
	Wedge files to BiqQuery.

### Task 2
Files:
	Task2_Wedge-Sample of Owners.ipynb

Task 2:
	Create a Python Script which:
		1) Connects to my GBQ instace, created in Task 1
		2) Builds a list of Wedge Owners
		3) Samples that list
		4) Extracts all records associated with the sampled owners of the Wedge and writes them to a 
			local text file.
	

### Task 3
Files: 
Task3_Wedge-Summary-Tables.ipynb

Task 3:
	Create Python code whic creates summary tables and builds a database which reads those summary tables
	
Notes:
	Summary tables:
		1) Sales by Date by Hour: determines the total spend in the store, number of transactions, and the number of 
			items sold.
			1.1) Output file: Sales_by_Date_by_Hour.txt
		2) Sales by Owner by Date: determines the total spend by owners in the store by number of transactions, and 
			items sold.
			2.1) Output file: Sales_by_Owner_by_Date.txt
		3) Sales by product description by date: determines the total spend by Product description, date, number of transactions,
			and items.
			3.1) Sales_by_Product_by_Date.txt
			
			
## Feedback

First, nice README. Really helped me put together the submisison document. 

Part 1 looks good. One note is to try to keep your code to no more than 80 columns wide. You've got some lines that are 
longer than that when you add on the comments. I'm shocked you've stuck with these crazy long folder names on your harddrive. 
Arguably you could have deleted your test cells in Part 1 B, but don't sweat it.

Part 2: resubmit this without that giant printing to the screen. Also, this code is messed up: 
```
# print the random sample results 
for onwner in sample :
    print(sample)
```
You're re-printing your sample for every "onwer" in the data. Clean that stuff up and then resubmit, everything
else looks good. Remember to re-read the submission guidelines!

I'd suggest on Part 3 that you change to all lowercase for table names and fields. I won't ask you to 
resubmit, but having these upper and lower case text is a recipe for sorrow. 

Almost done. Just fix part 2, commit-and-push, and slack me a link to the repo.



