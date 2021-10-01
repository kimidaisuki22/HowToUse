## install 
sudo apt install mariadb-server

## config
vim /etc/mysql/my.cnf

 ### change root password
 sudo mysqladmin -u root -p flush-privileges password

## bind listen address
edit /etc/mysql/mariadb.conf.d/50-server.cnf
change  "bind-address = 127.0.0.1" --> "bind-address = :: "
 then exec "sudo service mysql restart"
 
 ## comand line option
 -p | need password
 -u user | login user
 -e "cm" | execute comand
 
 ## example
 
### set password
SET PASSWORD FOR '${userName}'@'${host}' PASSWORD('${newPassWord}'); 

### delete User
DROP USER '${userName}'@'${host}'

### Create user
first Create need IDENTIFIED BY

GRANT ${PRVILEGE} ON ${database}.${table} 
TO '${userName}'@'${host}'
IDENTIFIED BY '${PASSWORD}';

 ${PRVILEGE} : ALL, SELECT
 ${database},${table}: * for any database or table
 
 ### get user grants
 SHOW GRANTS FOR '${userName}'@'${host}' ;
 
 ### find all user (need root)
 SELECT User,Host FROM mysql.user;
 
 
 
