High-level data cleaning steps for Excel   

### 1) Finding and removing duplicate data
  - One quick way to **identify** duplicate rows is to first select the entire range of data (using CTRL+A works well for this). Then, you would go to Data, Sort & Filter, Advanced. Check the box in the lower left that says 'Unique records only'.  
  - To actually **remove** the duplicate rows from the workbook, you'd again select the entire range (using CTRL+A), then go to Data, Data Tools, Remove Duplicates
 
### 2) Finding and removing extra spaces
  - In a temporary cell, you would type in the formula =TRIM(L2) and copy it all the way down the rows by double-clicking on the fill handle
  - Then you would copy all the cell values in the temporary range and then paste them "as values" over the values in the original column
    
### 3) Separating data without delimiters 
  - Use formulas LEFT, RIGHT, and MID
  - Syntax examples: =RIGHT(A5,7), =LEFT(A5,7), =MID(A5,4,7)
    
### 4) Correcting inaccurate or irrelevant data   
  - Use find & replace to fix inconsistencies (ie. "f" instead of "false")
  - Delete irrelevant data (save a copy of the original)  
    
### 5) Updating missing or incomplete data  
  - Fill in data if it makes sense (ie. if the surrounding data is all consistently the same)
  - See if blanks can be filled with a pattern in the surrounding data (ie. all the dates are 7 days apart)
  - Or, if it makes sense, use an average of surrounding values (ie. average of temperatures 5 days before and after)
  - Use conditional formatting to identify any blank cells that are left

### 6) Standardizing the case for text  
  - Standardize header names
  - You can make a temporary column and use the UPPER, LOWER, or PROPER formula, copying and pasting over the original
    
### 7) Standardizing formats for each data type (dates, numbers, etc.)  
  - Use Format Cells to make all the data in a column the same type (ie. mdy date, currency)
  - You may be able to use the fill handle for any dates that didn't convert (like text)
  - Use Format Cells to make sure all numbers have the same amount of decimal places
    
### 8) Working with outliers 
  - You can delete the outlier (usually not recommended)
  - You can use the median instead of the average
  - You can include the outlier for some purposes and exclude it for others
    
### 9) Visualizing to verify clean data  
  - Select a column and go to recommended charts
  - You don't need to make the chart, just preview
  - Check for consistency
  - Not visualizing, but also check options under filter
