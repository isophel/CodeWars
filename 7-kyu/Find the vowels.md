We want to know the index of the vowels in a given word, for example, there are two vowels in the word super (the second and fourth letters).

So given a string "super", we should return a list of [2, 4].

Some examples:
```
Mmmm  => []  
Super => [2,4]  
Apple => [1,5]  
YoMama -> [1,2,4,6]  
```    
NOTE: Vowels in this context refers to English Language Vowels - a e i o u y  
NOTE: this is indexed from [1..n] (not zero indexed!)
```py
def vowel_indices(word):
	return [i+1 for i, l in enumerate(word) if l.lower() in 'aeiouy']
```
