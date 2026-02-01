🧰 Tech Stack

   Python

   Pandas (data cleaning & validation)

   PySpark (scalable ETL concepts)

   MySQL (Raw + DWH storage)

   SQL

 


📂 Data Source

   Input data comes from a CSV file

   Batch processing (no streaming)




🗄️ Data Layers
   1️⃣ Raw Layer

      Raw CSV data is ingested into the database without heavy transformations

   Purpose:

      Preserve original data

     Allow reprocessing if ETL fails

     Act as a learning replacement for a Data Lake


  2️⃣ ETL Processing Layer
  
    ETL is performed using Pandas and PySpark:

    Data cleaning

    Data type corrections

    Column renaming

    Null handling

    Basic validation



  3️⃣ Data Quality Checks

    The ETL process focuses on the following Data Quality dimensions:

    Completeness

    Consistency

    Validity

    Accuracy
  
    Uniqueness

    Timeliness

    Checks are applied at a basic level suitable for learning.



🧱 Data Warehouse Design(OLAP)
⭐ Star Schema

    The Data Warehouse is modeled using a Star Schema(1 fact table and 2 dimention table).

    Fact Table
      fact_Emp
      Monthly_salary (Fact)
      st_id (FK)
      date_id (FK)

    Dimension Tables

       dim_Emp
       Status
       Education
       Industry
       Location
       AI_Risk
       Age_Group
       Exp_years


    dim_date
      Date_Recorded

    ✔️ Surrogate Keys are used
    ✔️ Fact contains only metrics + FKs
    ✔️ Dimensions store descriptive attributes








   
