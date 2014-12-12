##
##dm64.exe -h ALL 

---------------------------------------------------------------------- 
#FreeUkraine #SaveUkraine #StopRussia #PutinKhuilo #CrimeaIsUkraine
----------------------------------------------------------------------
Oracle to MySQL DataMigrator (v1.23.9, beta, 2014/12/12 13:50:17) [64bit]
Copyright (c): 2014 Alex Buzunov, All rigts reserved.
Agreement: Use this tool at your own risk. Author is not liable for any damages or losses related to the use of this software.
----------------------------------------------------------------------
From Oracle:

Set following command line arguments to copy from Oracle to MySQL:

-w copy_vector -o pool_size -r num_of_shards -t field_term -l lame_duck -K keep_data_file -1 arg_1 -2 arg_2 -3 arg_3 -q query_sql_file -Q query_sql_dir -c from_table -P from_partition -S from_sub_partition -f from_db -e nls_date_format -m nls_timestamp_format -O nls_timestamp_tz_format -z source_client_home -u to_user -p to_passwd -d to_db_name -s to_db_server -a to_table -Z target_client_home 

Here:
(Common) -w [--copy_vector]	Data copy direction.	
(Common) -o [--pool_size]	Pool size.	
(Common) -r [--num_of_shards]	Number of shards.	
(Common) -t [--field_term]	Field terminator.	
(Common) -l [--lame_duck]	Limit rows (lame duck run).	
(Common) -K [--keep_data_file]	Keep data dump.	
(Common) -1 [--arg_1]	Generic string argument 1.	
(Common) -2 [--arg_2]	Generic string argument 2.	
(Common) -3 [--arg_3]	Generic string argument 3.	
(From Oracle) -q [--query_sql_file]	Input file with Oracle query sql.	
(From Oracle) -Q [--query_sql_dir]	Input dir with Oracle query files sql.	
(From Oracle) -c [--from_table]	From table.	
(From Oracle) -P [--from_partition]	From partition.	
(From Oracle) -S [--from_sub_partition]	From sub-partition.	
(From Oracle) -f [--from_db]	From database.	
(From Oracle) -e [--nls_date_format]	nls_date_format for source.	
(From Oracle) -m [--nls_timestamp_format]	nls_timestamp_format for source.	
(From Oracle) -O [--nls_timestamp_tz_format]	nls_timestamp_tz_format for source.	
(From Oracle) -z [--source_client_home]	Path to Oracle client home.	
(To MySQL) -u [--to_user]	Target MySQL db user.	
(To MySQL) -p [--to_passwd]	Target db user password.	
(To MySQL) -d [--to_db_name]	Target database.	
(To MySQL) -s [--to_db_server]	Target db instance name.	
(To MySQL) -a [--to_table]	Target table.	
(To MySQL) -Z [--target_client_home]	Path to mysql client home.	

--USE CASES--

1. Oracle_to_MySQL. 18 use cases.


Oracle_to_MySQL: 18 use case(s) available:

1. ORA_DateTable_to_MYSQL - Copy Oracle table1 into MySQL  table.
2. ORA_Partition_KeepSpoolFile_to_MYSQL - Copy Oracle partition into MySQL  table.
3. ORA_Partition_Limit10_to_MYSQL - Copy only 10 rows from Oracle partition into MySQL  table.
4. ORA_Partition_to_MYSQL - Copy Oracle partition into MySQL  table.
5. ORA_QueryDir_Limit10_to_MYSQL - Read each SQL query file from a directory "c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora".
	  Copy only 10 rows from Oracle query results into MySQL  table.
6. ORA_QueryDir_to_MYSQL - Read each SQL query file from a directory "c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora".
	  Copy Oracle query results into MySQL  table.
7. ORA_QueryFile_Limit10_to_MYSQL - Read SQL from a query file "c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql".
	  Copy only 10 rows from Oracle query results into MySQL  table.
8. ORA_QueryFile_to_MYSQL - Read SQL from a query file "c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql".
	  Copy Oracle query results into MySQL  table.
