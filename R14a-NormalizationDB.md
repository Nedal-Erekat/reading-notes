# Database normalization
#### Database normalization is a process used to organize a database into tables and columns.
#### By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

## Reasons for Database Normalization
There are three main reasons to normalize a database.  
1. The first is to minimize duplicate data, 
2. the second is to minimize or avoid data modification issues, and 
3. the third is to simplify queries. 

##  In general I like to see tables that have one purpose.  Having the table serve many purposes introduces many of the challenges;
> namely, data duplication, data update issues, and increased effort to query data.

#### Duplicated information presents two problems:

1. It increases storage and decrease performance.
2. It becomes more difficult to maintain data changes.

### there are two main issue
1. Search and Sort Issues
2. Insert and Deletion Anomaly


- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key

