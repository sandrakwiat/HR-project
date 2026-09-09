# HR-project

STEP 1:
The first step was to connect Power BI to a folder containing the HR data.

The dataset consists of 18 separate files, with a new file added each month. Instead of importing each file individually, I connected Power BI directly to the folder and used Power Query to combine the files into a single dataset.

Why is this important?

Using a folder connection makes the data preparation process more efficient and scalable. When a new monthly file is added to the folder, the dataset can be updated without manually importing and combining additional files.

This approach reflects a more realistic business scenario, where data is continuously collected over time and reports need to be refreshed regularly.

Tools used: Power BI, Power Query

***

STEP 2: Creating Dimension and Fact Tables

The next step was to structure the data into separate dimension and fact tables.

The original Employment table contained both employee-related information and monthly employment records. To create a more organized and efficient data model, I split the data into two tables:

dimEmployees

The dimEmployees table contains unique information about each employee. Each employee appears only once in this table.

This table stores employee attributes that are not expected to change from month to month, such as demographic or personal information.

fctEmployment

The fctEmployment table contains monthly employment records for each employee. Each row represents an employee's employment status at a specific point in time, including information such as their position or other employment-related attributes.

Why is this important?

Separating the data into dimension and fact tables helps create a more structured and scalable data model.

This approach:

Reduces data duplication.
Makes relationships between tables easier to manage.
Improves the performance and clarity of the Power BI data model.
Makes it easier to analyze changes in employees' employment information over time.

This structure also follows a common data modeling approach used in Business Intelligence and analytics projects.

Tools used: Power BI, Power Query
