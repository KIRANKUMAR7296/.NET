# ADO.NET 

<table>
   <tr>      
      <th align=left><a href='#ado'>ADO</a></th>
      <th align=left><a href='#set'>Data Set vs Data Reader</a></th>   
      <th align=left><a href='#scalar'>ExecuteScalar</a></th>
      <th align=left><a href='#reader'>ExecuteReader</a></th>
      <th align=left><a href='#non'>ExecuteNonQuery</a></th>          
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
`Read Write` Access to Data | `Read Only` Access to Data
`Slow` Access | `Fast` Access
No need of Connection | Need Connection

<h3 name='scalar'>3. ExecuteScalar</h3> 

- Used when Query Returns `Single` Value. ( First Row or First Column from the Database )

<h3 name='reader'>4. ExecuteReader</h3> 

- Used when Query Returns `Multiple` Value ( Set of Rows and Columns )

<h3 name='non'>5. ExecuteNonQuery</h3>

- Used when Query `doesn't` returns Data from Database. 
- Only returns `Integer` specifying Number of Rows Inserted, Updated or Deleted.	
