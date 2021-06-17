# C#

<table>
   <tr>
      <th align=left><a href='#con'>Constructor</a></th>
      <th align=left><a href='#gc'>Garbage Collector</a></th>
      <th align=left></th>
   </tr>
</table>

### 1. What is C# 

-  An Object Oriented, Compiled by `.NET` Framework to generate Microsoft Intermediate Language.

<h3 name='con'>2. Constructor</h3>

- Automatically `invokes` whenever an object is created.
- Initialize `Data Members` of New Object.
- `Default` Constructor : A Constructor with no `Arguments`.
- `Parameterized` Constructor : A Constructor which has `Parameters`.

<h3 name='con'>3. Garbage Collector</h3> 

-  An Automatic Memory Manager ( `Allocate` and `Release` Memory for Objects )

<h3 name='box'>Boxing vs Unboxing</h3>

Boxing | Unboxing
:--- | :---
Converting a Value Type (Char, Int) to Reference Type (Object) | Converting Reference Type into Value Type 
Store in `Heap` | Store in `Stack`

- e.g. Boxing 
```c#
int num = 7;       // num = Value Type Variable        
object obj = num;  // Boxing

- e.g. Unboxing

```c#
int num = 7;  
object obj = num;  // Boxing
int i = (int)obj;  // Unboxing
```
   

4. ADO.NET (ActiveX )
 - Bridge between Front end controls and backend database.
 - Encapsulates all the Data Access Operations, Control Interactions and Display Data.

   Data Provider : Connection, Command and DataAdapter (Select, Insert, Delete and Update Command)
   DataSet : DataRelationCollection and DataTableCollection (DataTable, Rows, Columns and Constraints)

   Connection  : Connect Data Source for performing Operations.
   Command     : Query or Stored Procedure to and from Database for Extracting, Transforming or Loading data.
   DataAdapter : Helps DataSet to Load Data from Multiple Databases or Data Source.
   DataReader  : Read only Access to Data in Database.
   DataRelationCollection : represents relationship between two tables.

5. DataSet vs DataReader

   DataSet                   |  DataReader 
   Read Write Access to Data |  Read Only Access to Data
   Slow Access               |  Fast Access
   No need of Connection     |  Need Connection

6. ExecuteScalar 
 - Used when Query Returns Single Value. (First Row or First Column from the Database)

7. ExecuteReader 
 - Used when Query Returns Multiple Value (Set of Rows and Columns)

8. ExecuteNonQuery
 - Used when Query doesn't returns Data from Database. 
 - Only returns Integer specifying Number of Rows Inserted, Updated or Deleted.	

9. Clustered Index 
 - Defines the Order in which Data is Physically stored in a Table.
 - When we Create a Table with ID as PRIMARY KEY, this Automatically creates Clustered Index.

10. Non Clustered Index 
 - Doesn't Sort the Physical Data inside the Table.
 - Non Clustered Index is stored at different place then the Table Data.
 - e.g. Textbook content | Index is located on first page but the actual content is all at different pages.
 - Index contains column value and Address of the Record.



### 3. Difference between Public, Static and Void 

- `Public` : Public declared variables or methods are accessible anywhere in the application.
- `Static` : Static declared variables or methods are accessible without creating any instance of the class.
- `Void`   : The variables or methods doesn't return any value.

### 4. ref parameters 

- Argument passed as reference must be initialized before passing to method.

### 5. out parameters

- No need to be initialized before passing to method.

### 7. use of 'using' statement ?

- Obtain a resource and process it and automatically dispose after execution.

### 8. What is Serialization ?

- Converting `Object` into `Byte Stream`.

### 9. What is Deserialization ? 

- Creating an `Object` from a `Byte Stream`.

### 10. Constants vs Read Only 

- `Constant` Variables are declared and Initialized at `Compile` Time.
- `Read Only` is used only to assign value at `Run` Time.

11. Value type and Reference Type ?

- `Value` Type : Stores `Data Value` in Memory Space.
- `Reference` Type : Stores `Address` of Object where the value is stored. ( Pointer to Memory Location )

12. Custom Controls ?
-   Controls generated as Compiled Code (.dlls)
-   Developer can Drag and Drop to Web Forms
-   dll are stored in bin folder of the project.
-   we can use them by adding reference.

13. Sealed Class ?
-   `Restricts` the class from Inheritance. ( Sealed class can be used to Create another class )

15. Array vs Array List ?

- `Array` : Fixed Size Data Structure. | Access by [index] 
- `Array List` : Not Fixed Size. | Part of Collection Framework | Access by using Methods.

16. System.String vs System.Text.StringBuilder 
-   System.String : Immutable (Cannot Change the value) 
    if we modify value of String then New memory is allocated and old memory is released.

-   System.Text.StringBuilder :  Mutable (Can change the Value)
    Value can be modified at same memory location.

17. System.Array.CopyTo() vs System.Array.Clone()
-   Both performs shallow copy
    Clone  : Creates a same copy of Array. 
    CopyTo : Copies value of One Array into another New Array.

18. Finalize() vs Dispose()
- Dispose()  : Called when we want object to completely release resource.
  Finalize() : Do same but do not assure garbage collection of an Object (do not leave memory allocation)

19 Circular Reference 
- Situation in which two or more resource are dependent on each other and cause lock condition.

20 Generics in C# ?
- Used to make reusable class to reduce redundancy, increase performance and save time.

21 Object Pool ?
- Container having Objects to be used. Keep track of available Objects and Objects currently in use.

22 What are Custom Exceptions ? 
- Some Errors are need to be handles as per user requirement.

23 How to Inherit Class ?
- public class DerivedClass : BaseClass

Other Name for ( Derived Class : Child Class  : Sub Class   )
Other Name for ( Base Class    : Parent Class : Super Class )

24. What is the base class in .net from which all the classes are derived from ? ***
- System.Object

25. What are the different ways a method can be overloaded ?
- Different Data Types of Parameter (Data Type of the New Parameters can be changed while Deriving New)
  Different Order of Parameters (Order of the Parameters can be changed while Deriving New Class)
  Different Number of Parameters (New Parameters can be added while Deriving New Class)

Struct | Class
:--- | :--- 
Stored on the `Stack`. | Stored on the `Heap`
Do not support Inheritance and Polymorphism | Supports Inheritance and Polymorphism 

