# Python_Basics
variables, types ,opperators and control flow (conditional)
# Creating Variables
Unlike other programming languages, Python has no command for declaring a variable.               
•	A variable is created the moment you first assign a value to it.
#### Example
```
x = 5
y = "John"
print(x)
print(y) 
Output 5 
Output Jhon	
```
•	Variables do not need to be declared with any particular type and can even change type after they have been set.
```
Example
x = 4 # x is of type int
x = "Sally" # x is now of type str
print(x) 
output SallySallySallySally
```
## Variable Names
A variable can have a short name (like x and y) or a more descriptive name (age, carname, total volume). Rules for Python variables:        
•	A variable name must start with a letter or the underscore character             
•	A variable name cannot start with a number              
•	A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )              
•	Variable names are case-sensitive (age, Age and AGE are three different variables)           
Remember that variables are case-sensitive
Output Variables
The Python print statement is often used to output variables.
To combine both text and a variable, Python uses the + character:
#### Example
```
x = "awesome"
print("Python is " + x)
```
•	You can also use the + character to add a variable to another variable:
#### Example
```
x = "Python is "
y = "awesome"
z =  x + y
print(z)
output Python is awesome
```
•	For numbers, the + character works as a mathematical operator:
#### Example
```
x = 5
y = 10
print(x + y) 
output  15
```
•	If you try to combine a string and a number, Python will give you an error:
#### Example
```
x = 5
y = "John"
print(x + y) 
output     Error
```
# Data Types
There are different types of python data types. Some built-in python data types are:
Python Data Type 
## 1.	Numeric
Python numeric data type is used to hold numeric values like;
1.	int – holds signed integers of non-limited length.
2.	long- holds long integers(exists in Python 2.x, deprecated in Python 3.x). 
3.	float- holds floating precision numbers and it’s accurate upto 15 decimal places.
4.	complex- holds complex numbers.
In Python we need not to declare datatype while declaring a variable like C or C++. We can simply just assign values in a variable. But if we want to see what type of numerical value is it holding right now, we can use type(), like this:
#### Example
```
create a variable with integer value
a = 100
print(“The type of variable having value”, a, “is”, type(a))
 create a variable with float value
b = 10.896
print(“The type of variable having value”, b, “is”, type(b))
create a variable with integer value
c = 23+2J
print(“The type of variable having value”, c, “is”, type(c))
```
## 2. String
String is a sequence of characters. Python supports unicode characters. Generally strings are represented by either single or double quotes.
#### Example
```
A = ”string in double quote”
B = ‘string in single quote’
Print(A)
Print(B)
Using ‘,’ to concate the two or several strings.
Print(A,”concated with “,B)
Using ‘+’ to concate the two or several strings
Print(A+,”concated with “,+B)
```
## 3.List
List is a versatile data type exclusive in Python. In a sense it is same as array in C/C++. But interesting thing about list in Python is it can simultaneously hold different type of data. Formally list a ordered sequence of some data written using square brackets  ([]) and commas(,).
#### Example
```
List of having only integers 
A=[1,2,3,4,5,6]
Print(A)
List of having only strings
B=[“hello”,”john”]
Print(B)
List of having both integers and strings 
C=[“hey”,”you”,”1,2,3”,”go”]
Print(C)
```
## 4.Tuple
Tuple is another data type which is a sequence of data similar to list. But it is immutable. That means data in a tuple is write protected. Data in a tuple is written using parenthesis and commas.
##### Example
```
Tuple having only integer type of data.
A= (1,2,3,4)
Print(A)
Tuple having multiple type of data.
B=(“hello” , 1,2,3,”go”)
Print(B)
Prints whole tuple index of tuple are also 0 based.
Print(b[4]) this will prints a single element in a tuple , in this case “go”.
```
# Python Operators
Operators are used to perform operations on variables and values.
Python divides the operators in the following groups:
•	Arithmetic operators
•	Assignment operators
•	Comparison operators
•	Logical operators
•	Identity operators
•	Membership operators
•	Bitwise operators
## Arithmetic Operators
Arithmetic operators are used with numeric values to perform common mathematical operations:
Operator	Name	Example	
```
+	Addition	x + y	
-	Subtraction	x - y	
*	Multiplication	x * y	
/	Division	x / y	
%	Modulus	x % y	
**	Exponentiation	x ** y	 
//	Floor division	x // y	 
```
Assignment operators are used to assign values to variables:
Operator	Example	Same As
```
=	x = 5	x = 5	
+=	x += 3	x = x + 3	
-=	x -= 3	x = x - 3	
*=	x *= 3	x = x * 3	
/=	x /= 3	x = x / 3	
%=	x %= 3	x = x % 3	
//=	x //= 3	x = x // 3	
**=	x **= 3	x = x ** 3	
&=	x &= 3	x = x & 3	
|=	x |= 3	x = x | 3	
^=	x ^= 3	x = x ^ 3	
>>=	x >>= 3	x = x >> 3	
<<=	x <<= 3	x = x << 3	
```
## Comparison Operators
Comparison operators are used to compare two values:
Operator	Name	Example	
```
==	Equal	x == y	
!=	Not equal	x != y	
>	Greater than	x > y	
<	Less than	x < y	
>=	Greater than or equal to	x >= y	
<=	Less than or equal to	x <= y
```
## Logical Operators
Logical operators are used to combine conditional statements:
Operator	Description	Example	
```
and 	Returns True if both statements are true	x < 5 and  x < 10	
or	Returns True if one of the statements is true	x < 5 or x < 4	
not	Reverse the result, returns False if the result is true	not(x < 5 and x < 10)
```
## Identity Operators
Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object, with the same memory location:
Operator	Description	Example	
```
is 	Returns true if both variables are the same object	x is y	
is not	Returns true if both variables are not the same object	x is not y	
```
#### Bitwise Operators
Bitwise operators are used to compare (binary) numbers:
Operator	Name	Description
```
& 	AND	Sets each bit to 1 if both bits are 1
|	OR	Sets each bit to 1 if one of two bits is 1
 ^	XOR	Sets each bit to 1 if only one of two bits is 1
~ 	NOT	Inverts all the bits
<<	Zero fill left shift	Shift left by pushing zeros in from the right and let the leftmost bits fall off
>>	Signed right shift	Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off
```
