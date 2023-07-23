# Glassdoor Data Cleaning and Transformation

This project revolves around a dataset acquired from Kaggle, which contains uncleaned data of job postings for data science positions on Glassdoor. The primary objective of this project is to clean and transform the dataset to facilitate further analysis and visualizations. <br>
**Github Repository:** https://github.com/Prakb2401/Glassdoor-Data-Cleaning-and-Transformation <br>
**Kaggle:** https://www.kaggle.com/datasets/rashikrahmanpritom/data-science-job-posting-on-glassdoor

## Collaborators
- Prakhyath Bagavatula: [Prakb2401](https://github.com/Prakb2401) 
- Ramnath Gowrishankar: [raamnath025](https://github.com/raamnath025)
## Project Overview

The dataset initially presented several challenges that required addressing to make the data more usable and insightful. We approached these challenges by asking the following guiding questions:

1. Can we convert the salary column into integers for easier analysis?
2. How can we remove the numbers from the company name to make the data cleaner?
3. What additional information can we extract from the job descriptions to provide more context and insights?
4. How can we create new features from this dataset to enhance its value?

By addressing these questions, we were able to transform the raw dataset into a more structured and insightful format.

## Technologies Used
- Python
- Pandas
- Numpy
- Jupyter
- NLTK
## Project Structure

The final version of this project includes a Jupyter notebook that contains the Python script used to clean and transform the data. The notebook provides a step-by-step walkthrough of the process, detailing how we addressed each of the guiding questions and the methodologies used.

## Conclusions

After a thorough cleaning and transformation process, we were able to answer our guiding questions and gain valuable insights from the dataset:

1. **Can we convert the salary column into integers for easier analysis?**<br> 
    Yes, we were able to process the 'Salary Estimate' column to extract the minimum and maximum salary values, and calculate an average salary. This was achieved by handling two different formats for the 'Salary Estimate' string using the .split and .replace functions.

2. **How can we remove the numbers from the company name to make the data cleaner?**<br>
   We successfully removed numbers from the 'Company Name' column by applying a lambda function to each value. This function splits each company name string into parts at each newline character (`\n`), and returns the first part. The results were then applied back to the 'Company Name' column in the DataFrame, effectively replacing the original company names with the cleaned versions without the numbers. This process was designed to remove any ratings included at the end of the company names.

3. **What additional information can we extract from the job descriptions to provide more context and insights?**<br>
   We were able to extract valuable information regarding skills from the 'Job Description' column. By identifying the presence of certain keywords like "python", "sql", etc., we created new columns based on these keywords, providing a clear view of the skills required or recommended in the job descriptions.

4. **How can we create new features from this dataset to enhance its value?**<br>
   We created two new features: 'Average Rating' and 'Average Salary Per State'. The 'Average Rating' feature was created by writing a code that looped through our data, finding the average rating of companies headquartered in each state. This allowed us to compare and see which states have higher rated companies. Similarly, the 'Average Salary Per State' feature was created by using the average salaries that were already calculated to find which states on average have higher salaries for their Data Science employees.

Through this project, we have transformed an uncleaned dataset into a structured and insightful resource, ready for further analysis and visualization. The methodologies and results of this project demonstrate the power and necessity of data cleaning and transformation in data science.

## Future Work

This project serves as a foundation for further analysis and visualizations. With the cleaned and transformed dataset, we can now delve deeper into the data to uncover trends, patterns, and insights related to data science job postings on Glassdoor. 

## Contributions

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/your-repo/issues) if you want to contribute.

## License

This project is [MIT](https://choosealicense.com/licenses/mit/) licensed.
