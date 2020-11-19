# Database Normalization
//THIS WAS FROM THE WRONG LINK SOMEHOW///////////////////////////////////////////////////////////
- Using operators like `GROUP BY` and `HAVING` makes your query more specific, so you don't need subqueries.
- `PIVOT` operator rotates a table-valued expression. It turns the unique values in one column into multiple columns in the output and performs aggregations on any remaining column values.
- built in **SQL String functions** make it possible for you to find and alter text values, such as VARCHAR and CHAR datatypes, in SQLServer
- there are also built in **logic functions**
- you can **string together** tables in SQL
//////////////////////////////////////////////////////////////////////////////////////////////
- Database Normalization is a process used to organize a database into tables and columns
- Tables should only have one purpose
### Main reasons to normalize
- Minimizes duplicate data
- Avoids data modification issues
- Simplifies queries
### Modification Anomaly
- Insert Anomaly when data **cannot be inserted** unless additional information is gathered
- Update Anomaly when some of a records **data is repeated on other rows**, forcing multiple updates to effect a single change
- Search and Sort Issues: when desirable selection data is potentially present in multiple columns the queries become more complex
### Forms of DB Normalization
#### 1st (1NF)
- Info is stored in a relational table
- Each column contains atomic values
- No repeating groups of columns
#### 2nd (2NF)
- Table already in 1st normal form
- All columns depend on the tables primary key
#### 3rd (3NF)
- Table is already in 2nd normal form 
- Columns are not transitively dependent on the primary key

[<-- Back](301readingnotes.md) [Back to Home](README.md)