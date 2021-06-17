### Object Oriented Programming Concepts

<table>
  <tr>
    <th align=left><a href= "#class">1. Class</a></th>
    <th align=left><a href= "#int">2. Interface</a></th>
    <th align=left><a href= "#obj">3. Object</a></th>
    <th align=left><a href= "#abs">4. Abstraction</a></th>
    <th align=left><a href= "#enc">5. Encapsulation</a></th>
    <th align=left><a href= "#poly">6. Polymorphism</a></th>
    <th align=left><a href= "#inh">7. Inheritance</a></th>
  </tr>
</table>

<h3 name='class'>1. Class</h3>

- Blueprint or Template that Describes Attributes ( Physical Properties | Data Members ) and Method( Behavior ) of a Object.

```C#
public class Student  
 {  
     int id; 
     String name; 
 }  
```

<h3 name='int'>2. Interface</h3>

- `Blueprint` of a `Class`.
- Methods declared inside the Interface are `Abstract` Methods.
- Used to Achieve `Multiple` Inheritance.

```C#
using System;  

public interface Draw
{  
    void draw();  
}  

public class Rectangle : Draw  
{  
    public void draw()  
    {  
        Console.WriteLine("Drawing Rectangle...");  
    }  
}  

public class Circle : Draw
{  
    public void draw()  
    {  
        Console.WriteLine("Drawing Circle...");  
    }  
}  

public class TestInterface  
{  
    public static void Main()  
    {  
        Draw d;  
        d = new Rectangle();  
        d.draw();  
        d = new Circle();  
        d.draw();  
    }  
}  
```

```C#
Output :
Drawing Rectangle...
Drawing Circle...
```

<h3 name='obj'>3. Object</h3> 
- Instance of Class which has Property and Method

```C#
Student s1 = new Student();
```

- e.g. 
- `Person` is a `Class` 
- `Dia` is an `Instance` of Class `Person`
- `Property` : Dia has some `Attributes` ( Height, Weight, Color, Gender )    
- `Method` : `Behavior` and `Actions` of Dia ( Talk, Run, Play, Fight, Sing, Cry )

<h3 name='abs'>4. Abstraction</h3>
- Show only Important Information and `Hide` the Unnecessary Background Information.
- Main Purpose is to Hide the Unnecessary Details from Users.
- Help to Reduce Program `Complexity`.

<h3 name='enc'>5. Encapsulation</h3> 
- Bind together the `Data` and `Function` ( Class = Properties + Method )
- `Class` : Car
- `Properties` : ( Physical Attributes of Car | Color, Type, Size, Name, Model )
- `Method` : ( Action Performed by the Car | Use of Car | Drive | Stop )

<h3 name='poly'>6. Polymorphism (Many Forms)</h3>
- Having more than one form.
- e.g A Person at same time can have different Characteristics.
( Like a Man at same time is a Father, a Husband, an Employee and Different Behaviour at Different Situation )

### Similar Words

> Parent Class | Base Class    | Super Class
 
> Child Class  | Derived Class | Sub Class

<h3 name='inh'>7. Inheritance</h3> 
- The Process in which one class acquire the Property and Method of another Class.
- e,g `Child` Inherits from `Mom` and `Dad`.

### 1. Single Inheritance 
- Class `B` Inherit from Class `A` | New Class is Derived from Base Class
- e.g. `Boy` Inherit `Father` Properties and Behaviours.

### 2. Multilevel
- Class `C` Inherit from Class `B` and Class `B` Inherit from Class `A`
- e.g. `Boy` Inherit from `Father` and `Father` Inherit from `Grand Father`.

### 3. Multiple  
- Class `A` Inherit from Class `B` and Class `C` | A Class can be Derived from more than One Base Class
- e.g. Class Truck, Class Car, Class Bus Inherit from Class Vehicle.

### Method Overriding
- New Derived Class can `Inherit` and `Override` | Modify the Methods of its Base Class.

### Method Overloading 
- Creating Multiple Methods with `Same Name` but with different ( `Unique` ) Parameters.

### Operator Overloading
- Same Operator Behaves differently with Different Data Types according to Context.
- ( + Operator ) performs `Arithmetic` Operations between Two `Numbers` but performs `Concatenation` between Two `Strings`.

### Programming Constructs
- Common Building Blocks to Construct any Program.

1. `Sequence` : Step by Step Process ( Follow only One Direction )
2. `Selection` : Steps taken based on Conditions ( If Else or True False Condition )
3. `Iterations` : Repeated Process which can Change the Step based on Certain Conditions.

### String (https://www.w3schools.com/cs/cs_strings.asp)
- Sequence of `Characters`
- e.g. Character : 'A', 'K', 'Z'
- String : 

### Numbers 
- Integers, Floating Point Numbers, Complex Number, Binary or Hexadecimal Numbers

### Booleans (https://www.w3schools.com/cs/cs_booleans.asp)
- Only True ( `1` ) and False ( `0` ), Mostly used with Loops and Conditions.

### Array (https://www.w3schools.com/cs/cs_arrays.asp)
- Store Multiple Values in a Single Variable.
- e.g. string\[] cars = {"I20", "Swift", "Creta", "Verna"}


