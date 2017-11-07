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

Inheritance
* What is this in java?
It is a keyword that that refers to the current object.
* What is Inheritance?
> Inheritance is a mechanism in which one object acquires all the properties and behaviour of another object of another class. It represents IS-A relationship. It is used for Code Resusability and Method Overriding.
* What is composition?
> Holding the reference of the other class within some other class is known as composition.


### Interesting
* What is the default value of the local variables?
> The local variables are not initialized to any default value, neither primitives nor object references.
