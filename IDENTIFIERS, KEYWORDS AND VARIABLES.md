# Python Identifiers:
> A python identifier is a name used to identify a variable, function, class, module or other objects.

> An Identifier starts with a letter A-Z or a-z or an underscore( _ ) followed by zero or more letters, underscore & digits (0 to 9).

#### The following are naming conventions for Python Identifiers:

> Class names start with an uppercase letter. All other identifiers start with a lowercase letter and these identifier are called as public identifier.

> Starting an Identifier with a single leading underscore indicates that the identifier is protected

> Starting an Identifier with two leading underscore indicating a strongly private identifiers.

> If the Identifier starts and ends with two trailing underscores the identifier is a language-defined special name.


## Public, Protected and Private Attributes

> <span style='color:skyblue;font-weight:bold'>Public</span> attributes can only be accessed inside of the class definition.

> <span style='color:skyblue;font-weight:bold'>Protected</span> (restricted) attributes should only be used under certain conditions.

> <span style='color:skyblue;font-weight:bold'>Private</span> attributes can only be accessed inside of the class definition. 


<table  border='2'>
  <tr style='background: rgba(35, 52, 238, 0.735)'>
  <th style='color:#fff;'>Naming</th>
  <th style='color:#fff;'>Type</th>
  <th style='color:#fff;'>Meaning</th>
  </tr>
  <tr>
    <td>name</td>
    <td>Public</td>
    <td>These attributes can be freely used inside or outside of a class definition</td>
  </tr>
  <tr>
    <td>_name</td>
    <td>Protected</td>
    <td>Protected attributes should be used outside of the class definition, unless inside of a subclass definition</td>
  </tr>
  <tr>
    <td>__name</td>
    <td>Private</td>
    <td>This kind of attribute is inaccessible and invisible. It's neither possible to read nor to write those attributes, except inside of the class definition itself</td>
  </tr>
</table>

> Also, the <span style='color:skyblue;font-weight:bold'>str.isidentifier() </span>  function will tell us if a string is a valid identifier. This is available since Python 3.0.

      '__99__'.isidentifier()
>Output: True

 ## Python Keywords
 > Keywords are reserved words and you cannot use them as constant or variable or any other identifier names.

 > All the python keywords contain lowercase letters only.

<table>
    <tr>
      <td>and</td>
      <td>def</td>
      <td>exec</td>
      <td>if</td>
      <td>not</td>
      <td>return</td>
    </tr>
    <tr>
      <td>assert</td>
      <td>del </td>
      <td>finally</td>
      <td>import</td>
      <td>or</td>
      <td>try</td>
    </tr>
    <tr>
      <td>break</td>
      <td>elif</td>
      <td>for</td>
      <td>in</td>
      <td>pass</td>
      <td>while</td>
    </tr>
    <tr>
      <td>class</td>
      <td>else</td>
      <td>async</td>
      <td>from</td>
      <td>print</td>
      <td>is</td>
    </tr>
    <tr>
      <td>continue</td>
      <td>except</td>
      <td>global</td>
      <td>lambda</td>
      <td>raise</td>
      <td>yield</td>
    </tr>
</table>

## Variables
> Variables are nothing but reserved memory locations to store values. This means when you create a variable, you reserve some space in memory.

> Based on the datatype of a variable, the interpreter allocates memory & decided what can be stored in the reserved memory.

### Assigning values to variables:
> Python variables do not need explicit declaration ton reserve memory space. The declaration happens automatically when you assign a value to variable. The equal sign ( = ) is used to assign value to variables.

##### Example: 
      area_code = 110074 # type - int 
      name = "Speed" # type - str (string)
      floating_variable = 12.25 # type - float 

      # assigning single values to multiple variables
        a, b, c = 1 

      # assigning multiple values to multiple variables
      a, b, c = 12, 13, 14
