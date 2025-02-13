**I.Functions in Python**

    A function is a block of reusable code that performs a specific task. Functions avoids redundancy.
    Syntax:
      def  function_name( ):
          #block of code
    function_name()              #calling the function

  **Types of Functions in Python:**

      1.Built-in Functions: -They are predefined functions.eg:- print(), len(), sum(), etc.
      2.User-Defined Functions:- Functions created by the user using the def keyword.


**II.Local and Global Scope of  Variables**

    1.Local Variable:
       They are variables defined inside a function and only accessible within that function.It cannot be used outside 
       the function.
  
    2.Global Variable:
       These are variables defined outside a function and can be accessed anywhere in the program.Can be modified inside 
       a function using the global keyword.

**III.Type of Arguments in Python Function**

    1.Default Arguments: Arguments can have default values.
      Example: def greet(name,"message=Good Morning"):
                   print(message+"name")
               greet("Sam")
               Output: Good Morning Sam
              
    2.Positional Arguments: Values are assigned based on their position(in correct order).
      Example:def details(name,age):
                 print("My Name is "+name+"I am "+age+" years old")
                 
            details("Sam",37)                     # correct order
            details(37,"Sam")                     # incorrect order

    3.Keyword Arguments: Keyword arguments (kwargs) are function parameters that are passed with a name (key) 
                        and a value.Here position of the argument doesn't matter.
     Example:def details(name,age):
                 print("My Name is "+name+"I am "+age+" years old")
                 
            details(name="Sam",age=37)                     # correct order
            details(age=37,name="Sam")                     # Incorrect order, but order doesn't matter in keyword argument
            
    4.Arbitrary Arguments:It can take any number of positional arguments.
      Example: def sum_of_no(*numbers):
                  print("Sum of nos is:",numbers)

              sum_of_no(2,3,4,5)
              
    5.Keyword Arbitrary Argument:Keyword Arbitrary Arguments (**kwargs) allow a function to accept any number of keyword arguments
    (named arguments). These arguments are stored as a dictionary where the keys are argument names and the values are their 
    corresponding values.
      Example:def details(**kwargs):
                 print(kwargs)

              details(name="sam",age=37,sex="Male")
     
