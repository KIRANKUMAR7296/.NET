# C#

### 1. What is C# 
-  An Object Oriented, Compiled by `.NET` Framework to generate Microsoft Intermediate Language.

### 2. Difference between Public, Static and Void 
- `Public` : Public declared variables or methods are accessible anywhere in the application
- `Static` : Static declared variables or methods are accessible without creating any instance of the class.
- `Void`   : The variables or methods doesn't return any value.

### 3. Object : Instance of Class, through which we access the methods.
   e.g Class     : Car 
       Attribute : Color, Type
       Method    : Drive, Stop

### 4. Constructor : Automatically invokes | called whenever an object is created.

### 5. ref parameters : An Argument passed as reference must be initialized before passing to method.

### 6. out parameters : No need to initialized before passing to method.

### 7. use of 'using' statement ?
-  Obtain a resource and process it and automatically dispose after execution.

### 8. What is Serialization ?
-  Converting Object into Byte Stream.

9. What is Deserialization ? 
-  Creating an Object from a Stream of Bytes.

10. Constants vs Read Only 
-   Constant Variables are declared and Initialized at Compile Time
-   Read Only is used only to assign value at Run Time.

11. Value type and Reference Type ?
-   Value Type : Holds a Data Value within its Memory Space.
    Reference Type : Stores address of Object where the value is stored. (Pointer to Memory Location)

12. Custom Controls ?
-   Controls generated as Compiled Code (.dlls)
-   Developer can Drag and Drop to Web Forms
-   dll are stored in bin folder of the project.
-   we can use them by adding reference.

13. Sealed Class ?
-   Restricts the class from Inheritance. (Sealed class can be used to Create another class)

14. Method Overloading and Method Overriding ?
-   Overloading  : Creating Multiple Methods with same name but with different (unique) Parameters.
    Overriding   : Changing Attributes and Methods while Deriving New Class from Existing one. 

15. Array vs Array List ?
-   Array      : Fixed Size Data Structure. | Access by [index] 
    Array List : Not Fixed Size. | Part of Collection Framework | Access by using Methods.

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

26. Struct vs Class
-  | Struct                                       | Class                                  |
   | -------------------------------------------- - -------------------------------------- |
   | Stored on the Stack.                         | Stored on the Heap.                    |
   | Do not support Inheritance and Polymorphism. | Supports Inheritance and Polymorphism. |

