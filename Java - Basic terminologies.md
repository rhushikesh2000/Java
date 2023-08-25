**Java - Basic terminologies**
----
When we consider a Java program, it can be defined as a collection of objects that communicate via invoking each other's methods. Let us now briefly look into what class, object, methods, and instance variables mean.

- **Class:** The class is a blueprint (plan) of the instance of a class (object). It can be defined as a logical template that shares common properties and methods.

Example 1: Blueprint of the house is class.


- **Object:**  Objects have states and behaviors. Example: A dog has states color, name, and breed as well as behavior such as wagging their tail, barking, and eating. An object is an instance of a class.

- **Methods:** A method is a behavior. A class can contain many methods. It is in methods where the logic are written, data is manipulated and all the actions are executed.


- **Instance Variables :** Each object has its unique set of instance variables. An object's state is created by the values assigned to these instance variables.

- **public static void main(String [] args):** The method main() is the main entry point into a Java program; this is where the processing starts. Also allowed is the signature 

**public static void main(String… args){ ..}**
~~~java
Public Class   class_name {

public static void main(String[] args)

  {

        System.out.println("welcome to GUVI");

    }


            }
~~~
**Output:**
~~~
welcome to GUVI
~~~
**Comments in Java**

---

There are three types of comments in Java. 

**Single line Comment**

---

~~~java
**//** System.out.println("This is an comment.");
~~~
**Multiline Comment**

---

~~~
/*

   System.out.println("This is the first line comment.");
    System.out.println("This is the second line comment.");

*/
~~~

**Identifiers in java :**

---
All Java components require names. Names used for classes, variables, and methods are called identifiers.

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 001](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/91f55133-9615-463d-8144-f23a42f315d5)

  

**Rules to write** **Identifiers :**

---

- All identifiers should begin with a letter (A to Z or a to z), currency character ($) or an underscore (\_).
- After the first character, identifiers can have any combination of characters.
- A key word cannot be used as an identifier.
- We can’t use space in between an identifier.
- Most importantly, identifiers are case sensitive.
- Examples of legal identifiers: age, $salary, \_value, \_\_1\_value.
- Examples of illegal identifiers: 123abc, -salary.



**Keywords in java :**

---

 Keywords are predefined, reserved words used in Java programming that have special meanings to the compiler. The following list shows the reserved words in Java. These reserved words may not be used as constant or variable or any other identifier names.

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 002](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/b8f8aa5a-797d-42eb-af42-bcc0bdd433fd)














**Operators In java :**

---

Operators in Java are the symbols used for performing specific operations in Java. Operators make tasks like addition, multiplication, etc. which look easy although the implementation of these tasks is quite complex.

**Types of Operators in Java :**

 
 

1. **Arithmetic Operators**
---
These operators involve the mathematical operators that can be used to perform various simple or advanced arithmetic operations on the primitive data types . 

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 009](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/b939f147-d8ce-4f2b-9376-a8353ed527b4)

2. **Unary Operators in Java**

---

Java unary operators are the types that need only one operand to perform any operation like increment, decrement, negation, etc.
![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 010](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/5ab0858d-253f-4154-bd5c-72d685bbbfd3)


3. **Assignment Operators**

---

These operators are used to assign values to a variable. The left side operand of the assignment operator is a variable, and the right side operand of the assignment operator is a value. 

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 011](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/8a716b30-274c-49f9-a082-994e40781b8b)




4. **Relational Operators**

---

Java Relational Operators are a bunch of binary operators used to check for relations between two operands, including equality, greater than, less than, etc. They return a boolean result .

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 012](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/e561afb6-f15b-42b1-bff6-67e7f231abad)

5. **Logical Operators**

---

Logical operators are used to performing logical “AND”, “OR” and “NOT” operations, i.e. the function similar to AND gate and OR gate in digital electronics. They are used to combine two or more conditions/constraints or to complement the evaluation of the original condition under particular consideration. 

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 013](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/8ee4e5ee-0e0f-460e-8072-6beaa22d1e0b)



6. **Ternary Operator**

---

Java ternary operator is the only conditional operator that takes three operands. It’s a one-liner replacement for the if-then-else statement and is used a lot in Java programming. We can use the ternary operator in place of if-else conditions or even switch conditions using nested ternary operators.

**Syntax:**
~~~
 **variable = Expression1 ?  Expression2 : Expression3**
~~~
![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 014](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/59929c5b-ca9a-42bb-a45b-6809d8e696d6)




**Type Casting in Java :**

---


In Java, type casting is a method or process that converts a data type into another data type in both ways manually and automatically. The automatic conversion is done by the compiler and manual conversion is performed by the programmer. 

![Aspose Words d04dd5c6-5058-461f-907f-426e8aa3b525 015](https://github.com/rhushikesh2000/Java_tutorial/assets/124034778/114192ec-481a-4dc7-8485-343144d14b6f)


**Types of Type Casting**

---

There are two types of type casting:
- Widening Type Casting
- Narrowing Type Casting

**Widening Type Casting**

---

Converting a lower data type into a higher one is called widening type casting. It is also known as implicit conversion or casting down. It is done automatically. It is safe because there is no chance to lose data. It takes place when:

- Both data types must be compatible with each other.
- The target type must be larger than the source type.
~~~
byte -> short -> char -> int -> long -> float -> double  
~~~
For example, the conversion between numeric data types to char or Boolean is not done automatically. Also, the char and Boolean data types are not compatible with each other. Let's see an example.
~~~java
public class WideningTypeCastingExample  

{  

public static void main(String[] args)  

{  

int x = 7;  

//automatically converts the integer type into long type  

long y = x;  

//automatically converts the long type into float type  

float z = y;  

System.out.println("Before conversion, int value "+x);  

System.out.println("After conversion, long value "+y);  

System.out.println("After conversion, float value "+z);  

}  

}  
~~~

**Output:**
~~~
Before conversion, the value is: 7

After conversion, the long value is: 7

After conversion, the float value is: 7.0
~~~
**Narrowing Type Casting**

---

Converting a higher data type into a lower one is called narrowing type casting. It is also known as explicit conversion or casting up. It is done manually by the programmer. If we do not perform casting then the compiler reports a compile-time error.
~~~
double -> float -> long -> int -> char -> short -> byte 
~~~
Let's see an example of narrowing type casting.

In the following example, we performed the narrowing type casting two times. First, we have converted the double type into a long data type after that long data type is converted into an int type.
~~~java
public class NarrowingTypeCastingExample  

{  

public static void main(String args[])  

{  

double d = 166.66;  

//converting double data type into long data type  

long l = (long)d;  

//converting long data type into int data type  

int i = (int)l;  

System.out.println("Before conversion: "+d);  

//fractional part lost  

System.out.println("After conversion into long type: "+l);  

//fractional part lost  

System.out.println("After conversion into int type: "+i);  

}  

}  
~~~
**Output:**
~~~
Before conversion: 166.66

After conversion into long type: 166

After conversion into int type: 166
~~~
