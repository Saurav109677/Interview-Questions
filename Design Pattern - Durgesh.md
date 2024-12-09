Creational Design Pattern (used for object creation)

1. Singleton Design Pattern 
2. How to break singleton pattern and solution
3. Factory Method Design Pattern -
  - AndroidDeveloper.java and WebDeveloper.java
  - DeveloperClient (main) need not to create or bother about how to get the object of the developer.
    simply create (EmployeeFactory.java). this includes the logic to pass the object of developer according to the type provide
     e.g EmployeeFactory.getEmployee("ANDROID DEVELOPER") / "WEB DEVELOPER". 
     DeveloperClient need not worry how to get the developer. (Loose coupling)
   Advantages - 
   - Focus on main logic rather on implementaino of the developers
   - loose coupled
4. Abstract Factory Design Pattern -
  - similar to factory method design pattern. Differnece in layer of abstraction.
    ![image](https://github.com/user-attachments/assets/fae8ab6a-e87c-43ad-b956-fac90ebefe6f)

5. Builder Pattern
  - while creating object, it takes many attributes in constructor in factory pattern
  - hard to remember the sequence of the attr
  - if any attr is optional, then overload constructor
  - complexity of factory pattern
  - >> This pattern creates object by setting the attribute in chain fashion and at last calls build() to create new object
6. Prototype Design Pattern
  -  The concept is to copy an existing object rathr than creating a new instance from scrath. because creating new object may be costly.
  - This approach saves costly resource and time, especially when object creation is a heavy process. e.g network or db connection.
7. Shallow Clone or Deep Clone
  - when we clone any object, it may have pritimive data types(int/float) or some object (Student.class)
  - When using shallow clone, the new object will have the reference fo the object (address of heap space) . i.e if the object field say name is changed then it will reflect in previous object as well
  - Deep copy means, clone the object - creating new reference in the heap memory in every cloned object.
8. Implement Deep Copy. >> Simply add your own logic in overrided clone() function.

Behavioural Design Pattern (deals with how one object interact with others)
1. Observer design pattern  (publish and subscribe pattern)
  e.g - subscribe in youtube channel and everyone gets the notificaiton when any new video uploaded
2. Iterator design patter 
  - provides a way to access or traverse the elements of object without knowing the undelying implementation. whethere it be list/ArrayList/Map/Set etc.
  - simply create ur own MyItertor interface with hasNext() and next() method , which will help you to iterate
  - there is a pre-defined Iterator interface , but not support for all. It supports List, Set but not Map.
  - You can iterate the keySet() or valueset in map, but not whole map.
3. Adapter Design pattern
  - to make compatible of two interface, we need in between adapter interface to support both.
  - e.g charge iphone with android charger, using an via adapter
  ![image](https://github.com/user-attachments/assets/d5bf73eb-a24f-429c-86a9-020e9049e739)






