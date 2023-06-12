# EXP 06 - CREATE A SQL PROGRAM USING SET OPERATION
[ UNION , UNION ALL ,INTERSECT , EXCEPT ]

## AIM:

To create a sql program using set operation 

## ALGORITHM:

1) Create tables A and B with attributes ID and name
2) Insert values into the tables
3) Display the tables
4) Perform set operations
5) Union - Combines the distinct rows from both tables A and B
6) Union All - Combines all rows from both tables A and B, including duplicates
7) Intersect - Retrieves the common rows between tables A and B
8) Except - Retrieves the rows from table A that are not present in table B

## PROGRAM:
```java
CREATE TABLE A (
    ID INT,
    name VARCHAR(50)
);

CREATE TABLE B (
    ID INT,
    name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Jane');
INSERT INTO A (ID, name) VALUES (3, 'Alice');

INSERT INTO B (ID, name) VALUES (2, 'Jane');
INSERT INTO B (ID, name) VALUES (3, 'Alice');
INSERT INTO B (ID, name) VALUES (4, 'Mike');
SELECT * FROM A;
SELECT * FROM B;
SELECT * FROM A
UNION
SELECT * FROM B;
SELECT * FROM A
UNION ALL
SELECT * FROM B;
SELECT * FROM A
INTERSECT
SELECT * FROM B;
SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:

### TABLE A:

<img width="348" alt="dbms e6 1" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/7b22b552-69a9-4776-b356-093ee2071146">

### TABLE B:

<img width="356" alt="dbms e6 2" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/a1038978-15a0-45fd-b8eb-5804549c83ab">

### UNION:

<img width="364" alt="dbms e6 3" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/57891fca-ce83-474c-85c5-40a6ac77e086">

### UNION ALL:

<img width="366" alt="dbms e6 4" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/78cea972-e7a7-4d21-a6b2-9f8fb2b7ebc8">

### INTERSECT:

<img width="363" alt="dbms e6 5" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/9bb6aa61-06d9-4399-8809-bbce62fcb84e">

### EXCEPT:

<img width="390" alt="dbms e6 6" src="https://github.com/divvisha/SET-OPERATION/assets/127508123/55a4ca52-8383-4786-91fd-862d1b5045c0">

## RESULT:

Thus we have successfully obtained the required result using the above-given code.
