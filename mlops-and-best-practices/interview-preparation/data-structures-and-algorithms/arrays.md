# Arrays

An array is one of the easiest storage of data where data is stored in contiguous memory locations. These memory locations are known as the index of the array. These indexes can be used to reference or retrieve a value stored in the array. An array can be a one dimensional structure or a multidimensional structure

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption><p>image courtesy:<a href="https://www.c-sharpcorner.com/article/array-in-python/">https://www.c-sharpcorner.com/article/array-in-python/</a></p></figcaption></figure>

Python does not have a native array data structure but a 'list' is the equivalent data structure. A single list data structure can store data of different data types.

The numpy package enables Python to have 1d, 2d arrays which can be used for computation.

The equivalent data structure in R is a vector. R also has a list data type which like it's python equivalent can house multiple data types and data structures within it

{% code title="Create_n_append_list.py" lineNumbers="true" %}
```python
fruits = ['apple','mango','banana']
fruits.append('orange')
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
