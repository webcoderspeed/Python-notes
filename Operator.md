## Operators:
> Python language supports the following types of operators:-
>- 1) Arthmetic Operators
>- 2) Comparison (Relational) Operators
>- 3) Assignment Operaators
>- 4) Logical Operators
>- 5) Bitwise Operators
>- 6) Membership Operators
>- 7) Identity Operators

#### <strong>Arthmetic operators:</strong>
> Assume: a=10, b=20
   <table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>(+) Addition</td>
      <td>Add values on either side of the operator</td>
      <td>a+b = 30</td>
    </tr>
    <tr>
      <td>(-) Subtraction</td>
      <td>Substracts right hand operand fro left hand operand</td>
      <td>a-b = -10</td>
    </tr>
    <tr>
      <td>(*) Multipliction</td>
      <td>Multiplies values on either side of the operator</td>
      <td>a*b = 200</td>
    </tr>
    <tr>
      <td>(/) Division</td>
      <td>Divides left hand operands by right operand</td>
      <td>a/b = 2</td>
    </tr>
    <tr>
      <td>(%) Modulus</td>
      <td>Divides left operands by right hand operand and returns the remainder</td>
      <td>b%a = 0</td>
    </tr>
    <tr>
      <td>(**) Exponnent/Power</td>
      <td>Performs exponential calculation on operator</td>
      <td>a**b = 10 to the power of 20 = 10<sup>20</sup></td>
    </tr>
    <tr>
      <td>(//) Floor</td>
      <td>The division of operands where the result is quotient in which the digits after the decimal points are removed</td>
      <td>9//2 = 4 <br> 9.0 // 2.0 = 4.0 <br>9.4523//2.4512 = 3.0</td>
    </tr>
  </table>

#### <strong>Comparsion operators:</strong>
> These operators compare the values on either sides of them and decide the relation among them. They are also called Relation Operators.
>> Assume a = 10, b = 20

<table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>==</td>
      <td>If the values of two operands are qual then the condition becomes true</td>
      <td>a==b # false</td>
    </tr>
    <tr>
      <td>!=</td>
      <td>If the values of two operands are not equal then the condition becomes true</td>
      <td>a!=b # true</td>
    </tr>
    <tr>
      <td><></td>
      <td>If values of two operands are not equal then the condition becomes true</td>
      <td>a<>b # true</td>
    </tr>
    <tr>
      <td>></td>
      <td>If the values of the left operand is greater than the values right operand, then condition becomes true</td>
      <td>a>b # false</td>
    </tr>
    <tr>
      <td><</td>
      <td>If the values of the left operand is less than the value of right operand, then condition becomes true</td>
      <td>a < b # true </td>
    </tr>
    <tr>
      <td>>=</td>
      <td>If the value of left operand is greater than or qual to the value of right operand, then condition becomes true</td>
      <td>a>=b # false</td>
    </tr>
    <tr>
      <td><=</td>
      <td>If the value of left operand is less than or qual to the value of right operand, then condition becomes true</td>
      <td>a<=b # true</td>
    </tr>
  </table>

#### <strong>Assignment operators:</strong>
> An assignment operator is the operator used to assign a new value a variable
>> Assume a=10, b=20

 <table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>=</td>
      <td>Assign values from right side operands to left side operand</td>
      <td>c=a+b # assigns value of a+b into c</td>
    </tr>
    <tr>
      <td>+=</td>
      <td>If adds right operand to the left operand and assign the result to left operand</td>
      <td>a+=b # which is equivalent to a = a+b</td>
    </tr>
    <tr>
      <td>-=</td>
      <td>It substracts right operand from the left operand and assign the result to left operand</td>
      <td>a-=b # which is equivalent to a = a-b</td>
    </tr>
    <tr>
      <td>*=</td>
      <td>It multiplies right operands with the left operand and assign the result to left operand</td>
      <td>a*=b # which is equivalent to a = a*b</td>
    </tr>
    <tr>
      <td>/=</td>
      <td>It divides the left operand with the right operand and assign the result to left operand</td>
      <td>a/=b # which is equivalent to a = a/b</td>
    </tr>
    <tr>
      <td>%=</td>
      <td>It takes modulus using two operands and assign the resilt to left operand</td>
      <td>a%=b # which is equivalent to a = a%b</td>
    </tr>
    <tr>
      <td>**=</td>
      <td>It performs exponential(power) calculation on operands and assign value to left operand</td>
      <td>a**=b # which is equivalent to a = a**b</td>
    </tr>
    <tr>
      <td>//=</td>
      <td>It performs floor division on operators and assign value to left operand</td>
      <td>a**=b # which is equivalent to a = a**b</td>
    </tr>
  </table>

#### <strong>Logical operators:</strong>
> Logical operators are typically used with Boolean values
>> Assume a = True, b = False

<table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>and (Logical AND)</td>
      <td>If both the operands are true then condition becomes true</td>
      <td>a and b # false</td>
    </tr>
    <tr>
      <td>or (Logical OR)</td>
      <td>If any of the two operands are true then condition becomes true</td>
      <td>a or b # true</td>
    </tr>
    <tr>
      <td>not (Logical NOT)</td>
      <td>Used to reverse the logical state of its operand</td>
      <td>!a # false</td>
    </tr>
  </table>

###### AND truth table (how Logical AND works): 
> Y (output) : A.B (dot(.) represent multiplication)
> Above line can also be written as Y = A and B

<table>
    <tr>
      <th>A</th>
      <th>B</th>
      <th>Y = A and B</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </table>

###### OR truth table (how Logical OR works): 
> Y (output) : A+B (plus(+) represent addition)
> Above line can also be written as Y = A or B

<table>
   <tr>
      <th>A</th>
      <th>B</th>
      <th>Y = A + B</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr> 
</table>


###### NOT truth table (how Logical NOT works): 
> Y (output) : !A (! used to give opposite of value; if TRUE then it will false)
> Means if A = 1, then Y = !A = 0 

<table>
    <tr>
      <th>A</th>
      <th>Y = !A</th>
    </tr>
    <tr>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0</td>
    </tr>
</table>

#### <strong>Bitwise operators:</strong>
> Bitwise operator works on bits and performs bit-by-bit operation
>> Assume a = 60, b = 13

<table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>& (Binary AND)</td>
      <td>Operators copies a bit to the result if it exists in both operands</td>
      <td>a = 0b0011 1100 <br> b = 0b0000 1101 <hr> a & b = 0b0000 1100 <hr> a & b = 12 </td>
    </tr>
    <tr>
      <td>| (Binary OR)</td>
      <td>It copies a bit, if it exists in either operand</td>
      <td>a = 0b0011 1100 <br> b = 0b0000 1101 <hr> a | b = 0b0011 1101 <hr> a | b = 61 </td>
    </tr>
    <tr>
      <td>^ (Binary XOR)</td>
      <td>It copies the bit, if it is set in one operand but not both</td>
      <td>a = 0b0011 1100 <br> b = 0b0000 1101 <hr> a ^b = 0b0011 0001 <hr> a ^ b = 49 </td>
    </tr>
    <tr>
      <td>~ (Binary one's complement)</td>
      <td>It is unary and has the effect of 'flipping bits'</td>
      <td>a = 0b0011 1100 <br> ~a = 1100 0011 <hr> ~a = -61</td>
    </tr>
    <tr>
      <td><< (Binary left shift)</td>
      <td>The left operands value is moved left by the left number of bit specified by the right operand</td>
      <td> a = 0b0011 1100 <hr> b = a << 2 <hr> b = 240 <hr> b = 0b1111 0000 </td>
    </tr>
    <tr>
      <td>>> (Binary right shift)</td>
      <td>The right operands value is moved right by the right number of bit specified by the right operand</td>
      <td> a = 0b0011 1100 <hr> b = a >> 2 <hr> b = 15 <hr> b = 0b0000 1111 </td>
    </tr>
</table>

#### <strong>Membership operators:</strong>
> Membership operators test for membership in a sequence such as strings, list or tuples.

<table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>in</td>
      <td>Evaluates to True, if it finds a variable in the specified sequence and False otherwise</td>
      <td>(x in y) is True when x is a member of sequence y. <br>
      Example: <br>
       x = 2
       y = [1, 2, 3]
       print(x in y) # True
      </td>
    </tr>
    <tr>
      <td>not in</td>
      <td>Evaluates to True; if it does not find a variable specified sequence and False otherwise</td>
      <td>(x not in y) is True when x is not a member of sequence y. <br>
      Example: <br>
       x = 4
       y = [1, 2, 3]
       print(x not in y) # True </td>
    </tr>
</table>

#### <strong>Identity operators:</strong>
> Identity operators compare the memory locations of two objects.

<table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
      <th>Example</th>
    </tr>
    <tr>
      <td>is</td>
      <td>Evaluates to True, if the variables on either side of the operator point to the same object and False otherwise</td>
      <td>(x is y) is True, when id(x) equals to id(y) <br>
      Example: <br>
      x = 1
      y = 1
      print(x is y) # True
      </td>
    </tr>
    <tr>
      <td>is not</td>
      <td>Evaluates to False, if the variables on either side of the operator point to the same object and True otherwise</td>
      <td>(x is not y) is True, when id(x) is not equals to id(y) <br>
      Example: <br>
      x = 1
      y = 1
      print(x is not y) # False
      </td>
    </tr>
</table>

#### <strong>Operators precendance:</strong>
> <strong>PEMDAS:</strong> Power Exponent Multiplication Divide Addition Substraction
> The following table list all the operators from highest precedence to the lowest:

  <table>
    <tr>
      <th>Operator</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>**</td>
      <td>Exponentation (raise to the power)</td>
    </tr>
    <tr>
      <td>~, +, -</td>
      <td>Complement, unary plus and minus</td>
    </tr>
    <tr>
      <td>*, /, %, //</td>
      <td>Multiply, Divide, Modulo and Floor Division</td>
    </tr>
    <tr>
      <td>+, -</td>
      <td>Addition and Substraction</td>
    </tr>
    <tr>
      <td>>>, <<</td>
      <td>Right and Left bitwise shift</td>
    </tr>
    <tr>
      <td>&</td>
      <td>Bitwise AND</td>
    </tr>
    <tr>
      <td>^, |</td>
      <td>Bitwise exclusive 'OR' and 'OR'</td>
    </tr>
    <tr>
      <td><=, <>, >=</td>
      <td>Comparison operators</td>
    </tr>
    <tr>
      <td><, >, ==, !=</td>
      <td>Equality operators</td>
    </tr>
    <tr>
      <td>=, %=, /=, //=, -=, +=, *=, **=</td>
      <td>Assignment operator</td>
    </tr>
    <tr>
      <td>is, is not, in, not in, not, or, and</td>
      <td>Membership operators and Logical operators</td>
    </tr>
</table>

#### <strong>Variable formatting:</strong>
> Three ways by which you can format a variable.
>- 1) Using format() function and {}

      Example:
      a = 10, b = 20
      print("This value of a: {} and b: {}".format(a, b))
      # output: The value of a: 10 and b: 20

>- 2) Using format() function with indexes and {}

      Example: 
      a = 10, b = 20
      print("This value of b: {1} and a: {0}".format(a, b))
      # output: The value of b: 20 and a: 10

>- 3) Using Shorthand of format() function[f]

      Example: 
      a = 10, b = 20
      print(f"The value of a: {a} and b: {b}")
      # output: The value of a: 10 and b: 20