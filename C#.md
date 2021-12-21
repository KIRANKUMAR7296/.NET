# C#

<table>
   <tr>
      <th align=left><a href='#con'>Constructor</a></th>
      <th align=left><a href='#gc'>Garbage Collector</a></th>
      <th align=left><a href='#box'>Boxing and Unboxing</a></th>
      <th align=left><a href='#type'>Data Type</a></th>
      <th align=left><a href='#int'>Int16 vs Int32 vs Int64</a></th>
   </tr>
</table>

<table>
   <tr>
      <th align=left><a href='#service'>Web Service</a></th>
      <th align=left><a href='#api'>Web API</a></th>
      <th align=left><a href='#iis'>IIS</a></th>
      <th align=left><a href='#grid'>Grid View Binding</a></th>
      <th align=left><a href='#char'>charAt()</a></th>
      <th align=left><a href='#each'>foreach()</a></th>
   </tr>
</table>

### 1. What is C# 

-  `C#` is an `object oriented`, compiled by `.NET` framework, microsoft's intermediate language.

<h3 name='con'>2. Constructor</h3>

- `Constructor` automatically `invokes` whenever an `object` is created.
- It initialize `Data Members` of new object.
- There are 2 `types` of Constructor 👇🏻
- `Default` Constructor : A Constructor without `Parameters`.
- `Parameterized` Constructor : A Constructor with `Parameters`.

<h3 name='gc'>3. Garbage Collector</h3> 

- Garbage Collector is an `automatic memory manager`, it `allocates` and `releases` memory for objects.
- Garbage Collector `collects` and `dispose` garbage memory to make memory available for new allocations.

<h3 name='box'>4. Boxing vs Unboxing</h3>

Boxing | Unboxing
:--- | :---
Converting a `value type` ( Char, Int ) to `reference type` ( Object ) | Converting `reference type` to `value type`
After conversion the value is stored in `Heap` | After Conversion value is stored in `Stack`

- e.g. Boxing 
```c#
int num = 7;       // num = Value Type Variable        
object obj = num;  // Boxing
```
- e.g. Unboxing

```c#
int num = 7;  
object obj = num;  // Boxing
int i = (int)obj;  // Unboxing
```
<h3 name='type'>5. Data Types</h3>

<table>
   <tr><th colspan=3>Data Types in C#</th></tr>
   <tr><th>Value Type</th><th>Reference Type</th><th>Pointer Type</th></tr>
   <tr><td>Variable holds Data Value</td><td>Variable holds Memory Location</td><td>Variable holds Memory Address</td></tr>
   <tr>
      <td>
         <ul>
            <li>Integer (byte 8, short 16, int 32, long 64)</li>
            <li>floating (float 32, double 64, decimal 128)</li>
            <li>char ("A")</li>            
            <li>bool (true, false)</li>
         </ul>
      </td>
      <td>
         <ul>
            <li>String</li>
            <li>Array</li>
            <li>Class</li>
            <li>Object</li>
            <li>Interface</li>
         </ul>
      </td>
       <td>
         <ul>
            <li>Pointers</li>
         </ul>
      </td>
   </tr>
   <tr><td>Default Value is 0</td><td>Default Value is NULL</td><td>Default Value is NULL</td></tr>
   <tr><td>Assignment means copying Actual Data</td><td>Assignment means copying Reference</td><td></td></tr>
</table>

<h3 name='int'>6. Int16 vs Int32 vs Int64</h3>

- Stores `Positive` and `Negative` Integers.
- Each have different `Capacity` and `Range`. 

Int16 | Int32 | Int64
:--- | :--- | :---
`16` Bit Signed Integer | `32` Bit Signed Integer | `64` Bit Signed Integer
Takes `2` Bytes Memory Space | Takes `4` Bytes Memory Space | Takes `8` Bytes Memory Space

<h3 name='service'>Web Service</h3>

- `Service` offered by one device to another device.
- `Communicating` with each other via `World Wide Web`.
- `Server` running on Computer Device.
- `Request` and `Response` in the form of `HTML`, `XML`, `JSON`...

<h3 name='api'>Web API</h3>

- Application Programming Interface.
- A Framework for building `HTTP` Services that can be accessed by Client anywhere.
- API can be accessed using Browser on `Desktop`, `Laptop`, `Tablet` and `Mobile`.
- Supports `JSON` and `XML` format.

<h3 name='iis'>IIS</h3>

- Internet Information Services ( Web Server created by Microsoft )
- Used to `Host` ASP.NET Web Applications and Static Websites.
- Inbuilt Authentication and Authorization
- `Authentication` : Verify whether User is a `Valid` User ( Login Form : User Name and Password )
- `Authorization` : Check if you have a `Permission` to Access ( Secure Access )

