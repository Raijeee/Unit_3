# Black Box

```.py
def blackbox(input):
    #This black box counts the number of letters inbetween the first and last letters.
    out=""
    words=input.split()
    for words in words:
        if len(words)<=2:
            out+=(words+" ")
        else:
            out+=(words[0]+str(len(words)-2)+words[-1]+" ")
    return out
#Test 1
a=blackbox("internationalization")
print(a)
#Test 2
b=blackbox("Hello world !")
print(b)
#Test 3
c=blackbox("(codin) + (game) = (codingame)")
print(c)
```

# Output

![](quiz22out)
