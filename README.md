# Notes-for-8-9-10

Chapter 8 Notes:

An Interface is a 100% abstract class
An abstract class is a class that can't be instantiated
A concrete class is one that can be instantiated
Abstract classes value only happens when it is extended
Methods can also be abstract
Abstract methods have no body
Abstract methods need to be in a abstract class
Must implement all abstract methods when extending
Class object extends everything
Class object contains: equals(), hashCode(), getClass(), toString()
Avoid using object as ultra-flexible argument as it will return objects as object
Polymorphism gives us the freedom to use EVERYTHING a class inherited 
Even if an object is returned more generic, you can cast it back to it's real type to use it's specific methods/ vars
Two superclasses is called "multiple inheritance" and it can be bad and should be avoided over possible confusion over methods and variables and arise
Interfaces can solve any possible multiple inheritance issues
Classes can implement the same interface despite any differences 
Classes can implement multiple interfaces
Can use super methods in a subclasses methods by calling super.nameOfMethodInParent

Chapter 9 Notes:

Objects take memory and at a certain point you will need to destroy them to save memory
The stack refers to where all method invocations and local vairables are stored
The heap is where all objects are stored
Instance variables live on the object inside the heap
Constructors have similar syntax to methods w/o a return type
Can use and overload constructors to pass in variables to the object
Compiler will only make a no-arg constructor if you didn't make any constructors in the class
When you make an object you still use all the constructors in your parent classes
super() calls and users the constructors that you inherited, the compiler will put one in if you don't
Calling the super() must be the first statement as the child can't exist before the parents
Can use super() to pass arguments to the parent's constructors
CANNOT use this() and super() in the same constructor
Local variables are alive until the method their contained in, is completed
Once objects become unreachable they'll eventually be deleted
If an object is used in a method, once the method is completed it will delete the object
Instance variables support an object throughout it's entire life and is stored with the heap
Excpetions are if the instance variables are nulled out or gets a new instance variable

Chapter 10 Notes:

Math is a almost global method which doesn't need you to make a new instance of to use.
The static keyword lets a method run without any instance of the class (Ex: math)
You can mark a constructor private to ensure no one can create an isntance of it and only use static methods
Static methods can't use instance variables
Static methods can't use non-static methods either
Static vairable value is the same for all instances of the class, they are shared
Intialize static variable first and by using the static keyword before the data type
Static final variables are constants and cannot be changed
You can use the final keyword for non-static and local variables as well as method parameters, methods and class.
Some math methods are math.random() which returns a double betwen 0.0 and 1.0 (multiply to make larger)
math.abs() which returns the absolute value in a double
math.round() which returns and int or a long to the nearest integer value
math.min() which returns the lower value
math.max() which returns the higher value
Wrap primitive data types if you're using in a object or collection
Wrapper classes and the same as the primitive types except the first letter is uppercase
The exceptions are that int and char and fully spelled out
The syntax to wrap a value is: (Wrapper name) (Variable name) = new (Wrapper name)((primtive data))
To unwrap a value: (primitive data type) (name) = (variable name).(primitivedatatype)Value();
In newer versions of java you aren't forced to use wrapper classes in collections
Wrapper have statuc utillity methods such as
parse(Datatype) which automatically converts to other datatypes when applicable
String.format can be used to format an example w/ commas is
String s = String.format("%, d", 100000000); prints out 1,000,000,000
                       Do this     to this
Take the second argument to this method, and format it as a decimal integer and insert commas
Perecent sign means to insert argument here
Some important syntax to know:
%, d means "Insert commas and format the number as a decimal integer
%.2f means format the number with a precision of two decimal places
%,.2f means insert commas and format as decimal integer with two decimal places
Can have as many arguments as you like
Can use %tc which means date and time
Can use %tr which means just the time
Can use %tA %tB %td to mean day of the week, month and day






