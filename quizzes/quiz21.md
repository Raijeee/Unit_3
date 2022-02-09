# Scientific Notation Create a function to convert every number given to scientific notation.

## scientifiNot(number: int) -> :str

```.py
def scientifiNot(number):
    #Converts numeric numbers to scientific notations
    head=str(number)[0] # The first number is indexed with [0].
    middle=str(number)[1:3] # The middle number is indexed with [1:3] for first letter to third letter
    end=len(str(number))-1 # The end number is indexed with [-1].
    out=(f"{head}.{middle} * 1e{end}") # Strucutre the ouput as according
    return out
#Test 1
a=scientifiNot(137000)
print(a)
#Test 2
b=scientifiNot(1520000)
print(b)
#Test 3
c=scientifiNot(100)
print(c)
```

# Output:

![](quiz21out.png)
