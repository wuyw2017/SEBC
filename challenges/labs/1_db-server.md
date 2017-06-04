1. hostname of your database server:
```
 [root@ip-172-31-37-46 etc]# hostname
ip-172-31-37-46
```
2. The command and output for showing the database server version
```
[root@ip-172-31-37-46 etc]# mysql -V
mysql  Ver 14.14 Distrib 5.7.18, for Linux (x86_64) using  EditLine wrapper
```
3. The command and output for listing the databases created above
```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
| sys                |
+--------------------+
10 rows in set (0.00 sec)

mysql> 
```
