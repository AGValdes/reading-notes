# Class 04: Objects and Classes

## Classes
Classes are **reference types**
- When the object is created, enough memory is allocated on the managed heap for that specific object, and the variable holds only a reference to the location of said object. 

<code> //Declaring an object of type MyClass.
MyClass mc = new MyClass(); 

//Declaring another object of the same type, assigning it the value of the first object.
MyClass mc2 = mc; </code>

- Classes are declared by using the class keyword followed by a unique identifier
- A class defines a **type of object**, but it is **not** an object itself.
-  **object:** a concrete entity based on a class, and is sometimes referred to as an **instance** of a class.
- Objects can be created by using the new keyword followed by the name of the class that the object will be based on
``Customer object1 = new Customer();``
- you can create an object reference without creating an object at all
**Inheritence:**
- When you create a class, you can inherit from any other class that is not defined as sealed, and other classes can inherit from your class and override class virtual methods
- a class is declared by using a **base class** from which it **inherits** data and behavior

<code> public class Manager : Employee
{
    // Employee fields, properties, methods and events are inherited
    // New Manager fields, properties, methods and events go here...
}</code>

-  An **abstract** **class** contains abstract methods that have a signature definition but no implementation

<code>using System;

public class Person
{
    // Constructor that takes no arguments:
    public Person()
    {
        Name = "unknown";
    }

    // Constructor that takes one argument:
    public Person(string name)
    {
        Name = name;
    }

    // Auto-implemented readonly property:
    public string Name { get; }

    // Method that overrides the base class (System.Object) implementation.
    public override string ToString()
    {
        return Name;
    }
}
class TestPerson
{
    static void Main()
    {
        // Call the constructor that has no parameters.
        var person1 = new Person();
        Console.WriteLine(person1.Name);

        // Call the constructor that has one parameter.
        var person2 = new Person("Sarah Jones");
        Console.WriteLine(person2.Name);
        // Get the string representation of the person2 instance.
        Console.WriteLine(person2);

        Console.WriteLine("Press any key to exit.");
        Console.ReadKey();
    }
}
// Output:
// unknown
// Sarah Jones
// Sarah Jones</code>

# Constructors
- Whenever a class or struct is created, its constructor is called
- A class or struct may have multiple constructors that take different arguments
- If you don't provide a constructor for your class, C# creates one by default that instantiates the object and sets member variables to the default values
-  If you don't provide a constructor for your struct, C# relies on an implicit parameterless constructor to automatically initialize each field to its default value
- A constructor is a method whose name is the **same as the name of its type**
- Its method signature includes only the **method name** and its **parameter** list; it **does not** include a **return type**

<code>public class Person
{
   private string last;
   private string first;

   public Person(string lastName, string firstName)
   {
      last = lastName;
      first = firstName;
   }

   // Remaining implementation of Person class.
}</code>

**static constructor:** initializes static members of the type
- Static constructors are parameterless
<code>public class Adult : Person
{
   private static int minimumAge;

   public Adult(string lastName, string firstName) : base(lastName, firstName)
   { }

   static Adult()
   {
      minimumAge = 18;
   }

   // Remaining implementation of Adult class.
}</code>

## Properties
- Properties enable a class to expose a public way of getting and setting values, while hiding implementation or verification code.

- A get property accessor is used to return the property value, and a set property accessor is used to assign a new value. These accessors can have different access levels. For more information, see Restricting Accessor Accessibility.

- The value keyword is used to define the value being assigned by the set accessor.

- Properties can be read-write (they have both a get and a set accessor), read-only (they have a get accessor but no set accessor), or write-only (they have a set accessor, but no get accessor). Write-only properties are rare and are most commonly used to restrict access to sensitive data.

- Simple properties that require no custom accessor code can be implemented either as expression body definitions or as auto-implemented properties.

## Stack and Heap
- The **Stack** is more or less responsible for keeping track of what's executing in our code (or what's been "called").

- The **Heap** is more or less responsible for keeping track of our objects (our data, well... most of it - we'll get to that later.).
![stack/heap](https://csharpcorner.azureedge.net/UploadFile/rmcochran/csharp_memory01122006130034PM/Images/heapvsstack1.gif)

## Garbage Collection Fundementals
 **garbage collector (GC)** serves as an automatic memory manager. The garbage collector manages the **allocation and release of memory** for an application
 - Frees developers from having to manually release memory.

- Allocates objects on the managed heap efficiently.

- Reclaims objects that are no longer being used, clears their memory, and keeps the memory available for future allocations. Managed objects automatically get clean content to start with, so their constructors don't have to initialize every data field.

- Provides memory safety by making sure that an object cannot use the content of another object.


