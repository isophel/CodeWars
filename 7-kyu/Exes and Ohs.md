Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contains any char. When no 'x' and 'o' is present should return true.

```py
def xo(s):
    # initialize variables
    x = 0
    o = 0
    
    # for each element in string
    # check if converted to lowercase string is equal to 'x' or 'o'
    # and add +1 to corresponding variable
    # if no 'x' or 'o' occurse variables are equal to 0
    
    for el in(s):
        if str(el).lower() == 'x':
            x += 1
        elif str(el).lower() == 'o':
            o += 1
    if x == o:
        return True
    else:
        return False
```        
________________________
way better solutions
```py
def xo(s):
    s = s.lower()
    return s.count('x') == s.count('o')
```
```py
def xo(s):
    return s.lower().count('x') == s.lower().count('o')
```
