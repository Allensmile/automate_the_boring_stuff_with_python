
# Ch4 Practice Project
## Comma code

Say you have a list value like this:

spam = ['apples', 'bananas', 'tofu', 'cats']

Write a function that takes a list value as an argument and returns a string with all the items separated by a comma and a space, with and inserted before the last item. For example, passing the previous spam list to the function would return 'apples, bananas, tofu, and cats'. But your function should be able to work with any list value passed to it.


```python
def printList(listToPrint):
    string = ''
    for i in range(0, len(listToPrint)-1):
        string += str(listToPrint[i])
        string += ', '
    string += 'and '
    string += listToPrint[-1]
    return string
```


```python
testList = ['apples', 'bananas', 'tofu', 'cats']
print(printList(testList))

testList = ['apples', 1, 'bananas', True, 'tofu', -3.14, 'cats']
print(printList(testList))
```

    apples, bananas, tofu, and cats
    apples, 1, bananas, True, tofu, -3.14, and cats

