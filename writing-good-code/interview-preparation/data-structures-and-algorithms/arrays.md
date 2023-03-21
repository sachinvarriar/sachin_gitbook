# Arrays

An array is one of the easiest storage of data where data is stored in contiguous memory locations. These memory locations are known as the index of the array. These indexes can be used to reference or retrieve a value stored in the array. An array can be a one dimensional structure or a multidimensional structure

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption><p>image courtesy:<a href="https://www.c-sharpcorner.com/article/array-in-python/">https://www.c-sharpcorner.com/article/array-in-python/</a></p></figcaption></figure>

Python does not have a native array data structure but a 'list' is the equivalent data structure. A single list data structure can store data of different data types.

The numpy package enables Python to have 1d, 2d arrays which can be used for computation.

The equivalent data structure in R is a vector. R also has a list data type which like it's python equivalent can house multiple data types and data structures within it. In R vectors and lists, the index of data structures starts at position 1 unlike python or C++

Note: Pay attention to the bigO notations in the comments. It is written in terms of time complexity of each operation.

{% code overflow="wrap" lineNumbers="true" %}
```python
fruits = ['apple','mango','banana']
fruits.append('orange') #bigO notation //O(1)
print(fruits)
```
{% endcode %}

The above script shows how to create a list in python and also append a new value.

{% code lineNumbers="true" %}
```python
fruits = ['apple','mango','banana']
fruits[0]
fruits[-1]
fruits[1:]
fruits[:-1]
```
{% endcode %}

This script illustrates how to work with list indexes

We can remove the last added value to a list using the below syntax

```python
fruits.pop() #bigO notation // O(1)
```

If we wish to add a new value to the list at a particular position and push the values forward from the index to which we wish to add the value, we use a function called insert

{% code overflow="wrap" lineNumbers="true" %}
```python
fruits.insert(0,'orange') #bigO notation //O(n) since it has to iterate through the data and push values forward
fruits
```
{% endcode %}

As you see above adding a value to the beggining of a python list is a procedure that has high time complexity. We can use the deque method in python to do this efficiently. The steps to deque the list and put it back together involves multiple steps however has a time complexity of O(1) hence is more scalable.

{% code overflow="wrap" lineNumbers="true" %}
```python
from collections import deque
fruits = deque(fruits)
fruits.appendleft('tomato')
fruits # resulting object: deque(['tomato', 'orange', 'apple', 'mango', 'banana'])
fruits = list(fruits)
fruits # resulting list: ['tomato', 'orange', 'apple', 'mango', 'banana']
```
{% endcode %}

Strings can also be assumed to be lists in python, rather the best way to process a string is to make it a list and process it.
