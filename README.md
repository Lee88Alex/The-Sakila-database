# The-Sakila-database
The Sakila database used in this lab comes from the following source: https://dev.mysql.com/doc/sakila/en/ under New BSD license [Copyright 2021 - Oracle Corporation].
https://opensource.org/licenses/bsd-license.php?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDB0110ENSkillsNetwork883-2022-01-01

https://www.edx.org/course/getting-started-with-mysql

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/sakila/sakila_ERD.jpg
MySQL command line (CLI) to:

Create a database.
create database sakila;
use sakila;

Restore the structure and data of a table.
source sakila_mysql_dump.sql;
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.1.png

Explore and query tables.
DESCRIBE staff;
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.2.png

SHOW FULL TABLES WHERE table_type = 'BASE TABLE';
SELECT * FROM staff;
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.3.png

Dump/backup tables from a database.
mysqldump --host=127.0.0.1 --port=3306 --user=root --password sakila staff > sakila_staff_mysql_dump.sql
To view the contents of the dump file within the terminal, use the command below:
cat sakila_staff_mysql_dump.sql
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/D.3.png
