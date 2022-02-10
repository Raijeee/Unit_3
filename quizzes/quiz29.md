# Find the number of divisors of the input number that are divisible by 2. 

'''.py

def findtwodivisors(num):
    out=0 # Set output to 0 and integer
    if num%2==1: # If the number is not divisible by 2, set 0
        out=0
    else: # Otherwise
        while num!=0: # while the number is not equal to 0
            num/=2 # Input divide by 2
            out+=1 # Increase output by 1
    return out # Return output
out1=findtwodivisors(82392)
print(out1)
'''

# Code:
![](quiz29out.png)

# Output: 

![](quiz29out.png)
