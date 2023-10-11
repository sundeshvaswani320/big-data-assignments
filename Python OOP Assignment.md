Q1. What is the purpose of Python's OOP?

answer:
OOPs approach is defining attributes and their functionality as a single unit called class. It serves as a blueprint for all objects having similar attributes and behavior.

Q2. Where does an inheritance search look for an attribute?

answer:
Inheritance search is used to allow objects to inherit attributes and methods from their parent classes.This allows for code reuse and makes it easier to create and maintain large software systems.

Q3. How do you distinguish between a class object and an instance object?

answer:
A class object represents the blueprint or template for creating instance objects
An instance object is an individual object created from a class. It is an instantiation of the class.
eg :
class car:
pass

c1 = car()
car is class object and c1 is a instance object

Q4. What makes the first argument in a class’s method function special

answer:
This is known as the `self` parameter.The `self` parameter is used to access the attributes and methods of the instance object.

Q5. What is the purpose of the init method?

answer:
init method is a constructor. when you create an instance of the class , the  __init__ method is automatically called , allowing you to intialize the object's attributed or peform any setup

Q6. What is the process for creating a class instance?

answer
creating a class instance involves defining a class, then using that class to create objects by calling it with parentheses, and finally, you can access the object's attributes and methods using dot notation.


Q7. What is the process for creating a class?

answer:
1. use keyword class to define it with a name of class.
2. define attributes of class car. 
3. define the  constructor __init__ .
4. define the member function of the class.
5. make an instance of the class.
6. access the class attributes and methods.

code example:
class car:
    wheel =4
    def __init__(self, model, name):
        self.model = model
        self.name = name
    
    def show(self):
        print(f"car name is {self.name} and model is {self.model}")
        
p1 = car("2019", "seltos")
p1.show()

Q8. How would you define the superclasses of a class?

answer:
The superclass is a class from which other classes inherit properties. It's sometimes called a parent class or a base class. 


Q9. What is the relationship between classes and modules?

answer:
classes are used for creating objects with specific behaviors and attributes, while modules are used for organizing and encapsulating related code. Classes define objects, while modules provide a way to structure the overall program.


Q10. How do you make instances and classes?

answer
class car #(name of the class defining it.)
    
    pass #defining some attributes and method in class
   
p1 = car() # making an instance of the class car 
p1.name #eg then accessing the attributes and methods of the class

Q11. Where and how should be class attributes created?

answer
class attributes are created in the class but outside the any method or __init__ method 
class MyClass:
    class_attribute1 = "This is a class attribute"
    class_attribute2 = 42


Q12. Where and how are instance attributes created?

answer:
it is created when we make a class object and pass the values of the attributes

class car:

   def __init__(self ,name,model):
        name  =  self.name
        model = self.model
        
p1 = car("seltos","2019") # this is how instance attributes are created
p1.name


Q13. What does the term "self" in a Python class mean?

answer:
Self represents the instance of the class. By using the self  we can access the attributes and methods of the class in Python.
self is not a keyword we can use any other name instead of that.


Q14. How does a Python class handle operator overloading?


Q15. When do you consider allowing operator overloading of your classes?

answer:
operator overloading can be a valuable tool for making your code more expressive and readable, especially in specific scenarios where the operations have clear and intuitive meanings


Q16. What is the most popular form of operator overloading?

answer
most popular form operator overloading are arthimetic operator overloading like -,%,*,+ etc.


Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?

answer:
1.inheritnace
2.classes and objects.

Q18. Describe three applications for exception processing.

answer:
1. fault tolerant
2. error handling
3. resource management


Q19. What happens if you don't do something extra to treat an exception?

answer:
If you don't handle an exception in your code, and it is not caught by any try...except block, the program will terminate, and an error message will be displayed. This error message provides information about the type of exception

Q20. What are your options for recovering from an exception in your script?

answer:
1.try/ except block
2. raise exception
3. logging


Q21. Describe two methods for triggering exceptions in your script.

answer:
1.raise statement
2. assert statement.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of
whether or not an exception exists.

answer:
1. finally block
2.  defer statment

Q23. What is the purpose of the try statement?

answer
purpose of try block is if we have some suspicious code we can try that if it works in the try block without getting a error and if it works we will not get eny error if the code is not working we can define a except block to handle a error without getting an error this helps in not breaking our code

Q24. What are the two most popular try statement variations?

answer
1.try and except block 
2. try and finally block

Q25. What is the purpose of the raise statement?


answer:
raise statement purpose isto improve the ability to handle the challenges of your programs and make them more reliable by handling errors and exceptions gracefully.


Q26. What does the assert statement do, and what other statement is it like?


answer:
The assert statement in programming is used as a debugging aid that tests a condition, and triggers an error if the condition is not true.
it is similar to the if - else statement.


Q27. What is the purpose of the with/as argument, and what other statement is it like?

answer:
The purpose of the with/as statement is to ensure that certain operations are properly set up and cleaned up.
even if an exception occurs within the block of code.
it is similar to try/finally block

Q28. What are *args, **kwargs?

answer
*args is a Arbitrary argument which we define  as parameter when defining a function. it is used to take n number of arguments as input
**args is also a arbitrary argument which we define as parameter in the function. it is used for take n number of arguments as in input but only in key:value pair  like a dictionary

Q29. How can I pass optional or keyword parameters from one function to another?

answer
we can use the *args and **kwargs syntax to pass optional and keyword parameters from one function to another.

Q30. What are Lambda Functions?

answer                                                                  
we can use python's lambda functions, which are inline functions defined at the same place we use it. So we don't need to declare a function somewhere and revisit the code just for a single time use.



Q31. Explain Inheritance in Python with an example?
inheritance is  mainly of 3 types 
1. simple
2. multiple
3. multi - level

eg: 
class car:

    def __init__(self, name,model):
        self.name  = name 
        self.model =  model 
     
    def details(self):
        print(f"name of the car is {self.name} and model of car is {self.model}")
        
class car2(car):  # we are inheriting the method and attributes of the car(parent) class into child class(car2)

    pass
    
    
p1  =  car2("nissan" , "1980")  # making an object if the car2 class and calling it .
p1.details()
    


Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?

answer:
class A will get invoked

Q33. Which methods/functions do we use to determine the type of instance and inheritance?


answer:
1. type() -  function
2. isisntance() - function 
3. issubclass() - function

Q34.Explain the use of the 'nonlocal' keyword in Python.

answer
non local variables are used in nested functions whose local scope is not defined. this means the variable can neither be in local scope nor cna be in the global scope.

Q35. What is the global keyword?

answer:
variable which are defined outside any function are global varibles
eg:
a = 10 # this is a local variable
def funn():
    pass
    
fun()
    