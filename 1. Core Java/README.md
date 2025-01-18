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
 
### 21. Collections in java
 * Collection is a framework that is designed to store the objects and manipulate the design to store the objects.
 * **Collections are used to perform the following operations:**
 * Searching
 * Sorting
 * Manipulation
 * Insertion
 * Deletion
 * A group of objects is known as collections. All the classes and interfaces for collecting are available in java util package.

### 22. Classes and Interfaces are available in collections
 * **Interfaces**
 * Collection
 * List
 * Set
 * Map
 * Sorted Set
 * Sorted Map
 * Queue
 * **Classes**
 * Lists
 * ArrayList
 * Vector
 * Linked List
 * **Sets**
 * HashSet
 * Linked HashSet
 * TreeSet
 * **Maps**
 * HashMap
 * HashTable
 * TreeMap
 * Linked Hashed Map
 * **Queue**
 * Priority Queue

### 23. Ordered v/s Sorted
 * **Ordered:-** It means the values that are stored in a collection is based on the values that are added to the collection. So we can iterate the values from the collection in a specific order.
 * **Sorted:-** Sorted mechanisms can be applied internally ox externally so that the group objects sorted in a particular collection is based on the properties of the objects.
   
### 24. Explain the different lists available in the collection.
* Values added to the list are based on the index position and it is ordered by index position. Duplicates are allowed.
  
