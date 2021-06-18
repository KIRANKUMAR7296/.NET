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

DataSet |  DataReader 
:--- | :---
Has `Read Write` Access to Data | Has `Read Only` Access to Data
`Slow` Access | `Fast` Access
Do not need Connection | Needs `Connection`

<h3 name='execute'>3. ExecuteScalar | ExecuteReader | ExecuteNonQuery</h3>

ExecuteScalar | ExecuteReader | ExecuteNonQuery
:--- | :--- | :---
Is used when Query Returns `Single` Value | Query Returns `Multiple` Value | Query do not returns Data
e.g. First Row or First Column from the Database | Set of Rows and Columns | Only Returns Number of Rows Inserted, Updated or Deleted.
