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

- `IIS` stands for `Internet Information Services`  
- `IIS` is a `Web Server` created by `Microsoft`
- It is used to host `ASP.NET Web Applications` and `Static Websites`
- It consists of inbuilt `Authentication` and `Authorization`
- `Authentication` means to `verify` whether user is a `valid` user ( Login Form : User Name and Password )
- `Authorization` means to check if you have a `permission` to access the resource or database ( Secure Access )

<h3 name='grid'>Grid View Bind</h3>

- `Grid View` is used to display `tabular` data ( rows and columns ) on web page which is stored in a database.
- To `display` the data we need to `bind` the `Grid View` to the table in the database.
- We select the columns we want to show on `Grid View` and use `ExecuteReader` to read data from table.
- Binding requires `open` connection and connection is `closed` after binding.

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

- `Public` : Public declared `variables` or `methods` are accessible anywhere in the application.
- `Static` : Static declared `variables` or `methods` are accessible without creating any instance of the class.
- `Void`   : The `variables` or `methods` doesn't return any value.

### 8. ref parameters 

- Argument passed as reference must be initialized before passing to method.

### 9. out parameters

- Out parameters states that no need to be initialize parameters before passing to method.

### 10. use of 'using' statement ?

- `Using` statement is used to obtain a `resource` and process it and automatically `dispose` after execution.

### 11. Serialization vs Deserialization

Serialization | Deserialization
:--- | :---
Converting `Object` into `Byte Stream` | Creating an `Object` from a `Byte Stream`.

### 12. Constants vs Read Only 

Constant | Read Only
:--- | :---
Variables are declared and initialized at `compile` time | `Read Only` is used only to assign value at `run` time
Value is same through out the process | Any new value can be assigned at the run time.

### 13. Custom Controls ?

- Custom controls are `controls` generated as compiled code (.dlls)
- Developer can `drag` and `drop` to `web forms`
- `dll` are stored in `bin` folder of the project.
- we can use them by adding reference to the location of `dll` file.

### 14. Sealed Class ?

- Sealed Class `restricts` the class from `Inheritance` ( Sealed class can be used to create another class )

### 15. Array vs Array List ?

Array | Array List
:--- | :---
`Array` is a `fixed` size data structure | `Array List` is not a fixed size data structure
Items inside Array are accessed by `Index` | Items inside Array List are accessed by using `Method`

### 16. System.String vs System.Text.StringBuilder 

`System.String` :  | `System.Text.StringBuilder`
:--- | :---
`Systen.Strings` are `immutable` (Cannot change the value once assigned) | `System.Text.StringBuilder` are `mutable` (Can change the value)
If we `modify` value of String then `new memory` is allocated and old memory is released. | We `modify` the value at same memory location.

### 17. System.Array.CopyTo() vs System.Array.Clone()

- Both performs `Shallow` Copy.
- `Clone`  : Creates a same exact `copy` of Array. 
- `CopyTo` : Copies value from one array into another new array.

### 18. Finalize() vs Dispose()

- `Dispose()` is called when we want object to completely release the resource.
- `Finalize()` also release the resource but it does not assure `garbage collection` of an object (do not leave memory allocation)

### 19 Circular Reference 

- `Circular Reference` is a situation in which two or more resource are `dependent` on each other and cause `lock` condition.

### 20 Generics in C# ?

- `Generics` are ssed to make reusable class to reduce redundancy, increase performance and save time.

### 21 Object Pool ?

- `Object Pool` is a container having objects to be used. 
- It keeps track of available objects and objects currently in use.

### 22 What are Custom Exceptions ? 

- Some `errors` that are need to be handled as per user requirement.

### 23 How to Inherit Class ?
```.net
public class DerivedClass : BaseClass
```

`Derived Class` is also called as `Child Class` or `Sub Class`
`Base Class` is also called as `Parent Class` or `Super Class` 

### 24. What is the `base class` in `.net` from which all the classes are derived from ? ***

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
