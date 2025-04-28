# Exp.No:38  
## Deque - DELETION

---

### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

---

### PROGRAM  

```python

import collections
n1=input()
n2=input()
n3=input()
de=collections.deque([n1,n2,n3])
de.pop()
print(f"The deque after deleting at right is :\n{de}")
```

### OUTPUT

![image](https://github.com/user-attachments/assets/55f56c3e-35f6-4836-ad37-60248a2268aa)


### RESULT

The deque contains the elements deleted at the rear end: The deque after deleting at right is : deque(['p', 'y'])
