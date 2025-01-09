# Core Java


### 1. Features of java
 * **oops concept:**
 * **Platform independent:** A single program can work on different platforms without any modifications
 * **High Performance:**
 * **Multi Threaded:** A flow of execution is known as a thread. JVM creates a thread which is called the main thread. The user can create multiple threads by extending thread class or by implementing the runnable interface.
                 
 ### 2. Constructor
 * constructor is a block of code which is similiar to a method. It is called when an instance of object is created and memory is allocated for that object. Java compiler creates a default constructor when a class does not any constructor. It is used to initialize the state of object and invoked implicitly. Constructor name must be same as its parent class name.

 **Two types of constructor**
 * **Default constructor:** A constructor is called default constructor when it does not have any parameter. Default constructor is used to provide default values to the object like null and 0.
 * **Parameterized constructor:** A constructor has specific number of paramters is called parameterized constructor. It is used to provide different values to distinct objects. We can provide the same value also.

 ### 3. Constructor v/s Method
   |       constructor   |      Method       |
   |:--------------------|:------------------|
   | Constructor is used to initialize the state io object | Method is used to expose the behaviour of object |
   | Constructor must not have return type | Method may or may not have return type|
   | Constructor is invoked implicitly     |  Method is invoked explicitly |
   | Java compiler provide default constructor |  Java compiler does not provide default method |
   | Constructor name must be same as its parent class name |  Method name may or may not be the same as its parent class name|

  ### 4. Local variable v/s Instance variable
   | Local variable   |  Instance variable  |
   |:-----------------|:--------------------|
   | Local variable can be seen inside the method | Instance variable can be seen inside the class and outside the methods.|
   | Local variable is defined inside the method | Instance variable is defined inside the class |
   | Local variable can't be accessed | Instance variable can be accessed by using access modifier public|

  ### 5. Class
  * A class is a group of objects which have common properties. It is a blueprint from which object is created and it is a logical entity. A class can contain:
  *  Fields
  *  Mdthods
  *  Constructors
  *  Nested class and interface

  ### 6. Object
  * An entity that has state and behaviour is known as an object.
  * It can be physical and local entity.
    | Three Characteristics |
    |:----------------|
    | state: Represnts the date of an object |
    | Behaviour : Represents the behaviour of an object |
    | Identity : An object identity is typically implemented by unique id.|
  * An object is an instance of a class.

 ### 7. Inheritance
 * A process of acquiring properties of a class from another class is called inheritance. It is also known as IS-A relationship.
 * The class which has common property is called super class/ parent class/ base class.
 * The class which extends to its parent class is known as sub class/ derived class/ child class.
 * **Two reasons to go for inheritance**
   1. Generalisation : superclass is the generalised form of subclass.
   2. Reusability
 * **Advantages**
   1. Achieve data reuasability.
   2. Avoid data redundancy
   3. Achieve generalisation that helps to achieve polymorphism and abstraction.
 * **Three types of inheritance**
   1. Single
   2. Mutilevel
   3. Hierarchical
  
 ### 8. Encapsulation
 * A process of wrapping code and data together into single unit. e.g capsule
 * **Advantages**
 * We can make the class read only or write only
 * Provides control over data
 * Achieve data hiding
 * Make the variable private or protected.
 * Use public accessor method get and set.

### 9. Polymorphism
   
