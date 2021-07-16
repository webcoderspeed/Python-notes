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
> eg: num1 = 5

> <span style='color:black;font-weight:bold;'>Note</span>: You can also delete the reference to a object by using the del statement.

##### Syntax:

> del var1[, var2[, var3[...,varN]]]

#### Python Supports 4 different numerical types:

> 1. int (signed integers)
> 2. long (long integers, they can also be represtend in octal and hexadecimal)
> 3. float (floating point real values)
> 4. complex (complex Numbers)

### Strings:

> Strings in python are identified as a contiguous set of characters represented in the quotation marks, python allows for either pairs of single or double quotes.

> Subsets of strings cn be taken using the slice operator([] and [:]) with indexes starting at 0 in the beginning of the string & working from -1 at the end.

> The plus(+) sign is the string concatenation operator & asterisk(\*) is the repetition operator.

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

> 8. insert() : This method inserts obj into list at offset index.

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

### Tuples:

> A Tuple us another sequence datatypes that is similar to the list. A tuple consists of a number of values seperated by commas. Unlike lists, tuple are enclosed within parenthesis.

##### The main difference between lists and tuples are:

<table>
        <tr>
        <th>List</th>
        <th>Tuple</th>
        </tr>
        <tr>
        <td>Lists are enclosed in brackets []</td>
        <td>Tuples are enclosed in parenthesis ()</td>
        </tr>
        <tr>
        <td>Lists can be updated</td>
        <td>Tuples cannot be updated because tuples are immutable in nature but if the tuple consists of mutable child then the child can be updated. <br> eg: A list inside a tuple can be updated.
        </td>
        </tr>
</table>

#### Tuples can be thought of as read-only lists.

###### Example:

        a_tuple = (1, 2.5, 'Speed')
        b_tuple = (5, 'CSE', [1, 2])

        print(a_tuple) # print complete list
        # output: (1, 2.5, 'Speed')

        print(a_tuple[0]) # prints the first element of the list
        # output: 1

        print(b_tuple[2]) # prints the third element of the list
        # output: [1, 2]

        b_tuple[1] = 2 # Invalid

> Note: As we all know once the tuple is created it cannot be updated [size of the tuple can't be changed. And therefore we can't use assignment operator for mutating value inside of a tuple because tuples are immutable in nature. But if the consist of mutable object. i.e; A tuple consist of list. As in above example I have created a tuple named b_tuple with list inside of it so we can add/remove/update the elements of a list without affecting the size of tuple].

        b_tuple[2][0] = 3 # changing the value of first element of list inside a tuple

        print(b_tuple) # print complete list
        # output: (5, 'CSE', [3, 2])

###### Example:

        tuple_data = (1, 2.5, 'Speed')
        list_data = [1, 2.5, 'Speed']

        tuple_data[1] = 3.14 # Invalid syntax with tuple
        list_data[1] = 3.14 $ Valid syntax with list

### Dictionary:

> Dictionary is an ordered set of key: value pairs, with the requirement that the keys are unique( with one dictionary)

> Unlike sequences, which are indexed by a range of numbers, dictionaries are indexed by keys, which can be any immutable type; strings and numbers can be keys.

###### Example:

        a_dict =  {
               'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                }

        print(a_dict['name']) # print value for 'name' key
        # output: Sanjeev Sharma

#### Creating Dictionary:

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }
        b_dict = {} # empty dictionary

#### Accessing values in dictionary:

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }
        print(''''
                a_dict['roll_no'] : { a_dict['roll_no'] }
                a_dict['name'] : { a_dict['name'] }
                a_dict['branch'] : { a_dict['branch'] }
             ''')

        # output:
        '''
                a_dict['roll_no'] : 65
                a_dict['name'] : Sanjeev Sharma
                a_dict['branch'] : CSE
        '''

#### Updating dictionary:

> You can update a dictionary by adding a new entry or a key-value pair.

###### Example:

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print("Dictionary before updation: ", a_dict)

        a_dict['roll_no'] = 09
        a_dict['name'] = "Nik"
        a_dict['branch'] = "ECE"
        print("Dictionary after updation: ", a_dict)

        # output:
        '''
        Dictionary before updation: { 'roll_no' : 65, 'name' : 'Sanjeev Sharma', 'branch' : "CSE" }

        Dictionary after updation: { 'roll_no' : 09, 'name' : 'Nik', 'branch' : "ECE" }
        '''

#### Delete dictionary element:

> You can remove individual dictionary elements use del statement.

