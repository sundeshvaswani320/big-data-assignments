## Assignment Part-1
#Q1. Why do we call Python as a general purpose and high-level programming language?

#answer 
"""python is general purpose language because it can be applied a wide range of tasks and domains . its high level nature is characterized by its abstraction from low level details and its emphasis on code readability and developer productivity"""



#Q2. Why is Python called a dynamically typed language?

#answer
"""python is called dynamically typed language because it allows varibales to change their data type during the run time and also in python we dont have to specify the datatypes while declaring the variable """


#Q3. List some pros and cons of Python programming language?

#answer
""" pros  =1 . very easy to learn and use.
2. large support of libraries
3.cross- platform connections 
4. large community and ecosystem
cons = 1.not used in web development 
2. design limitations
3.performance - it can be slower than compiled language like c++ , java 
"""

#Q4. In what all domains can we use Python?

#answer
"""machine learning and data science , scientific computation, automation and scripting , game deveolpment """

Q5. What are variable and how can we declare them?
a = 23

Q6 How can we take an input from the user in Python?
#by using input function 

a = input() 
b = int(input())  # -  if we want to take integer as an input

#Q7. What is the default datatype of the value that has been taken as an input using input() function? 

#answer
a string

#Q8.What is type casting?

answer
type casting is changing a datatype of a variable


#Q9Can we take more than one input from the user using single input() function? If yes, how? If no, why?

answer
# - yes we can take more than 1 input in input function
#example
a,b  = input().split(",")
print(a,b)

#Q10. What are keywords?

#anwser
keyword are pre - defined function or word that can't be used as varibale names


Q11. Can we use keywords as a variable? Support your answer with reason.

answer
yes ,but we shoudn't as it will override the properties of the keyword.


Q12. What is indentation? What's the use of indentaion in Python?

answer
indentation are the spaces in code.used to create a block of statment.


#Q13. How can we throw some output in Python?

answer
by using print() -function or return function

#Q14. What are operators in Python?

answer
keywords used to perform certain operations on values or variable are known as operators.

#Q15. What is difference between / and // operators?

answer
/ -  is a float division operator
//- is a int division operator

#Q16. Write a code that gives following as an output.

answer
a = "ineuron"
a = a*4
print(a)

#Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

answer
num = int(input())
if num % 2 == 0:
    print("even number")
else:
    print("odd numbder")

#Q18. What are boolean operator?

answer
boolean operator have only 2 values example - True or False 
,1 or 0 and YES or NO

Q19. What will the output of the following?

answer
1. 1
2. 0
3. False
4. 1

#Q20. What are conditional statements in Python?

answer
conditional statements - if , elif, else used for conditional filtering

#Q21. What is use of 'if', 'elif' and 'else' keywords?

answer
use of if - it the first condition to check the condition is true or not if its true it will stop there only and if it is false then it goes to elif condition if elif is false then it goes to else condition which is the last condition.


#Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

answer
age = int(input())
if age >= 18 :
    print("I can vote")
else:
    print("I can't vote")


#Q23. Write a code that displays the sum of all the even numbers from the given list.


answer
numbers = [12, 75, 150, 180, 145, 525, 50]
l = 0
for i in numbers:
    if i % 2 == 0:
        l = l+i
    else:
        continue
print(l)


#Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

answer
x,y,z = input("enter your 3 numbers").split(',')
max(x,y,z)

#Q25. Write a program to display only those numbers from a list that satisfy the following conditions


answer
numbers = [12, 75, 150, 180, 145, 525, 50]
lst = []
for i in numbers:
  if i > 150:
    if i > 500:
      break
  elif i%5==0:
    lst.append(i) 

print(lst)