AUTHOR: Lemuel Waye Otoo-Biney

1. The Dangers of Data Redundancy
----------------------------------
Data Integrity is factual or correct data.
if a company stores a customer's physical address into 3
seperate tables this will cause a data redundancy because
the physical address is repeated, more space in the tables
is used and this will also bring misinformation due to the
customer updating thier physical address, the table having
the updated address will not match the other tables.The 
contradicting data can cause problems in processing queries.

-----------------------------------------------------------

2. Primary vs Foreign Key Enforcement
---------------------------------------
A primary Key is a unique ID like a student_id and there can only
be one primary key coloumn in a table.A Foreign Key is a column
in the child table that relates to the primary key of the parent table.
The database checks the link between the primary key and foreign key the
because every time there are queries to add, update, delete data it will
not allow for a row in the child table to be deleted or adding a row 
with non existing foreign key in the child table student.

E.g)A parent table called Student with a columns such as primary 
key=student_id, varchar(100)=full_name with one row (1, Lemmy Otoo)
and a child Table Courses:
with columns having a primary key= course_id, Date=start_date, foriegn
key student_id. Inserting a value in the child table 
course_id, start_date, student_id
(101     ,'2026-07-20', 1) will work because there is a student with there
is a student_id = 1 but if a value is inserted has a foreign key= 100 it or
in a new cousrse_id in the same foreign key=1 it will not work.

