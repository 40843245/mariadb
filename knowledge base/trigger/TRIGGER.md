# TRIGGER
## CREATE TRIGGER
### LIST TRIGGERS
#### Way 1 (SHOW clause)

    SHOW TRIGGERS;

#### Way 2 (SELECT ... FROM clause)

From Mariadb 5.0.10, one can directly access data from table "trigger" in database "INFORMATION_SCHEMA". One can reach the goal through the SELECT ... FROM clause.

Looks as follows.

    select trigger_schema, trigger_name, action_statement
    from information_schema.triggers
  
###### NOTICE 
It is only support on Mariadb 5.0.10 or above.

#### Ref
From stackoverflow,

https://stackoverflow.com/questions/47363/show-all-triggers-in-a-mysql-database
