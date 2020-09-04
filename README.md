# mysql cheatsheet

## connect to mysql from bash terminal
`mysql -u $db_user -p`

## database management

### show databases
`show databases;`

### create database
`create database $databasename`

### drop database
`drop database $databasename;`

## user management

### get all privileges (and users)
`select * from information_schema.user_privileges;`

### drop user
`drop user '$username'@'$hostname';`

### create user
`create user '$username'@'$hostname' identified by '$password';`

## grant management

### show grants
`show grants for '$username'@'$hostname';`

### grant all permissions
```
grant usage on $database.* to '$username'@'$hostname';
grant all privileges on $database.* to '$username'@'$hostname';
```

### grant some permissions
```
grant usage on $database.* to '$username'@'$hostname';
grant $permissions on $database.* to '$username'@'$hostname';
```
*$permissions is select, update, delete, etc.*

