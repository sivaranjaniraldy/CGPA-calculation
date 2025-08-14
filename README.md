**Project Title: CGPA Calculation**

**Introduction**

This project is a Google Colab notebook designed to calculate the CGPA (Cumulative Grade Point Average) for senior students. It processes student data from a CSV file, calculates grade points based on letter grades, and is intended to be a straightforward tool for computing a student's academic standing.

**Features**

* **Data Processing:** Reads student data, including grades for multiple subjects, from a CSV file.
* **Grade Point Conversion:** Converts a set of predefined letter grades (O, A+, A, B+, B, C, P, F) into corresponding grade points.
* **CGPA Calculation:** Utilizes the converted grade points to calculate the CGPA.
* **Interactive Environment:** The project is set up within a Google Colab notebook, making it easy to run and share. It also includes code for file uploads directly within the notebook interface.

### **Requirements**

* **Google Colab:** The notebook is designed to run on the Google Colab platform.
* **Python Libraries:** The project utilizes the `pandas` library for data manipulation. It's pre-installed in Colab, so no additional installation is needed.
* **Input Data:** The project requires a CSV file named `mark 01.csv` containing student data. This file must include the following columns: `Register_no`, `Name`, and nine subject grade columns (`Grade1` through `Grade9`). Other columns may also be present but are not used in the CGPA calculation itself.

### **How to Use**

1.  **Open the Notebook:** Open the `SENIOR_CGPA_CALCULATION.ipynb` file in Google Colab.
2.  **Upload Data:** In the notebook, a file upload widget is provided. Click to upload your `mark 01.csv` file.
3.  **Run the Code:** Execute the cells in the notebook sequentially.
    * The first cell will handle the file upload and read the CSV into a pandas DataFrame.
    * Subsequent cells will display the data and perform the grade point conversions and CGPA calculations.
4.  **Review Results:** The output will display the initial DataFrame and the results of the CGPA calculation.

### **Methodology**

The CGPA is calculated based on the following grade point system:

| Grade | Grade Point |
| :---- | :---------- |
| O     | 10          |
| A+    | 9           |
| A     | 8           |
| B+    | 7           |
| B     | 6           |
| C     | 5           |
| P     | 4           |
| F     | 0           |

The notebook iterates through the grades of each student for the nine subjects and uses this grading scale to compute a final CGPA.
