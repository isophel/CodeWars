Create a function named divisors that takes an integer and returns an array with all of the integer's divisors(except for 1 and the number itself). If the number is prime return the string '(integer) is prime' (use Either String a in Haskell).

You can assume that you will only get positive integers as inputs.
```py

# for each number in range excluding 1 and integer itself
# check if division remainder is equal to zero
# if so add i to list

def divisors(integer):
    temp = []
    for i in range(2, integer):
        if integer%i == 0:
            temp.append(i)
    
    if len(temp) == 0:
        outputStr = str(integer) + " is prime" 
        return outputStr
    else:
    	return temp
```  

other solutions
```py
def divisors(num):
    l = [a for a in range(2,num) if num%a == 0]
    if len(l) == 0:
        return str(num) + " is prime"
    return l
 ``` 
 ```py
 def divisors(n):
    return [i for i in xrange(2, n) if not n % i] or '%d is prime' % n
```
