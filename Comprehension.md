### Comprehension:
> Comprehension helps programmers to create lists/generator object/dictionary in a concise way.
###### Syntax:
        [output iteration condition]

#### List Comprehensions:
> Python supports completed lists called list comprehension.
###### Syntax:
      a_list = [expression for variable in sequence]
      '''
      where,
      the expression is evaluated once, for every item in the sequence.
      '''

> List comprehension help programmers to create lists in a concise way. This is mainly beneficial to make new lists where each element is obtained applying some operations to each member of another sequence or iterable.

> List comprehension is also used to create a subsequence of those elements that satisfy a certain condition.

      # Example:
      squares = [(i**2) for i in range(11)]
      print(squares)
      # Output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

      # Example:
      names = ['nik', 'fury']
      print([len(name) for name in names])
      # output: [3, 4]

      # Example: First letter Capitalize
      print([name.capitalize() for name in names])
      # output: ['Nik', 'Fury']

      # Example: only those whose length>3
      print([name.capitalize() for name in names if len(name)>3])
      # output: ['Fury']

#### Ternary Operator: if condition else
##### Syntax example: num1 if num1>num2 else num2 

      # Example: Ternary Operator
      names = ['nik', 'fury', 'james', 'lex', 'anna', 'king', 'blake']
      print([name.upper() if len(name)>4 else name for name in names]) 
      # output: ['nik', 'fury', 'JAMES', 'lex', 'anna', 'king', 'BLAKE']

      # Example: Create a new dictionary using dictionary comprehension with key and value square.
      print({i: i*i for i in range(1, 11)})
      # output: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64, 9: 81, 10: 100}

      # Example: create a new set using set comprehension
      print({i*i for i in range(1, 11)})
      # output: {64, 1, 4, 36, 100, 9, 16, 49, 81, 25}

