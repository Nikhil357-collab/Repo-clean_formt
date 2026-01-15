# Repo-clean_formt
cleaning and format the data power query.excel


## Project Overview
This project demonstrates a **professional data cleaning and preparation workflow** using a real-world Kaggle dataset (Netflix Movies & TV Shows).  
The objective is to maintain **clear separation between raw and processed data**, apply structured cleaning rules, and document **data quality observations** like a real data analyst.

---

## 📂 Dataset
- Source: Kaggle – Netflix Movies and TV Shows Dataset
- Format: CSV
- Records: Movies and TV Shows metadata (title, director, cast, rating, release year, etc.)

---

##  Tools & Technologies Used

### File Formats
- **CSV** – raw and final export
- **Excel (.xlsx)** – analyst-friendly cleaned output

### Spreadsheet & Analysis Concepts
- Data Cleaning Pipelines
- Raw vs Processed Data Separation
- Data Quality Annotation
- Duplicate Detection
- Missing Value Analysis
- Format Validation

---

## 🧹 Data Cleaning Steps Performed

1.   Raw Data Preservation
   - Original dataset saved as `Raw_Data.xlsx`
   - No transformations applied

2.   Missing Value Identification
   - Detected blanks in columns such as:
     - `director`
     - `rating`
     - `date_added`
   - Context-aware handling (not blindly removed)

3.   Duplicate Detection
   - Removed duplicates based on:
     - `show_id`
     - `title`
   - Raw backup retained to avoid irreversible loss

4. Text Standardization
   - Removed extra spaces (`TRIM`)
   - Standardized casing (`PROPER`)
   - Cleaned inconsistent naming patterns

5. Format Validation
   - Dates validated and converted to proper datetime format
   - Categorical values checked for inconsistencies

6.  Cleaned Data Isolation
   - Final processed data stored separately in `Cleaned_Data`
   - Ensures professional pipeline separation

7.  Data Quality Notes
   - Added a `Data_Quality_Notes` column
   - Examples:
     - 'Missing director names present'
     - “Rating values inconsistent or missing”
     - “Invalid or missing date format”
     -  'blank cell appears but not remove because of chances of loss of other necessary data from there column'