<h3 name='grid'>Grid View Bind</h3>

- Grid View is used to Display `Tabular` Data ( Rows and Column ) on Web Page which is stored in a Database.
- To `Display` the Data we need to `Bind` the Grid View to the Table in the Database.
- We Select the Columns we want to Show on Grid View and use `ExecuteReader` to Read Data from Table.
- Binding requires `Open` Connection and Connection is `Closed` after Binding.

<h3 name='char'>charAt()</h3>

- `charAt()` : Character at specific `Index`.
- In C# Indexing Starts from `0`.

```c#
str.charAt(8)  // Character at Index Location 8
```

<h3 name='each'>foreach()</h3>

- `foreach()` : `Loop` iterate through each items of an `Array` or `Collection`
- An alternative to `for` loop.

```c#
foreach (item in iterables)
{
    body
}
```

### 7. Difference between Public, Static and Void 

- `Public` : Public declared variables or methods are accessible anywhere in the application.
- `Static` : Static declared variables or methods are accessible without creating any instance of the class.
- `Void`   : The variables or methods doesn't return any value.

### 8. ref parameters 

- Argument passed as reference must be initialized before passing to method.

### 9. out parameters

- No need to be initialized before passing to method.

### 10. use of 'using' statement ?

- Obtain a resource and process it and automatically dispose after execution.

### 11. Serialization vs Deserialization

Serialization | Deserialization
:--- | :---
Converting `Object` into `Byte Stream` | Creating an `Object` from a `Byte Stream`.

### 12. Constants vs Read Only 

Constant | Read Only
:--- | :---
Variables are Declared and Initialized at `Compile` Time | `Read Only` is used only to assign value at `Run` Time

### 13. Custom Controls ?

- Controls generated as Compiled Code (.dlls)
- Developer can Drag and Drop to Web Forms
- `dll` are stored in `bin` folder of the project.
- we can use them by adding reference.

### 14. Sealed Class ?

- `Restricts` the class from Inheritance. ( Sealed class can be used to Create another class )

### 15. Array vs Array List ?

Array | Array List
:--- | :---
Is a `Fixed` Size Data Structure | Is not a Fixed Size Data Structure
Items are Accessed by `Index` | Items are Accessed by using `Method`

### 16. System.String vs System.Text.StringBuilder 

`System.String` :  | `System.Text.StringBuilder`
:--- | :---
Strings are `Immutable` (Cannot Change the value) | Strings are `Mutable` (Can change the Value)
If we `modify` value of String then New memory is allocated and old memory is released. | Value can be modified at same memory location.

### 17. System.Array.CopyTo() vs System.Array.Clone()

- Both performs `Shallow` Copy.
- `Clone`  : Creates a same copy of Array. 
- `CopyTo` : Copies value of One Array into another New Array.

### 18. Finalize() vs Dispose()

- `Dispose()` : Called when we want object to completely release resource.
- `Finalize()` : Do same but do not assure garbage collection of an Object (do not leave memory allocation)

### 19 Circular Reference 

- Situation in which two or more resource are dependent on each other and cause lock condition.

### 20 Generics in C# ?

- Used to make reusable class to reduce redundancy, increase performance and save time.

### 21 Object Pool ?

- Container having Objects to be used. Keep track of available Objects and Objects currently in use.

### 22 What are Custom Exceptions ? 

- Some Errors are need to be handles as per user requirement.

### 23 How to Inherit Class ?

- public class DerivedClass : BaseClass
> Derived Class : Child Class  : Sub Class  
> Base Class    : Parent Class : Super Class 

### 24. What is the base class in .net from which all the classes are derived from ? ***

- `System.Object`

### 25. What are the different ways a method can be overloaded ?

- We can change the `Data Types` of parameters ( Data type of the new parameters can be `changed` while deriving new )
- We can change the `Order` of parameters ( `Order` of the parameters can be `changed` while deriving new class )
- We can change the `Number` of parameters ( New parameters can be `added` while deriving new class )

Struct | Class
:--- | :--- 
`Struct` is stored on the `Stack`. | `Class` is stored on the `Heap`
`Struct` do not support `Inheritance` and `Polymorphism` | `Class` support `Inheritance` and `Polymorphism`

### 26. Abstract Class

- A special type of class that cannot be instantiated ( Cannot be used to create `objects` )
- Designed to be inherited by `subclasses` that either implement or `override` its methods. 

### 27. Abstract Method

- Abstract Method are only used in an `Abstract Class`
- Method does not have any body it is just derived from its base `Abstract Class`
- It can be `overridden` by the derived class.

### 28. Delegates

- A delegate is a `reference type` variable that holds the reference to a `method`
- The reference can be changed at `runtime`
- Delegates are especially used for implementing `events` and the `call back` methods.
