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
 * If a task is perfomed in different ways is known as polymorphism.
 * It can be achived by using method overloading and overriding.
 * A single object can refer to super class or sub class depending upon reference type is called polymorphism.

  ![image](https://github.com/user-attachments/assets/d2d62965-ed0d-4b71-bec8-f5122fe0184b)
 * Above, Using manipulation referene type we can call the Addition class add() method.

 * **Types of polymorphism**
 * RunTime Polymorphism
 * CompileTime Polymorphism

 ### 10. Method Overloading v/s Method Overriding
 |   Method overloading |  Method Overriding  |
 |:---------------------|:--------------------|
 | Method overloading increases the readability of the program | Method overrriding provides specific implementation of the method that is already provided by parent class|
 |Method overloading is performed within a class | Method overrriding is performed within two classes and have IS-A relationship |
 | In case of method overloading, parameter must be different |  In case of method overriding, parameter must be same |
 | Method loading is an example of compiletime polymorphism | Mehtod overrriding is an example of run time polymorphism |

 ### 11. Compiletime Polymorphism v/s Runtime Polymorphism
 | Compiletime Polymorphism | Runtime Polymorphism |
 |:------------------------- | :--------------------|
 | In ctp, call is resolved by compiler | In rtp, call is not resolved by compiler |
 | CTP is known as early binding and static binding | RTP is known as dynamic binding and late binding |
 | Overloading in ctp, one method shares the same name with diff parameters, signature and return type | Overriding in rtp, Have the same name with same parameter or signature and same return type but associated in a class and its subclass.
 | It provides fast execution |  It provies slow execution |

 * **Overloading**
   
   ![image](https://github.com/user-attachments/assets/3a0a101d-233f-44fc-ab39-a451fe5389bc)
 * Here the add() method has different parameters in the Addition class is overloaded in the same class as with the super-class.

 * **Overriding**
   
   ![image](https://github.com/user-attachments/assets/328fcd0c-bec3-4756-b557-058af0535c89)
   * addition.add() method calls the add() method in the Sub-class and not the parent class. So it overrides the Super-class method and is known as Method Overriding.

 ### 12. Abstraction 
 * Abstraction is the process of hiding implementation details and showing only funtionality to the user. (e.g process of phone)
 * **There are two ways to achieve abstraction**
 * **Abstract class:** A class which is declared with abstract keyword is known as abstract class. It can have abstract and non-abstract methods.

   ![image](https://github.com/user-attachments/assets/ce11511b-0e9f-42c0-abee-9045df5e17f7)

 * **Interface:** An interface is a blueprint of a class. It has static constants and abstract methods. Interface in java is a mechanism to achieve abstraction.
* An interface is a template that has only method declarations and not the method implementation.

  ![image](https://github.com/user-attachments/assets/2b0fc47e-b6ff-46b5-b83b-fbc60a145229)
  
  ![image](https://github.com/user-attachments/assets/bfad4f1e-e4f2-46b0-bce4-44aa54d8ef49)

 * **Why we use interface**
 * To achieve abstraction
 * To support funtionality of multiple inheritance.
 * To achieve loose coupling.

 ### 13. Array v/s Arraylist
 | Array | ArrayList |
 |:-------|:---------|
 | Array is a fixed length data structure and size should be given at the time of array declaration | Arralylist is a variable length collection class|
 |Array can store primitives and objects in java | Arraylist can store only objects in java|
 | Array length can't be changes once it is created | ArrayList can be changed |
 | Need to specify an index to put an object into array. e.g name[1] = “book” | No index required. e.g name.add(“book”) |

 ### 14. String v/s StringBuilder v/s StringBuffer
  * **String:** It is immutable and string variables are stored in constant string pool. Once the string references changes the old value that exists in constant string pool, it can't be erased.

    ![image](https://github.com/user-attachments/assets/e6faf05b-1704-4db7-9a77-47a979367c29)

 * **StringBuffer:** StringBuffer is mutable. String values are stored in stack and if the values are changed then the new value replaces the old value.
 * The stringBuffer is synchronized which is thread-safe.
 * Perfomance is slower than stringBuilder.

    ![image](https://github.com/user-attachments/assets/b8450dd9-6e5b-4977-adf2-74ef29b1becc)

 * **StringBuilder:** StringBuilder is mutable and its values are stored in heap. It is not thresd-safe so it is faster in performance.

### 15. Public v/s Private access modifier
* Methods and instance variables are known as members.
* **Public Access Modifier:**
* Public members are visible in the same package as well as the outside package that is for other packages.
* **Private Access Modifier:**
* Private members are visible in the same class only and not for the other classes in the same package as well as classes in the outside packages.

### 16. Default v/s Protected access modifier
* **Default:** Methods and variables declared in a class without any access specifiers are called default.
  
  ![image](https://github.com/user-attachments/assets/7dbbf4c8-19e5-4a4e-ae03-05018c542fed)
* **Protected:** Protected is the same as Default but if a class extends then it is visible even if it is outside the package.

  ![image](https://github.com/user-attachments/assets/ac67f02b-fa39-42bf-837f-04e91f76e816)

### 17. HashMap v/s HashTable
| HashMap | HashTable |
|:--------|:----------|
| HashMap is not synchronized | HashTable is synchronized |
| HashMap is not thread safe | HashTable is thread-safe |
| Iterator is used to iterate the values | Enumerator is used to iterate the values |
| Allows one null key and multiple null values | Doesn't allow anything that is null |
| Performance is higher than hashtable | Performance is slow |

### 18. HashSet v/s TreeSet 
| HashSet | Treeset |
|:-------- |:---------|
| Inserted elements are in random order | Maintains the elements in sorted order |
| Can able to store null objects | couldn't store the null objects |
| performance is fast | Performance is slow |

### 19. HashMap v/s HashSet
 | HashMap | HashSet |
 |:---------|:--------|
 | HashMap stores key-value pair | HashSet stores objects |
 | HashMap does not allow duplicate keys but duplicate values are allowed | HashSet does not allow duplicate values |
 | HashMap can contains single null key and multiple null values | HashSet can contain  a single null value |
 | HashMap uses the put() method to add elements in the Map | HashSet uses the add() to add element to the Set |

 ### 20. Abstract class v/s Interface
 | Abstract Class  | Interface |
 |:----------------|:--------------|
 | Abstract class can have abstract and non-abstract method | Interface can have only abstract method |
 | Abstract class does not support multiple inheritance | Interface supports multiple inheritance |
 | Abstract class can provide implementation of interface | Interface can't provide implementation of abstract class |
 | Abstract keyword is used to declare abstract class | Interface keyword is used to declare interface |
 | Abstract class can be extended using keyowrd 'extends' | Interface can be implemented using keyword 'Implement' |
 
### 21. Collectioons in java