###### Example:

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print(a_dict)

        del a_dict['roll_no']
        print(a_dict)
        del a_dict
        print(a_dict) # An exception is raised because after del a_dict, the dictionary does not exist anymore

        # output:
        '''
        { 'roll_no' : 65, 'name' : 'Sanjeev Sharma', 'branch' : "CSE" }
        { 'name' : 'Sanjeev Sharma', 'branch' : "CSE" }
        NameError: name 'a_dict' is not defined
        '''

#### Properties of Dictionary keys:

> There are two important points to remember about dictionary keys:
>
> - More than on entry per key is not allowed. This means no duplicate key is allowed when duplicate keys are encountered during assignment, the last assignment is to be considered.
> - Keys must be immutable. This means you can use strings, number or tuples as dictionary keys but something like ['key'] is not allowed.

### Built-in Dictionary Functions & Methods:

> 1. len() - This method returns length of the dictionary.

###### Syntax: len(dict)

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
          }

        print(len(a_dict)) # output: 3

> 2. str() - This method produces a printable string representation of a dictionary.

###### Syntax: str(dict)

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
          }

        print(str(a_dict))

        # output: {'roll_no': '65', 'name': 'Sanjeev Sharma', 'branch': 'CSE'}

> 3. type() - This method return the type of the passed variable. If passed variable is dictionary then it would return a dictionary type.

###### Syntax: type(dict)

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
          }

        print(type(a_dict)) # output: <class 'dict'>

> 4. clear() - This method removes all items from the dictionary.

###### Syntax: dict.clear()

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
          }

        a_dict.clear()
        print(a_dict) # output: {}

> 5. copy() - This method returns a copy of the dictionary.

###### Syntax: dict.copy()

        a_dict = {
                'roll_no':'65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
          }

        b_dict = a_dict.copy()
        print(b_dict)

        # output: {'roll_no': '65', 'name': 'Sanjeev Sharma', 'branch': 'CSE'}

> 6. fromkeys() - This method create a new dictionary with keys from sequence and values set to value

###### Syntax: dict.fromkeys(sequence[, values])

        a_dict = {}

        keys = ['a', 'e', 'i', 'o', 'u']

        print(a_dict.fromkeys(keys)) # without value

        value = 'vowels'

        print(a_dict.fromkeys(keys, value)) # with value

        # output:
        '''
        {'a': None, 'e': None, 'i': None, 'o': None, 'u': None}
        {'a': 'vowels', 'e': 'vowels', 'i': 'vowels', 'o': 'vowels', 'u': 'vowels'}
        '''

> 7. get() - This method returns a value from the given dictionary by passing key in it. If the key is not available then it returns default value None.

###### Syntax: dict.get(key, default=None)

        a_dict = {
                'roll_no': '65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print(a_dict.get('name'))

        # output: Sanjeev Sharma

> 8. items() - This method returns a lift of dictionary(key, value) tuple pairs.

###### Syntax: dict.items()

        a_dict = {
                'roll_no': '65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print(a_dict.items())

        # output:
        """
        dict_items([('roll_no', '65'), ('name', 'Sanjeev Sharma'), ('branch', 'CSE')])
        """

> 9. keys() - This method returns a list of all the available keys in the dictionary.

###### Syntax: dict.keys()

        a_dict = {
                'roll_no': '65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print(a_dict.keys())

        # output: dict_keys(['roll_no', 'name', 'branch'])

> 10. setdefault() - This method is similar to get(), but will set dict[key] = default if the key is not already in dict.

###### Syntax: dict.setdefault(key, default=None)

        a_dict = {
                'roll_no': '65',
                'branch': 'CSE'
                 }

        a_dict.setdefault('name' )
        print(a_dict)

        # output: {'roll_no': '65', 'branch': 'CSE', 'name': None}

> 11. update() - This method adds key-values pairs of another dictionary into a given dictionary.

###### Syntax: a_dict.update(b_dict)

        a_dict = {
                'roll_no': '65',
                'branch': 'CSE'
                 }

        b_dict = {
                'name': 'Sanjeev Sharma'
                 }

        a_dict.update(b_dict)
        print(a_dict)

        # output: {'roll_no': '65', 'branch': 'CSE', 'name': 'Sanjeev Sharma'}

> 12. values() - This methods returns a list of all values available in a given dictionary.

###### Syntax: dict.values()

        a_dict = {
                'roll_no': '65',
                'name': 'Sanjeev Sharma',
                'branch': 'CSE'
                 }

        print(a_dict.values())

        # output: dict_values(['65', 'Sanjeev Sharma', 'CSE'])

### Sets

> A set is an an unordered collections of items. Every element is unique (no duplicates) & must be immutable (which cannot be changed)

#### Creating a set

> A set is created by placing all the items (elements) inside curly braces {} seperated byb comma or by using the built-in function set()
> It can have an umber of items & they may be of different types(integer, float, tuples, string etc). But a set cannot have a mutable element like list or dictionary as its elements.

        a_set = { 8.5, 'Speed', (1, 2, 3)}
        # alternate way using set() function
        a_set = set([8.5, 'Speed', (1, 2, 3)])

        # to create a empty set
        a_set = set()

#### Set operations:

> Sets can be used to carry to out mathematical set operations like union, intersection, difference & symmetric difference.

> 1. Set Union: Union of A & B is a set of all elements from both sets.
>    > Union is performed using | operator

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set | b_set)

        # output: {1, 2, 3, 4, 5, 6, 7, 8}

> 2. Set Intersection: Union of A & B is a set of elements that are common in both sets.
>    > Intersection is performed using & operator

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set & b_set)

        # output: {4, 5}

> 3. Set Difference: Difference of A and B (A-B) is a set of elements that are only in A but not in B.
>    > Similarly, B-A is a set of elements that are only in B but not in A.
>    >
>    > > Difference is performed using - operator

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set - b_set)
        print(b_set - a_set)

        # output:
        # {1, 2, 3}
        # {8, 6, 7}

