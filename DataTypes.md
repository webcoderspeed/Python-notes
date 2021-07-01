# DataTypes:
> The data stored in memory can be of many types.

> Python has various standard datatypes that are used to define the operations possible on them & the storage method for each of them.

## Python has 5 standard datatypes:

> 1. Numbers
> 2. String
> 3. List
> 4. Tuple
> 5. Dictionary

### Number:
> Number datatypes store numeric values.

> Number objects are created when you assign a value to them.
eg: num1 = 5

> <span style='color:black;font-weight:bold;'>Note</span>: You can also delete the reference to a object by using the del statement.

##### Syntax:
> del var1[, var2[, var3[...,varN]]]

#### Python Supports 4 different numerical types:
> 1) int (signed integers)
> 2) long (long integers, they can also be represtend in octal and hexadecimal)
> 3) float (floating point real values)
> 4) complex (complex Numbers)

### Strings: 
> Strings in python are identified as a contiguous set of characters represented in the quotation marks, python allows for either pairs of single or double quotes.

> Subsets of strings cn be taken using the slice operator([] and [:]) with indexes starting at 0 in the beginning of the string & working from -1 at the end.

> The plus(+) sign is the string concatenation operator & asterisk(*) is the repetition operator.

##### Example:
      s = 'Hello'
      print(s) # prints complete string

      # using the escape character when writting string in multiple line
      s = "Hello" \ 
          "World"

      # writting string in multiple line using 
      ''' ''' or """ """
      s = '''
          This is 
          a
          multiline string
          '''

      s = """
          This is 
          a
          multiline string
          """

      # string are immutable in nature means cannot be changed
      s = "Hi"
      # s[0] = "A" # Not valid

      # accessing the character of string using index values
      s = "Hello Speed"
      print(s[0]) # prints first character of the string.

      print(s[2:5]) # prints characters starting from 2nd position to 5-1 (4th) position
      
      print(s[2:]) # prints string starting from 2nd index

      print(s*2) # prints string two times

      print(s+"Sharma") # prints the concatenate strings

      # output:
      # H
      # llo
      # llo Speed
      # Hello Speed Hello Speed
      # Hello Speed Sharma

    
###### More Examples on String Function:
        
        s = "Hello World"

        print(s.capitalize()) # output: Hello World

        print(s.casefold()) # output: hello world

        print(s.center(50))  # output: { Returns a centered string of length width. Padding is done using the specified fill character (default is a space) }

        print(s.center(100, '*')) # output: ********************************************Hello World*********************************************

        print(s.upper()) # output: HELLO WORLD

        print(s.count('l')) # output: 3

        print(s.find('World')) # output: 6

        print(s.startswith('h')) # output: False

        print(s.endswith('d')) # output: True


### Lists:
> Lists are the most versatile of python's compound datatypes.

> A list containings items seperated by commas & enclosed within brackets([]).

> List are similar to array, one difference between them is that all the items, belonging to a list can be of different datatypes.

###### Example: 
        a_list = [1,2.5,'Speed']
        b_list = [5, 'CSE']

        print(a_list) # prints complete list

        print(a_list[0]) # prints the first element of the list

        print(a_list[1:3]) # prints the elements from 1st index position to 3-1 (2nd) index position

        print(a_list[1:]) # prints elements starting from 1st index position

        print(b_list*2) # prints the list two times

        print(a_list+b_list) # prints the concatenated lists

#### Updating List:
> You can update single or multiple elements of list by giving the slice on the left-hand side of the assignment operator, and you can add to elements in a list with the append() method.

###### Example:
        # updating elements of list
        list1 = [10, 'SPEED', '9.8', 'CSE']
        print(f"list1[1]: {list1[1]}")  # output: list1[1]: SPEED

        list1[1] = 'SPEED SHARMA'# updating the second element of list
        print(list1)  # output: [10, 'SPEED SHARMA', '9.8', 'CSE']

        # adding elements to a list
        data = [1,2,3]
        data.append(4) # adding element to list using append() method
        print(data)  # output:[1, 2, 3, 4]

