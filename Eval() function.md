## eval() function:
> eval() function is used when we have to evaluate certain expression. As eval() function is capable of taking float/int or str input & giving the resultant output in integer/float.

##### Syntax: eval()

      a, b, c = 5, 3, 9
      print(a+3*b-2*c) # 4

###### Example: 
        a, b, c = 5, 3, 9
        # but if we use eval()
        output = eval(a+3*b-2*c)
        print(output) # -4
        var = eval(input("Enter a value: "))
        # Enter a value: 45.678
        print(type(var)) # <class 'float'>
        # var = eval(input("Enter value: "))
        # Enter value: Hello # invalid - Hello is not defined because eval() will treat 'Hello' as a variable
        
          


