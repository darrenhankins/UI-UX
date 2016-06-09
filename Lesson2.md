Thursday, June 9, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Lesson 2
###### Object-Oriented Programming

###### Think and Reflect on where your skills are at...

Objective Domain Matrix

* OOP is a programing technique that makes use of objects
* Objecst are self-containted data structures that consist of properties, methods and events

Classes
* A class defines a blueprint for an objects
* A class defines how the objects should be build and how they should behave
* A object is also know as an instance of a class

Defining a C# class
* class keyword name, variables (private-only class can access these variables), constructor, behavior
  * `private` variables

Methods
* is a block of code containg a series of statements
* defines the cactions or operations supportd by a class
* is defined by specifying the access level, the retrun type, the name of the method, and an optional list of parameters
  * if `void` a return statement with no value can be used

Constructors
* are special class methods that are executed when a new instance of a class is created
* are used to initialize the data members of the object
* must have exactly the same name as the class and they do not have a return type
* multiple constructors, each with a unique signature, can be defined for a class (first line of constructor is the `signature`, its the type of variable being passed)

Creating objects
* Objects need a template that defines how they should be built
* All objects created from the same template look and behave in a similar way
* `new` instantiates the object
* constructors job is to initialize variables

Properties
* `set` and `get` Properties
* are class memebers that can be accessed like data fields but contain code like a method
* has two accessors, `get` and `set`. The get accessor is used to return the property value, and the set accessor is used to assign a new value to the property

`Note: by default all variables should be set to 'private'`

The `this` Keyword
* `this` keyword is a reference to the current instance of the class (which is an object)
* You can use this the `this` keyword to refer to any member of the current object.

Delegates
* special objects that can hold a reference to a method with a specific signature
* Here, you define a `RectangleHandler` delegate that can hold a reference to a method that returns void and accepts a single parameter of the rectangle type
* The signature of `DisplayArea` method matches the `RectangleHandler` delegate and therefore can be assigned to one of its instance

```csharp
public delegate void RectangleHandler (Rectangle rect)

```

Events
* Are a way for a class to notify other classes or objects when something of interest happens
* The class that sends the notification is called a publisher of the event
* The class that receives the notification is called the subscriber of the event

```csharp

class Rectangle {

  public event EventHandler Changed;
  private double length;

  // this a a property
  public double Length {
    get {
      ...
    }

    set {
      length = value;
      Changed(this, EventArgs.Empty);
    }
  }
}

```
Subscribing to events
* The signature of the event handler method matches the requirements of the event's delegate

`Note: 'cast' an object`

Namespaces
* A namespace is a language element that allows you to organize code and create globally unique class names.
* The .NET Framework uses namespaces to organize all its classes
  * The System namespace groups all the fundamental classes
  * The System.Data namespace organizes classes for data access
  * The System.Web namespace is used for Web-related classes

Static members
* `static` keyword is used to declare members that do not belong to an individual objects but to a class itself
* When a instance of a class is created, a separate copy is created for each instance field, but only one copy of a static field is shared by all instances
* A `static` member cannot be referenced through an instance object. Instead, a static member is referenced through the class name

Values and References
* A value type directly stores dat within its memory
* Reference types store only a reference to a memory location. The actual data is stored at the memory location being referred to
* When you copy a reference type variable to another variable of the same type, only the references are copied. As a result, after the copy , both variables will point to the same object

Encapsulation
* Is a mechanism to restrict access to a class or class members in order to hide design decisions that are likely to change
* Access modifiers control where a type or type member can be used
    * `public` - access is not restricted
    * `private` - access is restricted to the containing class
    * `protected` - access is restricted to the containing class and to any class that is derived directly or indirectly from the containing class
    * `internal` - access is restricted to the code in the same assembly
    * `protected internal` - a combination of protected and internal - that is, access is restricted to any code in the same assembly and only to derived classes in another assembly

`Note: 'least' privileges applied to class structure`

Inheritance
* is an OOP feature that allows you to develop a class once, and then reuse that code over and over as the basis of new classes.
* The class whose functionality is inherited is called a base class
* The class that inherits the functionality is called a derived class
* A derived class can also define additional features that make it different from the base class
* Unlike classes, the structs do not support inheritance

`Note: 'struct' similar to 'class' but not a lot intelligence associated with it`

```csharp
class Polygon {
  ...
}
// Rectangle inheritance Polygon attributes
class Rectangle : Polygon
{
  ...
}
```

Abstract classes
* provides a common definition of a base class that can be shared by multiple derived classes
* often provides incomplete implementation
* to instantiate an abstract class you must inherit from it and complete its implementation

Sealed classes
* provide complete functionality but cannot be used as base class
* use the sealed keyword when you implementation is complete and you do not want a class or its member to be inherited

Inheriting from Objects
* The Object class is the ultimate base class of all the classes in the .NET Framework
* All classes in the .NET Framework inherit either directly or indirectly form the Object class

Casting
* in C# yo can cast an object to any of its base types
* all classes in the .NET Framework inherit either directly or indirectly from the Object class
* Assigning a derived class object to a base class object doesn't require any special syntax:
```csharp
Object o = new Rectangle (10,20);
```
* Assigning a base class object to a derived class object must be explicitly cast:
```csharp
Rectangle r = (Rectangle) o;
```
* At execution time, if the value of o is not compatible with the Rectangle class, the runtime throws a System.invalid.

The `is` Operator
* To avoid runtime errors such as InvalidCastException, the is operator can be used to check whether the cast is allowed before actually performing the cast

The `as` Operator
* The `as` operator is similar to the cast operation buy, in the case of `as`, if the type conversion is not possible, null is allowed before actually performing the cast

Polymorphism
* same name, different functionality
* Polymorphism is the ability of derived classes to share common functionality with base classes but still define their own unique behavior

Interfaces (contract)
* establish contracts through which objects can interact with each other without knowing the implementation details
* an interface definition cannot consist of any data fields or any implementation details such as method bodies
* A common interface defined in the System namespaces is the IComparable namespace. This is a simple interface defined as follows:
* Each class that implements IComparable is free to provide its own custom comparison login inside the CompareTo Method

`Note: You can only inherit on class at a time, however, you can inherit as many interfaces as you like. Specific order in identifying the class first then interfaces`
