# Awesome python tricks 

This is a repo where I share some cool python tricks that I consider useful, this notes will be updated as I learn new things

This uses `python >= 3.7.1`.


## 1. Tuples 

 - Tuples use lexicographic order, it can be useful for sorting lists of tuples, finding maximum and minimum and their respective indices.

```python

min((listOfNumbers[i], i) for i in range(len(listOfNumbers)))

max((listOfNumbers[i], i) for i in range(len(listOfNumbers)))
```

- Tuples are immutable : 

```python

tuple = (1,['a','b'])

tuple[0] = 8 # this isn't possible in python
```

In python we can't change the object references, However the values of the tuple may potentially change. 

```python

tuple = (1,['a','b'])

letters = tuple[1]

letters.append('c') 

print(tuple) # (1,['a','b','c'])
```

Variables are just names we give to objects stored in memory, namely, the second element of tuple, and letters points to the same object in memory, so by changing the value of letters, the second item of tuple will automatically change. 