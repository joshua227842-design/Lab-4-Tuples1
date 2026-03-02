# Lab-4-Tuples1
Lab 4 – Tuples
##1- Exercising tuples

```python
a = input("Enter first value: ")
b = input("Enter second value: ")
c = input("Enter third value: ")
d = input("Enter fourth value: ")
e = input("Enter fifth value: ")

my_tuple = (a, b, c, d, e)

print("Tuple created:", my_tuple)
print("Data type:", type(my_tuple))
```
How do you assign a single element in a tuple?

You cannot assign or change a single element in a tuple because tuples are immutableif you try something like this:
```python
x = (1, 2, 3)
x[0] = 10
```
It will give an error because tuple elements cannot be modified after creation.

2 ## Count the repeated integers and print the result

```python
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)

for num in set(my_tuple):
    count = my_tuple.count(num)
    print("Number", num, "appears", count, "times")
    ```
    This prints how many times each number appears in the tuple.

   ## 1D:

   ```python
my_tuple = (1,2,3,4,3,2,1,2,3,5,4,3,2,1)

print("Original tuple id:", id(my_tuple))

my_tuple = my_tuple + my_tuple

print("New tuple id after concatenation:", id(my_tuple))
print("New tuple:", my_tuple)
   
    ```

    The memory address id changes after concatenatio, this proves it created a new tuple instead of modifying the old one.
