Steps I Performed on the Netflix Dataset using Excel Tool.

1. Load the Dataset

Opened the original dataset (netflix_titles.csv).

Checked total rows (8,807) and columns (12).

2. Remove duplicates

Select the whole table → Go to Data → Remove Duplicates.

Keep show_id as the unique key.


3. Filter for Latest 5 Years

Found the latest release_year in the dataset (2021).

Kept only rows where release_year >= 2017 (last 5 years: 2017–2021).
 


4. Keep Only 500 Rows

Took the first 500 rows from this filtered data (head selection).

Resulting file had exactly 500 records.



5. Handle Missing Values

director → replaced blanks with "Unknown".

cast → replaced blanks with "Unknown".

country → replaced blanks with "Unknown".

date_added → left as blank (or "Not Available" if you want in Excel).

rating → replaced blanks with "Not Rated".

duration → replaced blanks with "Unknown".


6. Standardize Date Format

Converted date_added column into Date format (dd-mm-yyyy).


7. Split “Duration” Column

Created two new columns:

duration_minutes: extracted numeric value where duration contained "min" (e.g., 90 min → 90).

seasons: extracted numeric value where duration contained "Season" (e.g., 2 Seasons → 2).



