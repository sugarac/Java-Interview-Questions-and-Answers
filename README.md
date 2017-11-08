## Java Interview Questions and Answers
### Object-Oriented Programming
* What are the main 3 Object Oriented Programing (OOP) concepts?
* Explain object serialization and how to implement it in Java.
* Explain anonymous classes. 
* Describe the differences between abstract classes and interfaces. 
* Explain what a Singleton class is and how to create one in Java 
* Why should the equals() and hashCode() methods often be overridden together? 
* How do you properly override the equals() method? For example, what considerations should be taken when checking for equality?
* Difference between final, finally and finalize?
* In Java, does the finally block gets executed if we insert a return statement inside the try block of a try-catch-finally?
* Explain method overloading & overriding. 
* What is memory leak and how does Java handle it?

Topics:
<a href="#static">static</a>,
<a href="#final">final</a>,
<a href="#overload">Overload</a>,
<a href="#inheritance">Inheritance</a>,
<a href="#abstraction">Abstraction</a>,
<a href="#interface">Interface</a>,
<a href="#interesting">Interesting</a>,

### Constructor
* What is constructor?
> Constructor is just like a method that is used to initialize the state of an object. It is invoked at the time of object creation.
* What is the purpose of default constructor?
> The default constructor provides the default values to the objects. The java compiler creates a default constructor only if there is no constructor in the class.
* Does constructor return any value?
> Yes, that is current instance (You cannot use return type yet it returns a value).
* Is constructor inherited?
> No, constructor is not inherited.
* Can you make a constructor final?
> No, constructor can't be final.

### static
* What is static variable?
> static variable is used to refer the common property of all objects (that is not unique for each object) e.g. company name of employees,college name of students etc. <br />
static variable gets memory only once in class area at the time of class loading.

* What is static method?
> static method belongs to the class rather than object of a class. <br />
static method can be invoked without the need for creating an instance of a class. <br />
static method can access static data member and can change the value of it. <br />

* Why main method is static?
> because object is not required to call static method if It were non-static method,jvm creats object first then call main() method that will lead to the problem of extra memory allocation.

* What is static block?
> It is used to initialize the static data member. <br />
It is excuted before main method at the time of classloading. <br />

### final
* What is final variable? What is final method? What is final class?
> The value of final variable can't be changed. Final methods can't be overriden. Final class can't be inherited.
* Can you declare the main method as final?
> Yes, such as, public static final void main(String[] args){}.

### Overload
* What is method overloading?
> If a class have multiple methods by same name but different parameters, it is known as Method Overloading. It increases the readability of the program.
* Why method overloading is not possible by changing the return type in java?
> Becauseof ambiguity.
* Can we overload main() method?
> Yes, You can have many main() methods in a class by overloading the main method.

### Override
* What is method overriding?
> If a subclass provides a specific implementation of a method that is already provided by its parent class, it is known as Method Overriding. It is used for runtime polymorphism and to provide the specific implementation of the method.
* Can we override static method? Why?
> No. It is because the static method is the part of class and it is bound with class whereas instance method is bound with object and static gets memory in class area and instance gets memory in heap.
Difference between method Overloading and Overriding.
* Difference between method Overloading and Overriding.
> 1) Method overloading increases the readability of the program.	Method overriding provides the specific implementation of the method that is already provided by its super class.
> 2) Method overloading is occurs within the class.	Method overriding occurs in two classes that have IS-A relationship.
> 3) In this case, parameter must be different.	In this case, parameter must be same.

### Inheritance
* What is this in java?
> It is a keyword that that refers to the current object.
* What is super in java?
> It is a keyword that refers to the immediate parent class object.
* Can you use this() and super() both in a constructor?
> No. Because super() or this() must be the first statement.
* What is Inheritance?
> Inheritance is a mechanism in which one object acquires all the properties and behaviour of another object of another class. It represents IS-A relationship. It is used for Code Resusability and Method Overriding.
* What is composition?
> Holding the reference of the other class within some other class is known as composition.

### Abstraction
* What is abstraction?
> Abstraction is a process of hiding the implementation details and showing only functionality to the user.
Abstraction lets you focus on what the object does instead of how it does it.
* What is the difference between abstraction and encapsulation?
> Abstraction hides the implementation details whereas encapsulation wraps code and data into a single unit.
* What is abstract class?
> A class that is declared as abstract is known as abstract class. It needs to be extended and its method implemented. It cannot be instantiated.

* Can there be any abstract method without abstract class?
> No, if there is any abstract method in a class, that class must be abstract.

* Can you use abstract and final both with a method?
No, because abstract method needs to be overridden whereas you can't override final method.

* Is it possible to instantiate the abstract class?
No, abstract class can never be instantiated.

### Interface
* What is interface?
> Interface is a blueprint of a class that have static constants and abstract methods.It can be used to achieve fully abstraction and multiple inheritance.

* Can you declare an interface method static?
> No, because methods of an interface is abstract by default, and static and abstract keywords can't be used together.

* Can an Interface be final?
> No, because its implementation is provided by another class.

* What is marker interface?
> An interface that have no data member and method is known as a marker interface.For example Serializable, Cloneable etc.

* What is difference between abstract class and interface?
> 1) An abstract class can have method body (non-abstract methods).	Interface have only abstract methods.
> 2) An abstract class can have instance variables.	An interface cannot have instance variables.
> 3) An abstract class can have constructor.	Interface cannot have constructor.
> 4) An abstract class can have static methods.	Interface cannot have static methods.
> 5) You can extends one abstract class.	You can implement multiple interfaces.
* Can we define private and protected modifiers for variables in interfaces?
> No, they are implicitly public.

* When can an object reference be cast to an interface reference?
> An object reference can be cast to an interface reference when the object implements the referenced interface.

### Interesting
* What is the default value of the local variables?
> The local variables are not initialized to any default value, neither primitives nor object references.
