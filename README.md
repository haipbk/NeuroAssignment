<!-- <table align="center"><tr><td align="center" width="9999"> <b> Reusable Hive Scripts </b></td></tr></table> -->
<table align="center"><tr><td> <font size="40"> Reusable Hive Scripts </font></td></tr></table>

## Export Sample Data of Hive Tables:


This script will generate sample 100 records along with column headers of each table mentioned in file “Export_Hive_TablesList.txt” (should be in the same folder as script). Generates separate file for each table for easy use of exported data.
 

### Command to Execute:
./Export_Hive_Data.sh DB_Name

### Note:
*	Make sure you have access to the Hive Database you are connecting from the Server   
*	You should have execute privilege on Export_Hive_Data.sh, else run the below command to get (read,write,execute privilege on the file)
$chmod u+rwx  Export_Hive_Data.sh


## Create Hive DDL Scripts:


This script will help users to generate DDL Scripts of Hive Tables of a particular database, this will be useful when we want to generate scripts for existing tables, especially when we want to promote scripts from one environment to another.
Tables for which DDL need to be created should be in the same folder as Shell Script with name “Hive_TablesList.txt”, below is the sample
 
 
### Command to Execute:
./ Hive_Create_DDL.sh DB_Name

### Note:
* Make sure you have access to the Hive Database you are connecting from the Server   
* You should have execute privilege on Hive_Create_DDL.sh, else run the below command to get (read,write,execute privilege on the file)
$chmod u+rwx  Hive_Create_DDL.sh

