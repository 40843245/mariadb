# notice when a FK references to a PK
Please be careful about these details when a FK references to a PK. Otherwise, you will get the error for a while.

Take my recent project as example. Last night, there were lots of different errors while I tried to make a FK reference to a PK. 
I had checked it two times. However, I didn't solve the issues at this morning.

When I checked at third time, I accidentally solve all of them. In this event, I have learn a lesson. I think it is

    1. NEVER use the same name in same database among FK constraint name and one of these items:
       other FK constraint name
       field name
       table name 
       database name
       etc
       
       NEVER!!!
       
    2. Before make a link about a FK references to a PK, please check there are duplicate values in primary key (in PK table).
    Because if one tries to make a link about a FK to a PK that has duplicate values, then the property of PK will be violated.
    Thus, one has to delete duplicate row (if exists) before make a link about a FK to a PK.
    
    For more details about PK's property, see my notes at Github.
    
## See Also
PK

https://github.com/40843245/mariadb/blob/main/knowledge%20base/key/PK/PK.md
    
    
    
    
