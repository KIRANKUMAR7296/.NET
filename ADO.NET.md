# ADO.NET 

<table>
   <tr>      
      <th align=left><a href='#ado'>ADO</a></th>
      <th align=left><a href='#set'>Data Set vs Data Reader</a></th>   
      <th align=left><a href='#execute'>ExecuteScalar | ExecuteReader | ExecuteNonQuery</a></th>               
   </tr>
</table>
  

<h3 name='ado'>1. ADO.NET ( ActiveX Data Object )</h3>

- `ADO.NET` is a bridge between front end `controls` and backend `database`.
- It encapsulates all the data access operations, control interactions and display data.
- A `Data Provider` i.e. Connection, Command and DataAdapter ( `Select`, `Insert`, `Delete` and `Update` Command )
- And a `DataSet` i.e DataRelationCollection and DataTableCollection ( `DataTable`, Rows, Columns and Constraints )

<p><img src='Image/ADO.NET Objects.jpg'></p>

- `Connection` helps to connect `Data Source` for performing operations.
- `Command` is a `Query` or Stored Procedure to and from Database for `Extracting`, `Transforming` or `Loading` data.
- `DataAdapter` helps DataSet to `load` Data from multiple Databases or Data Source.
- `DataReader` has `Read only` access to data in Database.
- `DataRelationCollection` represents relationship between two `Tables`.

<h3 name='set'>2. DataSet vs DataReader</h3>

- Used to `Get` and `Store` data in a C#.

DataSet |  DataReader 
:--- | :---
`DataSet` has `Read Write` access to data | `DataReader` is used to retrieve or access `Read Only` data from Database
`SqlAdapter` fills data in DataSet | DataReader is created by calling `Command.ExecuteReader`
Speed to access data is `Slow` | Speed to access data is `Fast` due to `Read Only`
No need to `Open` or `Close` connection | Needs to `Open` and `Close` Connection Manually

<h3 name='execute'>3. ExecuteScalar | ExecuteReader | ExecuteNonQuery</h3>

ExecuteScalar | ExecuteReader | ExecuteNonQuery
:--- | :--- | :---
Is used when Query return `Single` Value | Is used when Query return `Multiple` Values | Is used when Query return no Data
e.g. First Row or Column from the Database | e.g. Multiple Rows and Columns (Iterations) | e.g. Only Returns Number of Rows Inserted, Updated or Deleted (Rows Affected)