4.  Set Symmetric difference:

    > Symmetric difference of A and B is a set of elements in both A and B except those that are common in both.
    >
    > > Symmetric difference is performed using ^ operator

            a_set = {1, 2, 3, 4, 5}
            b_set = {4, 5, 6, 7, 8}
            print(a_set ^ b_set)

            # output: {1, 2, 3, 6, 7, 8}

> 5. add(): Add an element to a set

###### Syntax: setobj.add(element)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        a_set.add(6)
        print(a_set)

        # output: {1, 2, 3, 4, 5, 6}

> 6. clear(): Remove all elements from a set

###### Syntax: setobj.copy(element)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        print("a_set: ", a_set)
        b_set = a_set.copy()
        print("b_set: ", b_set)

        # output:
        # a_set:  {1, 2, 3, 4, 5}
        # b_set:  {1, 2, 3, 4, 5}

> 7. difference_update(): Remove all elements of another set from this set.

###### Syntax: setobj_1.difference_update(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        a_set.difference_update(b_set)
        print(a_set)

        # output: {1, 2, 3}

> 8. intersection_update(): Update the set with the intersection of itself and another.

###### Syntax: setobj_1.intersection_update(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        a_set.intersection_update(b_set)
        print(a_set)

        # output: {4, 5}

> 9. isdisjoint(): Return True if two sts have a null intersection

###### Syntax: setobj_1.isdisjoint(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set.isdisjoint(b_set))

        # output: False

> 10. issubset(): Return True if another set contains this set

###### Syntax: setobj_1.issubset(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set.issubset(b_set))

        # output: False

> 11. issuperset(): Return True if this set contains another set

###### Syntax: setobj_1.issuperset(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set.issuperset(b_set))

        # output: False

> 12. pop(): Remove and return an arbitary set element. Raise key error if the set is empty.

###### Syntax: setobj.pop()

##### Example:

        a_set = {1, 2, 3, 4, 5}
        print(f"a_set: {a_set}")
        b_set = a_set.pop()
        print(f"b_set: {b_set}")

        # output:
        # a_set: {1, 2, 3, 4, 5}
        # b_set: 1

> 13. symmetric_difference(): Return the symmetric difference of two sets as a new set

###### Syntax: setobj_1.symmetric_difference(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        print(a_set.symmetric_difference(b_set))

        # output: {1, 2, 3, 6, 7, 8}

> 14. symmetric_difference_update(): Update a set with the symmetric difference of itself and another

###### Syntax: setobj_1.symmetric_difference_update(setobj_2)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        a_set.symmetric_difference_update(b_set)
        print(a_set)

        # output: {1, 2, 3, 6, 7, 8}

> 15. update(): Update a set with union of itself & other

###### Syntax: setobj_1.update(listobj [, setobj_2])

##### Example:

        a_set = {1, 2, 3, 4, 5}
        b_set = {4, 5, 6, 7, 8}
        listobj = [9, 10, 11, 12, 13, 14, 15]

        a_set.update(listobj) # without b_set
        print(a_set)

        # output: {1, 2, 3, 4, 5, 9, 10, 11, 12, 13, 14, 15}

        a_set.update(listobj) # with b_set
        print(a_set)

        # output: {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15}

> 16. discard(): Remove an element from set if it is a member. Do noting if the element is not in set

###### Syntax: setobj.discard(element)

##### Example:

        a_set = {1, 2, 3, 4, 5}
        a_set.discard(5)
        print(a_set)

        # output: {1, 2, 3, 4}