# Database Normalization 

- **Database normalization**:- is the process of structuring a **relational database** in accordance with a series of so-called **normal forms** in order to reduce **data redundancy** and improve **data integrity**.

- **Normalization**:-  entails organizing the **columns** (attributes) and **tables** (relations) of a database to ensure that their **dependencies** are properly enforced by database integrity constraints. It is accomplished by applying some formal rules either by a process of synthesis (creating a new database design) or decomposition (improving an existing database design).

- **Database normalization** is a process used to organize a database into tables and columns.

- Ex: The main idea with this is that a table should be about a **specific topic** and **only supporting topics** included. 


- By limiting a table to one purpose you **reduce the number of duplicate data contained within your database**. This eliminates some issues stemming from database modifications.

#### What is a Database Table?
A relational database is made up of several components, of which the table is most significant.  The database table is where all the data in a database is stored, and without tables, there would not be much use for relational databases.

- A database consists of one or more tables.  Each table is made up of **rows** and **columns**.

**Columns**: are defined to hold a specific type of data, such as dates, numeric, or textual data.  In the simplest of definitions a column is defined by its name and data type

**Rows**:A table can contain zero or more rows.  When there are zero, it said to be empty.  There is not practical limit on the number of rows a table can hold 

#### Reasons for Database Normalization

There are three main reasons to normalize a database.  The first is to **minimize duplicate data**, the second is to **minimize or avoid data modification issues**, and the third is to **simplify queries**. 

- **Data Duplication and Modification Anomalies**
Duplicated information presents two problems:

1. It increases storage and decrease performance.

2. It becomes more difficult to maintain data changes.

Database normalization fixes them. There are three modification anomalies that can occur:
 
 Normalizing an example table
These steps demonstrate the process of normalizing a fictitious student table.

1. **First normal form**:
- Eliminate repeating groups in individual tables.
- Create a separate table for each set of related data.
- Identify each set of related data with a primary key.

2. **Second normal form**:
- Create separate tables for sets of values that apply to multiple records.
- Relate these tables with a foreign key.

3. **Third normal form**:
- Eliminate fields that do not depend on the key.


1.  Unnormalized table:

TABLE 1
Student#	Advisor	Adv-Room	Class1	Class2	Class3
1022	    Jones	    412	     101-07	  143-01	159-02
4123	    Smith  	  216	      201-01	211-02	214-01

2. **First normal form**: No repeating groups

- Tables should have only two dimensions. Since one student has several classes, these classes should be listed in a separate table. Fields Class1, Class2, and Class3 in the above records are indications of design trouble.

- Spreadsheets often use the third dimension, but tables should not. Another way to look at this problem is with a one-to-many relationship, do not put the one side and the many side in the same table. Instead, create another table in first normal form by eliminating the repeating group (Class#), as shown below:

TABLE 2
Student#	Advisor	Adv-Room	Class#
1022	    Jones	    412	    101-07
1022	    Jones	    412	    143-01
1022	    Jones	    412	    159-02
4123	    Smith	    216	    201-01
4123	    Smith	    216	    211-02
4123	    Smith	    216	    214-01


3. **Second normal form**: Eliminate redundant data

-Note the multiple Class# values for each Student# value in the above table. Class# is not functionally dependent on Student# (primary key), so this relationship is not in second normal form.

The following two tables demonstrate second normal form:

Students:

TABLE 3
Student#	Advisor	Adv-Room
 1022	    Jones	   412
 4123	    Smith	   216

Registration:

TABLE 4
Student#	Class#
 1022	    101-07
 1022	    143-01
 1022	    159-02
 4123	    201-01
 4123	    211-02
 4123	    214-01

4. Third normal form: Eliminate data not dependent on key

In the last example, Adv-Room (the advisor's office number) is functionally dependent on the Advisor attribute. The solution is to move that attribute from the Students table to the Faculty table, as shown below:

Students:

TABLE 5
Student#	Advisor
1022	Jones
4123	Smith

Faculty:

TABLE 6
Name	 Room	 Dept
 Jones	412	 42
 Smith	216	 42


 - **source https://docs.microsoft.com/**