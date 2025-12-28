# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
~~~
import math
class cse:
    def mech(self,r):
        print("Area of circle:",round(math.pi*r**2,2))

r = int(input()) 
a = cse()
a.mech(r)
~~~
## Output
<img width="663" height="201" alt="Screenshot 2025-10-20 144718" src="https://github.com/user-attachments/assets/c747b4d4-1cef-4573-9392-362ef5d65563" />

## Result
Thus , the program has been executed succesfully.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
~~~
dict1 = eval(input())
dict2 = eval(input())
def merge(d1, d2):
    merged_dict = {**d1, **d2}
    return merged_dict
result = merge(dict1, dict2)
print(result)


~~~

## Output
<img width="1050" height="251" alt="Screenshot 2025-10-20 152122" src="https://github.com/user-attachments/assets/087d406c-6d4b-47af-a825-e3f03f80f01b" /><img width="676" height="251" alt="Screenshot 2025-10-20 152138" src="https://github.com/user-attachments/assets/a84c5b9d-3998-4ef0-a952-d74b7616770e" />


## Result
Thus , the program has been executed succesfully.

# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
~~~
my_dict = {2: 56, 1: 2, 5: 12, 4: 24, 6: 18, 3: 323}

sorted_by_keys = dict(sorted(my_dict.items()))
sorted_by_values = dict(sorted(my_dict.items(), key=lambda item: item[1]))
print("Original dictionary:", my_dict)
print("Dictionary sorted by keys:", sorted_by_keys)
print("Dictionary sorted by values:", sorted_by_values)
~~~
## Sample Output
<img width="758" height="166" alt="Screenshot 2025-10-20 153400" src="https://github.com/user-attachments/assets/5f01db86-97da-4661-9d15-a7d7603003ce" />

## Result
Thus , the program has been executed succesfully.

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
~~~
list1 = [5, 10, 20,]

try:
    print(list1[5])
except IndexError:
    print("You're out of list range")

~~~

## Output
![WhatsApp Image 2025-10-20 at 15 09 26_aed4cc27](https://github.com/user-attachments/assets/fae84b30-133b-46e7-9d94-417d7317d390)

## Result
Thus , the program has been executed succesfully.

# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
~~~
def count_lines_not_starting_with_T(filename):
    count = 0  
    with open(filename, "r") as file:
        for line in file:
            if not line.startswith('T'):
                count += 1
    return count

result = count_lines_not_starting_with_T("story.txt")
print("Number of lines that not starting with 'T':", result)


~~~

## Output
![WhatsApp Image 2025-10-20 at 15 00 09_458980ee](https://github.com/user-attachments/assets/f2d64c74-9918-46af-ac16-77644294a679)

## Result
Thus , the program has been executed succesfully.
