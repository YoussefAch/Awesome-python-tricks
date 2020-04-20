# Awesome python tricks 

This is a repo where I share some cool python tricks that I consider useful, this notes will be updated as I learn new things

This uses `python >= 3.7.1`.


## 1. Tuples 

Tuples use lexicographic order, it can be useful for sorting lists of tuples, finding maximum and minimum and their respective indices.

```python

min((listOfNumbers[i], i) for i in range(len(listOfNumbers)))

max((listOfNumbers[i], i) for i in range(len(listOfNumbers)))
```