## Python Input:
> In python, we have the input() function which allow us to take the input from the user.

#### Syntax:
> input([prompt]) # where prompt is the string we use when we wish to display some message on screen so it's optional.

###### Example:
      num = input("Enter a number: ")
      print(num)

      # Output: Enter a number: 15
      # 15

### Python Output:
> In python, we use the print() function  to output data to the standard output device.

#### Syntax: 
> print(*objects, sep="", end="\n", file=sys.stdout, flush=False)

>  - Here, <span style='color:black;font-weight:bold'>objects</span> is the values to be printed.
> - The <span style='color:black;font-weight:bold'>sep</span> is separator which is used between the values. It defaults into a space character.
> - After all values are printed, <span style='color:black;font-weight:bold'>end</span> is printed. It defaults into a new line.
> - The file is the object where the values are printed & its default value is sys.stdout(screen)
> - <span style='color:black;font-weight:bold'>flush</span> parameter is used to flush (clear) the internal buffer/stream (or we can say it is used to flush the output stream), it has two values "False" and "True".