* **ArrayList:-**
* It is an ordered collection by index and not sorted.
* It implements the random access interface.

  ![image](https://github.com/user-attachments/assets/95a805d0-56e7-4c29-a9cc-85b6de04fc1b)
  
* **Vector:-**
* It is same as ArrayList
* Vector methods are synchronized
* Vector also maintains the insertion order and accepts the duplicates.
* It also random access.
* Thread safety usually causes performacen hit.
  ![image](https://github.com/user-attachments/assets/5975a2d9-2881-47be-b1e0-4a394f7a0d46)

* **Linked List:-**
* Elements are doubly linked to one another
* Performance is slower than ArrayList
* Good choice for insertion and deletion
* Maintains the insertion order and accepts the duplicates.
* In Java 5.0, it supports common queue methods peek(),pool(),offer() etc.

  ![image](https://github.com/user-attachments/assets/86de4454-bcc0-4f94-a4d6-f00793fe06f1)

### 25. Explain about Set and their types in a collection.
* Set cares about uniqueness. it does not allow duplications. Here 'equals()' method is used to determine whether two objects are identical or not.
  
* **HashSet:-**
* Unordered and Unsorted .
* Uses the hashcode of the object to insert the values.
* use this when the requirement is "no duplicates and don't care about the order".
* It does not follow any insertion order. Duplicates are not allowed.
  
  ![image](https://github.com/user-attachments/assets/bc6fc37a-173e-430c-ad87-85b0142ff52f)

* **Linked HashSet**
* An ordered version of the hash set is known as linked hash set.
* Maintains a doubly linked list of all the elements.
* Use linked hash set when an iteration order is required.
* It maintains the insertion order in which they have been added to set. Duplicates are not allowed.
  
  ![image](https://github.com/user-attachments/assets/10c2ed54-060a-4905-becb-20255212dc45)

* **TreeSet**
* It is one of two sorted collections.
* Uses the 'Read-Black' tree structure and guarantees that the elements will be in ascending order.
* we can construct a tree set with the constructor by using a comparable or comparator.
* TreeSet sorts the elements in ascending order and duplicates are not allowed.
  
  ![image](https://github.com/user-attachments/assets/f9de95f7-ee31-46c5-9f42-ad665e9e6aea)
 
### 26. Explain about Map and its types.
* Map cares about the unique identifier. we can map a unique key to a specific value. It is key-value pair. We can search a value based on the key. Like the set,  the map also uses the 'equals()' method to determine whether two keys are the same or different.
  
* **HashMap**
* unordered and unsorted map.
* HashMap is a good choice  when we don't care about the order.
* It allows one null key and multiple null values.
* Duplicate keys are not allowed.
* It does not maintain any insertion order and is unsorted.
  
  ![image](https://github.com/user-attachments/assets/d82f68c7-df3e-4435-9e9a-082cf8ece731)

* **HashTable**
* Like the vector key, methods of class are synchronised.
* Thread safety and therefore slows the performance.
* It does not allow anything that is null.
* Duplicate keys are not allowed.
  
  ![image](https://github.com/user-attachments/assets/6ca1ead4-0d3c-410c-8f58-838ae73beea3)

* **Linked HashMap**
* Maintain insertion order and slower than hashmap.
* Faster iteration.
* Duplicate keys are not allowed.

  ![image](https://github.com/user-attachments/assets/14fe17b9-cdb2-4d02-ae40-63b1a153b7fe)

* **TreeMap**
* Sorted Map
* Like TreeSet, we can construct a sort order with constructor.
* It is sorted in ascending order based on the key.
* Duplicate keys are not allowed.
  
  ![image](https://github.com/user-attachments/assets/2043dc54-6dca-4759-994a-91fb0e802c19)
  
### 27. Explain the priority Queue. 
 * **Priority Queue:** Linked list has been enhanced to implement the Queue Interface. Queues can be handled with a linked list.The purpose of queue is "Priority-in", priority-out". Hence, elements are ordered either naturally or according to the comparator. The elements ordering represents their relative priority.

 ### 28. Types of Execption
 * **Checked Execption:** These exceptions are checked by the compiler at the time of compilation. Classes that extend Throwable class except runtime execption and error are called checked exception. Checked exception must either declare the exception using throws keyword or surrounded by appropriate try/catch. E.G ClassNotFoundException
 * **Unchecked Exception:** These execptions are not checked during thr compile time by the compiler. The compiler does not force to handle these exceptions which includes . 1) Arithmetic Exception  2) ArrayIndexOutOfBounds Exception

### 29. What are different ways to handle exception ?
* **Using try/Catch:**
* The risky code is surrounded by try block. If an exception occurs then it is caught by catch block which is followed by try block.
  
  ![image](https://github.com/user-attachments/assets/1c25f444-66da-45b3-ac24-3090eae90cac)
  
* **By declaring throws keyword:**
* At the end of the method, we can declare the exception using throws keyword.
  
  ![image](https://github.com/user-attachments/assets/badee970-83c4-4dc0-85a2-06251edb62dc)
  
### 30. What is Thread.
* In Java, the flow of execution is called Thread. Every java program has at least one thread called the main thread, the main thread is created by JVM. The user can define their own threads by extending the Thread Class or implementing the runnable interface. Threads are executed concurrently.
  
  ![image](https://github.com/user-attachments/assets/859e90ef-13a0-4ab5-83b5-12ed2e148689)

### 31. How do you make a thread in java?
 * **Extend Thread class:**
 * Extending a thread class and override the run method. The thread is available in java.lang.thread.
 * The disadvantage of using a thread class is that we can not extend any other classes because we have already extended the thread class. we can overload the run() method in our class.
 * **Implement Runnable Interface:**
 * Another way is by implementing the runnable interface. For that, We should provide the implementation for run() method which is defined in the interface.
   
   ![image](https://github.com/user-attachments/assets/306b41ea-ac1f-45fb-a7a2-f1f568b1022f)

 ### 32. Explain about join() method.
 * Join method() is used to join one thread with the end of the currently running thread.
   
   ![image](https://github.com/user-attachments/assets/225d0271-1af3-4210-97e5-4e741f3e5379)
   
 * Based on the above code, the main method has started the execution. When it reaches the code t.start() then 'thread t' starts the own stacks for the execution. JVM Switches b/w the main thread and ' thread t'.
 * Once it reaches the code t.join() then 'thread t' alone is executed and completes its task then only the main thread start the execution.
 * It is non-static method . The join() method has an overloaded version. So we can mention the time duration in join() method also ".s".

 ### 33. What does the yield method of the Thread class do?
 * A yield() method moves the currently running thread to a runnable state and allows the other thread for execution so that equal priority threads have a chance to run. It is a static method. It doesn't release any lock. Yield() method moves the thread back to the runnable state only and the thread to sleep(), wait() or block.
   
   ![image](https://github.com/user-attachments/assets/b9602de6-ff2a-4030-9ad5-48cb01fc5949)
   
### 34. Explain abour wait() method.
 * wait() method used to make the thread to wait in the waiting pool. When the wait() method is executed during a thread execution thne immediately the thread gives up the lock on the object and goes to the waiting pool. Wait() method tells the thread to wait for a given amount of time. Then the thread will wake up after notify() or notify All()  method is called.
   Wait() method and the other above mentioned methods do not give lock on the object immediately until the currently executing thread completes the synchronized code. It is mostly used in synchronization.
   
   ![image](https://github.com/user-attachments/assets/4e9f75cc-d9ca-4621-ae80-ea3b126abd76)
   
### 35. Notify v/s Notify All()
   | Notify | Notify All |
   |:-------|:-----------|
   |This method is used to send a signal to wake up a single thread in the waiting pool. | This method sends a signal to wake up all the threads in the waiting pool.|
### 36. How to stop a thread in java ? Explain about sleep() method in a thread?
 * We can stop a thread by using below folloiwing thread method.
 * Sleeping
 * Waiting
 * Blocked
 * **Sleeping:** Sleep() method is used to sleep the currently executing thread for the given amount of time. Once the thread is wake up it can move to the runnable state so sleep() method is used to delay the execution for some period.
 * It is static method.
   
  ![image](https://github.com/user-attachments/assets/2cda8655-8bd5-4cbf-b26f-02fcb34ab44e)
  
### 37. When to use Runnable interface v/s Thread class in java?
 * If we need our class to extend some other classes other than the thread then we can go with the runnable interface because in java we can extend only one class.
 * If we are not going to extend any class then we can extend the thread class.

### 38. Start() v/s Run() method of thread class.
 * Start method creates a new thread and code inside the run() method is executed in the new thread. If we directly called the run() method then a new thread is not created and the currently executing thread will continue to execute the run() method.

### 39. What is multithreading.
 * Multithreads are executed simultaneously. Each thread starts its own stack based on the flow or priority of the threads.
   
    ![image](https://github.com/user-attachments/assets/bd9b7514-d739-47cc-9836-f69745c0d647)
   
* Once the execution reaches , t.start() line then a new thread is created and the new stack for the thread is also created. Now, JVM switches to the new thread and the main thread are back to the runnable state.
  
   ![image](https://github.com/user-attachments/assets/a6c7a896-81b7-4452-ad4a-c364854aee0c)
  
* Once the run method has completed then JVM switches back to the main thread and the user thread has completed the task and stack was disapeared. JVM switches b/w each thread until both the threads are completed. This is called Multi-Threading.

### 40. Explain the thread life cycle in Java.
* Explain the thread life cycle in Java:
* New
* Runnable
* Running
* Non-Runnable(Blocked)
* Terminated
  
  ![image](https://github.com/user-attachments/assets/116b9c01-582f-4d45-91d9-0fde8772a2f3)
  
* **New:**  In New state, a Thread instance has been created but start () method is not yet invoked. Now the thread is not considered alive.
* **Runnable:** The Thread is in the runnable state after the invocation of the start () method, but before the run () method is invoked. But a thread can also return to the runnable state from waiting/sleeping. In this state, the thread is considered alive.
* **Ruuning:** The thread is in a running state after it calls the run () method. Now the thread begins the execution.
* **Non-Runnable:** The thread is alive but it is not eligible to run. It is not in the runnable state but also, it will return to the runnable state after some time. Example: wait, sleep, block.
* **Terminated:** Once the run method is completed then it is terminated. Now the thread is not alive.

### 41: What is synchronization?
* Synchronization makes only one thread to access a block of code at a time. If multiple threads accesses the block of code, then there is a chance for inaccurate results at the end. To avoid this issue, we can provide synchronization for the sensitive block of codes.
* The synchronized keyword means that a thread needs a key in order to access the synchronized code.
* Locks are per objects. Every Java object has a lock. A lock has only one key. A thread can access a synchronized method only if the thread can get the key to the objects to lock.
* For this, we use the “Synchronized” keyword.
  ![image](https://github.com/user-attachments/assets/c0a77c51-18cc-45f2-9098-80ab726342d5)
  
### 42. What is meant by Serialization?
* Converting a file into a byte stream is known as Serialization. The objects in the file are converted to bytes for security purposes. For this, we need to implement a java.io.Serializable interface. It has no method to define.
* Variables that are marked as transient will not be a part of the serialization. So we can skip the serialization for the variables in the file by using a transient keyword.

### 43. What is the purpose of a transient variable?
* Transient variables are not part of the serialization process. During deserialization, the values of the transient variables are set to the default value. It is not used with static variables.

### 44. Which methods are used during the Serialization and Deserialization process?
* ObjectOutputStream and ObjectInputStream classes are higher level java.io. package. We will use them with lower level classes FileOutputStream and FileInputStream.
* ObjectOutputStream.writeObject —->Serialize the object and write the serialized object to a file.
* ObjectInputStream.readObject —> Reads the file and deserializes the object.
* To be serialized, an object must implement the serializable interface. If superclass implements Serializable, then the subclass will automatically be serializable.

### 45. What is the purpose of a Volatile Variable?
* Volatile variable values are always read from the main memory and not from thread’s cache memory. This is used mainly during synchronization. It is applicable only for variables. E.G volatile int number;
### 46. Serialization v/s Deserialization
  |Serialization | Deserialization|
  |:-------------|:--------------|
  |Serialization is the process which is used to convert the objects into byte stream | Deserialization is the opposite process of serialization where we can get the objects back from the byte stream.|
  | An object is serialized by writing it an ObjectOutputStream. | An object is deserialized by reading it from an ObjectInputStream. |

### 47. What is SerialVersionUID?
 * Whenever an object is Serialized, the object is stamped with a version ID number for the object class. This ID is called the  SerialVersionUID. This is used during deserialization to verify that the sender and receiver that are compatible with the Serialization.