9. ORA_ShardedPartition_to_MYSQL - Break input sharded partition into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle sharded partition into MySQL  table.
10. ORA_ShardedSubpartition_to_MYSQL - Break input sharded sub-partition into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle sharded sub-partition into MySQL  table.
11. ORA_ShardedTable_to_MYSQL - Break input table1 into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle table1 into MySQL  table.
12. ORA_Subpartition_KeepSpoolFile_to_MYSQL - Copy Oracle sub-partition into MySQL  table.
13. ORA_Subpartition_Limit10_to_MYSQL - Copy only 10 rows from Oracle sub-partition into MySQL  table.
14. ORA_Subpartition_to_MYSQL - Copy Oracle sub-partition into MySQL  table.
15. ORA_Table_KeepSpoolFile_to_MYSQL - Copy Oracle table1 into MySQL  table.
16. ORA_Table_Limit10_to_MYSQL - Copy only 10 rows from Oracle table1 into MySQL  table.
17. ORA_TimestampTable_to_MYSQL - Copy Oracle table1 into MySQL  table.
18. ORA_TimezoneTable_to_MYSQL - Copy Oracle table1 into MySQL  table.

--DETAILS--

-USE-CASE # 1
Use case name: ORA_DateTable->MYSQL
	Description:  Copy Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -c SCOTT.Date_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Date_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 2
Use case name: ORA_Partition_KeepSpoolFile->MYSQL
	Description:  Copy Oracle partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -K[--keep_data_file] is "Keep data dump."
  -c[--from_table] is "From table."
  -P[--from_partition] is "From partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -K 1 ^
  -c SCOTT.Partitioned_test_from ^
  -P part_15 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 3
Use case name: ORA_Partition_Limit10->MYSQL
	Description:  Copy only 10 rows from Oracle partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -l[--lame_duck] is "Limit rows (lame duck run)."
  -c[--from_table] is "From table."
  -P[--from_partition] is "From partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -l 10 ^
  -c SCOTT.Partitioned_test_from ^
  -P part_15 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 4
Use case name: ORA_Partition->MYSQL
	Description:  Copy Oracle partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -P[--from_partition] is "From partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -c SCOTT.Partitioned_test_from ^
  -P part_15 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 5
Use case name: ORA_QueryDir_Limit10->MYSQL
	Description:  Read each SQL query file from a directory "c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora".
	  Copy only 10 rows from Oracle query results into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -l[--lame_duck] is "Limit rows (lame duck run)."
  -Q[--query_sql_dir] is "Input dir with Oracle query files sql."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -l 10 ^
  -Q c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 6
Use case name: ORA_QueryDir->MYSQL
	Description:  Read each SQL query file from a directory "c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora".
	  Copy Oracle query results into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -Q[--query_sql_dir] is "Input dir with Oracle query files sql."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -Q c:\Python27\data_migrator_1239\test\v101\query\query_dir_ora ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 7
Use case name: ORA_QueryFile_Limit10->MYSQL
	Description:  Read SQL from a query file "c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql".
	  Copy only 10 rows from Oracle query results into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -l[--lame_duck] is "Limit rows (lame duck run)."
  -q[--query_sql_file] is "Input file with Oracle query sql."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -l 10 ^
  -q c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 8
Use case name: ORA_QueryFile->MYSQL
	Description:  Read SQL from a query file "c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql".
	  Copy Oracle query results into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -q[--query_sql_file] is "Input file with Oracle query sql."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -q c:\Python27\data_migrator_1239\test\v101\query\oracle_query.sql ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 9
Use case name: ORA_ShardedPartition->MYSQL
	Description:  Break input sharded partition into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle sharded partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -P[--from_partition] is "From partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 3 ^
  -r 3 ^
  -t "|" ^
  -c SCOTT.Partitioned_test_from ^
  -P part_15 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 10
Use case name: ORA_ShardedSubpartition->MYSQL
	Description:  Break input sharded sub-partition into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle sharded sub-partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -S[--from_sub_partition] is "From sub-partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 3 ^
  -r 3 ^
  -t "|" ^
  -c SCOTT.Sub_Partitioned_test_from ^
  -S part_15_sp1 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 11
