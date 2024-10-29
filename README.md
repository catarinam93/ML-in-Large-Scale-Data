# ML-in-Large-Scale-Data
Assignment of the course Large Scale Data Science (BSc in Artificial Intelligence and Data Science 3rd year, 2nd semester)

## A little context
### Introduction
The central theme of this project is centered around the analysis and prediction of patient data collected during their stay in the Intensive Care Unit (ICU). The primary dataset, provided in the EVENTS.csv.gz file, contains extensive records of various events related to ICU patients. This compressed file is approximately 4.2 Gigabytes in size. Our objective is to conduct a comprehensive data analysis and apply machine learning techniques to glean insights from this data. Specifically, we aim to carry out statistical analyses and data visualizations for each patient (denoted by SUBJECT_ID), keeping in mind that a single patient can have multiple hospital admissions (denoted by HADM_ID).

Following our professor’s recommendation, we focused on a single disease to streamline our analysis and prediction efforts. We identified the most recurrent disease within the dataset. All tables were stored in Google BigQuery for efficient querying and management.

During the project, we selected and analyzed several key columns that we deemed most relevant for our work. The merging of these columns into a new table resulted in a BigQuery table format, which posed challenges when using other tools like ApacheSpark, Dask, etc., as these tools require a CSV file for processing.

Therefore, we conducted a comprehensive analysis using only BigQuery and BigFrames.pandas. The final table contained over 4 billion rows. By exporting this table through Google Sheets, we were able to convert it into a CSV file, albeit containing only 500 rows out of the original 4 billion. This limited sample allowed us to perform some level of analysis using the desired tools, albeit less accurately. This approach enabled us to apply and practice the knowledge we gained and to produce a more complete project.

### Visualization of the datasets found important
We performed an analysis of several chosen tables, meticulously selecting (on the section "Junction of the columns of the tables found important") the columns that were most relevant to our study. This selection process was crucial for focusing our efforts on the most informative aspects of the data, ensuring that our visualizations would provide meaningful insights.

### Data Pre Processing
After all the relevant data is gathered, preprocessing is performed, including handling null values, outliers, and other processes.

### Prediction Model
The last step was to build a Machine Learning model which could predict the Length of Stay (LOS) of the patients.

### Conclusion
In conclusion, this project provided a comprehensive opportunity to delve into the intricacies of working with large datasets, specifically within the context of ICU patient events. Utilizing a variety of tools and techniques, such as map-reduce, PySpark, BigQuery and Dask we were able to efficiently process and analyze the substantial volume of data contained in the EVENTS.csv.gz file. This hands-on experience underscored the practical utility of big data technologies in managing and extracting meaningful insights from extensive datasets, highlighting their importance in modern data science workflows.

Despite encountering several challenges throughout the process, we successfully performed the required statistical analysis and visualization for each patient, and developed a predictive model for the length of stay. These accomplishments illustrate not only the effectiveness of the tools employed but also our adaptability and problem-solving skills. The knowledge gained from this project is invaluable, as it equips us with the expertise to handle similar big data tasks in the future, ensuring that we can make data-driven decisions with confidence. Overall, the project was a rewarding experience that met all the outlined objectives.

**Note:** All the work was performed in Google Cloud Platform (GCP)
