# ADO.NET 

<table>
   <tr>      
      <th align=left><a href='#ado'>ADO</a></th>
      <th align=left><a href='#set'>Data Set vs Data Reader</a></th>   
      <th align=left><a href='#execute'>ExecuteScalar | ExecuteReader | ExecuteNonQuery</a></th>               
   </tr>
</table>
  

<h3 name='ado'>1. ADO.NET ( ActiveX Data Object )</h3>

- Bridge between Front end `Controls` and backend `Database`.
- Encapsulates all the Data Access Operations, Control Interactions and Display Data.

- `Data Provider` : Connection, Command and DataAdapter ( `Select`, `Insert`, `Delete` and `Update` Command )
- `DataSet` : DataRelationCollection and DataTableCollection ( `DataTable`, Rows, Columns and Constraints )

- `Connection`  : Connect `Data Source` for performing Operations.
- `Command` : `Query` or Stored Procedure to and from Database for `Extracting`, `Transforming` or `Loading` data.
- `DataAdapter` : Helps DataSet to Load Data from Multiple Databases or Data Source.
- `DataReader` : `Read only` Access to Data in Database.
- `DataRelationCollection` : Represents relationship between two `Tables`.

<h3 name='set'>2. DataSet vs DataReader</h3>

- Used to `Get` and `Store` data in a C#.

DataSet |  DataReader 
:--- | :---
Has `Read Write` Access to Data | Used to Retrieve `Read Only` Data from Database
`Slow` Access | `Fast` Access
Do not need Connection | Needs `Connection`

<h3 name='execute'>3. ExecuteScalar | ExecuteReader | ExecuteNonQuery</h3>

ExecuteScalar | ExecuteReader | ExecuteNonQuery
:--- | :--- | :---
Is used when Query returns `Single` Value | Query returns `Multiple` Value | Query returns no Data
e.g. First Row or Column from the Database | Set of Rows and Columns | Only Returns Number of Rows Inserted, Updated or Deleted.