Use case name: ORA_ShardedTable->MYSQL
	Description:  Break input table1 into 3 logical shards (-r[--num_of_shards] 3) 
	  and run copy process on each shard in thread pool (-o[--pool_size] 3).
	  Copy Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 3 ^
  -r 3 ^
  -t "|" ^
  -c SCOTT.Timestamp_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 12
Use case name: ORA_Subpartition_KeepSpoolFile->MYSQL
	Description:  Copy Oracle sub-partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -K[--keep_data_file] is "Keep data dump."
  -c[--from_table] is "From table."
  -S[--from_sub_partition] is "From sub-partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -K 1 ^
  -c SCOTT.Sub_Partitioned_test_from ^
  -S part_15_sp1 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 13
Use case name: ORA_Subpartition_Limit10->MYSQL
	Description:  Copy only 10 rows from Oracle sub-partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -l[--lame_duck] is "Limit rows (lame duck run)."
  -c[--from_table] is "From table."
  -S[--from_sub_partition] is "From sub-partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -l 10 ^
  -c SCOTT.Sub_Partitioned_test_from ^
  -S part_15_sp1 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 14
Use case name: ORA_Subpartition->MYSQL
	Description:  Copy Oracle sub-partition into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -S[--from_sub_partition] is "From sub-partition."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -c SCOTT.Sub_Partitioned_test_from ^
  -S part_15_sp1 ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 15
Use case name: ORA_Table_KeepSpoolFile->MYSQL
	Description:  Copy Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -K[--keep_data_file] is "Keep data dump."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -K 1 ^
  -c SCOTT.Timestamp_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 16
Use case name: ORA_Table_Limit10->MYSQL
	Description:  Copy only 10 rows from Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -l[--lame_duck] is "Limit rows (lame duck run)."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -l 10 ^
  -c SCOTT.Timestamp_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 17
Use case name: ORA_TimestampTable->MYSQL
	Description:  Copy Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -c SCOTT.Timestamp_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timestamp_test_to ^
  -Z "C:\Temp\mysql\bin"

-USE-CASE # 18
Use case name: ORA_TimezoneTable->MYSQL
	Description:  Copy Oracle table1 into MySQL  table.
	Arguments:
	  -w[--copy_vector] is "Data copy direction."
  -o[--pool_size] is "Pool size."
  -r[--num_of_shards] is "Number of shards."
  -t[--field_term] is "Field terminator."
  -c[--from_table] is "From table."
  -f[--from_db] is "From database."
  -e[--nls_date_format] is "nls_date_format for source."
  -m[--nls_timestamp_format] is "nls_timestamp_format for source."
  -O[--nls_timestamp_tz_format] is "nls_timestamp_tz_format for source."
  -z[--source_client_home] is "Path to Oracle client home."
  -u[--to_user] is "Target MySQL db user."
  -p[--to_passwd] is "Target db user password."
  -d[--to_db_name] is "Target database."
  -s[--to_db_server] is "Target db instance name."
  -a[--to_table] is "Target table."
  -Z[--target_client_home] is "Path to mysql client home."	
	Example: 
	  echo y|c:\Python27\dm_dist_64\20141212_135017\dm64\dm64.exe ^
  -w ora2mysql ^
  -o 1 ^
  -r 1 ^
  -t "|" ^
  -c SCOTT.Timezone_test_from ^
  -f SCOTT/tiger2@orcl ^
  -e "YYYY-MM-DD HH24.MI.SS" ^
  -m "YYYY-MM-DD HH24.MI.SS.FF2" ^
  -O "YYYY-MM-DD HH:MI:SS.FF2 TZH:TZM" ^
  -z "C:\app\alex_buz\product\11.2.0\dbhome_2\BIN" ^
  -u alex ^
  -p mysql_pwd ^
  -d test ^
  -s localhost ^
  -a Timezone_test_to ^
  -Z "C:\Temp\mysql\bin"