#### Delete list elements:
> To remove a list element, you can use either the del statement if you know exactly which element you deleting.

##### Example:
        data = [10, 'SPEED', '9.8', 'CSE']
        print("Before deleting list element are: ", data)
        del data[0]
        print("After deleting list element are: ", data)

        # output:
        # Before deleting list element are:  [10, 'SPEED', '9.8', 'CSE']
        # After deleting list element are:  ['SPEED', '9.8', 'CSE']

#### Basic List Operation : 
> 1. len() : Find the length of the list.

        data = [10, 20, 30]
        print("Number of elements in datalist: ", len(data))
        #output: Number of elements in datalist: 3

> 2. \+ : Concatenation of lists.

        a_list = [10, 20]
        b_list = [30, 40]
        print(a_list + b_list) # prints the concatenated list

> 3. \* : Repeatition of list elements 
        
        a_list = [10, 20, 30]
        print(a_list*2) # prints the list 2-times

> 4. in : Membership operator which returns True when element present in list. False otherwise.

        a_list = [10, 20, 30, 40]
        print(20 in a_list) # True
        print(50 in a_list) # False

##### Built-in Functions and Methods

> 1. max() : This method returns the element from the list with maximum value.
###### Syntax: max(list)

        data = [10,20,30]
        print(max(data)) # output: 30

> 2. min() : This method returns the element from the list with minimum value.
###### Syntax: min(list)

        data = [10,20,30]
        print(min(data)) # output: 10

> 3. list() : This method takes sequence types and converts them to lists. This is used to convert any given object into list.
###### Syntax: list(obj)

        tuple1 = (10, 20, 30)
        print(list(tuple1)) # converts the tuple object in list object
        # output: [10, 20, 30]

> 4. append() : This method appends a passed object into the existing list. In simple words append() is used to add the element to list.

###### Syntax: listObject.append(obj)

        data = [10, 20, 30]
        data.append(40)
        print(data) # output: [10, 20, 30, 40]

> 5. count() : This method return count of how many times obj occurs in list.

###### Syntax: listObject.count(obj)

        data = [10, 20, 30]
        print(data.count(20)) # output: 1

> 6. extend() : This method appends the contents of sequence to list.

###### Syntax: list.extend(sequence)

        a_list = [10, 20, 30]
        b_list = [40, 50, 60]
        a_list.extend(b_list)
        print(a_list) # output: [10, 20, 30, 40, 50, 60]

> 7. index() : This method returns the lowest index in list that obj appears.

###### Syntax: listObject.index(obj)

        data = [10, 20, 30]
        print(data.index(20)) # output: 1

> 8. insert()  : This method inserts obj into list at offset index.

###### Syntax: listObject.insert(index, obj)

        data = [10, 20, 30]
        data.insert(1, 50)
        print(data) # output: [10, 50, 20, 30]

> 9. pop() : This method removes and returns last obj from the list.

###### Syntax: listObject([index])

        data = [10, 20, 30]
        print(data.pop(1)) # output: 20

> 10. remove() : This method does not return any value but removes the given obj from the list.

###### Syntax: listObject.remove(obj)

        data = [10, 20, 30]
        data.remove(20)
        print(data) # [10, 30]

> 11. reverse() : This method does not return any value but reverse the given obj from the list.

###### Syntax: listObject.reverse()

        data = [10, 20, 30]
        data.reverse()
        print(data) # output: [30, 20, 10]

> 12. sort() : This method sorts obj of list, use compare function if given.

###### Syntax: listObject([function]) 

        data = [5, 10, 9, 4, 3, 7 , 4, 1 ]
        data.sort()
        print(data) # output: [1, 3, 4, 4, 5, 7, 9, 10]


