# Family Reconstitution Checks   
George Alter

The Access database "Fam_Recon_checks_ver_5.accdb" runs SQL queries that check for inconsistencies in family reconstitution data.  For example, dates of birth of mothers and children are compared to find women that would have been too young or too old when the child was born.  Most of these checks will also work on data from population registers.   
  
Steps:
1. Use the MS-Access Linked Table Manager (under the External Data tab) to link the IDS files (CONTEXT, CONTEXT_CONTEXT, INDIV_CONTEXT, INDIV_INDIV, INDIVIDUAL) to the data in a separate MS-Access database. Check the "Always prompt for new location" to change to a different database.  Test data have been provided in the Fam_Recon_test_data_v2.accdb file.     
        
2. Run the "Run report" macro.  Executing the macro called "Run report" will run all of the queries and create a report with the results.    
   
3. Select "Print Preview" under the "Views" option on the "Home" tab.  Click "Print" to print the report.   
         
Notes:      
The Linked Table Manager can be used to link to data in other IDS databases in Access or other database systems.   Databases other than Access (MySQL, Posgres, Oracle, etc.) can be linked via ODBC.   
   
The queries given here may require editing before they can be used in other database systems.  While basic SQL keywords are the same in all versions of SQL, functions are often implemented differently.  These queries make extensive use of functions for dates and for parsing text, which may not be compatible with other dialects of SQL.   
   
These queries can be tested using the [Fam_Recon_test_data_v2.accdb](https://github.com/altergc/IDS/blob/main/Tools/Family_Reconstitution_Checks/Fam_Recon_test_data_v2.accdb), which is provided in this repository.  This test should generate the result found in the [Fam_recon_report_Test_Data.pdf](https://github.com/altergc/IDS/blob/main/Tools/Family_Reconstitution_Checks/Fam_recon_report_Test_Data.pdf) file.   
   
   
## License    
This work is licensed under the [MIT License](https://opensource.org/licenses/MIT).    
Please see the LICENSE.txt file in this folder.    
    
## Citation	 
Please cite this work as:    
Alter, G. C. (2022). Famly Reconstitution Checks [SQL]. https://github.com/altergc/IDS/tree/main/Tools/Family_Reconstitution_Checks
