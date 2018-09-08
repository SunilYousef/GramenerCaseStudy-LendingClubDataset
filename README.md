# GramenerCaseStudy-LendingClubDataset
Using EDA, understand risk analytics in banking and financial services and understand how data is used to minimize the risk of losing money while lending to customers.

# Business Objectives
This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

Independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

# Tasks
research a little about risk analytics (understanding the types of variables and their significance should be enough).
## Perform
Data sourcing
Data cleaning
Fix rows and columns
Checklist for Fixing Rows
Delete summary rows: Total, Subtotal rows
Delete incorrect rows: Header rows, Footer rows
Delete extra rows: Column number, indicators, Blank rows, Page No.
Checklist for Fixing Columns
Merge columns for creating unique identifiers if needed: E.g. Merge State, City into Full address
Split columns for more data: Split address to get State and City to analyse each separately
Add column names: Add column names if missing
Rename columns consistently: Abbreviations, encoded columns
Delete columns: Delete unnecessary columns
Align misaligned columns: Dataset may have shifted columns
Save this checklist for future reference: https://cdn.upgrad.com/UpGrad/temp/9fd01a02-b165-48d3-b1f9-499158476b96/Data+Cleaning+_+Checklist.xlsx
Fix missing values
good methods add information
bad methods exaggerate information
In case you can add information from reliable external sources, you should use it to replace missing values. But often, it is better to let missing values be and continue with the analysis rather than extrapolate the available information.
Set values as missing values: Identify values that indicate missing data, and yet are not recognised by the software as such, e.g treat blank strings, "NA", "XX", "999", etc. as missing.
Adding is good, exaggerating is bad: You should try to get information from reliable external sources as much as possible, but if you can’t, then it is better to keep missing values as such rather than exaggerating the existing rows/columns.
Delete rows, columns: Rows could be deleted if the number of missing values are insignificant in number, as this would not impact the analysis. Columns could be removed if the missing values are quite significant in number.
Fill partial missing values using business judgement: Missing time zone, century, etc. These values are easily identifiable.
Working With Missing Values https://pandas.pydata.org/pandas-docs/stable/missing_data.html
Standardise values
Standardise units: Ensure all observations under a variable have a common and consistent unit, e.g. convert lbs to kgs, miles/hr to km/hr, etc.
Scale values if required: Make sure the observations under a variable have a common scale
Standardise precision for better presentation of data, e.g. 4.5312341 kgs to 4.53 kgs.
Remove outliers: Remove high and low values that would disproportionately affect the results of your analysis.
Remove extra characters like such as common prefix/suffix, leading/trailing/multiple spaces, etc. These are irrelevant to analysis.
Standardise case: There are various cases that string variables may take, e.g. UPPERCASE, lowercase, Title Case, Sentence case, etc.
Standardise format: E.g. 23/10/16 to 2016/10/20, “Modi, Narendra" to “Narendra Modi", etc.
Fix invalid values
Encode unicode properly: In case the data is being read as junk characters, try to change encoding, E.g. CP1252 instead of UTF-8.
Convert incorrect data types: Correct the incorrect data types to the correct data types for ease of analysis. E.g. if numeric values are stored as strings, it would not be possible to calculate metrics such as mean, median, etc. Some of the common data type corrections are — string to number: "12,300" to “12300”; string to date: "2013-Aug" to “2013/08”; number to string: “PIN Code 110001” to "110001"; etc.
Correct values that go beyond range: If some of the values are beyond logical range, e.g. temperature less than -273° C (0° K), you would need to correct them as required. A close look would help you check if there is scope for correction, or if the value needs to be removed.
Correct values not in the list: Remove values that don’t belong to a list. E.g. In a data set containing blood groups of individuals, strings “E” or “F” are invalid values and can be removed.
Correct wrong structure: Values that don’t follow a defined structure can be removed. E.g. In a data set containing pin codes of Indian cities, a pin code of 12 digits would be an invalid value and needs to be removed. Similarly, a phone number of 12 digits would be an invalid value.
Validate internal rules: If there are internal rules such as a date of a product’s delivery must definitely be after the date of the order, they should be correct and consistent.
Filter data
Deduplicate data: Remove identical rows, remove rows where some columns are identical
Filter rows: Filter by segment, filter by date period to get only the rows relevant to the analysis
Filter columns: Pick columns relevant to the analysis
Aggregate data: Group by required keys, aggregate the rest
Univariate analysis - i.e. analysis of a single variable
Create metadata by classifying data in catagorical (ordered, unordered) and Quantitative varaibles
Create segments
Understand each catagorical data and there characteristics
Bivariate analysis
Analyse multuple varaibles by plotting there Correlation ans co-efficient
Derived metrics
Results of following analysis in business terms,
univariate
bivariate
Include visualisations
Summarise the most important results in the presentation
