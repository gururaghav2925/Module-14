# Exp.No:39  
## DEQUE - INSERTION

---

### AIM  
To write a Python program to insert elements at REAR END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Initialize an empty deque.  
3. Start an infinite loop using `while True`.  
4. In each iteration, take input from the user.  
5. If the input is an empty string, break the loop.  
6. If the input is not empty, convert it to an integer and append it to the deque.  
7. After the loop ends, append the values `14` and `15` to the deque.  
8. Print the message `"The deque after appending at right is :"`.  
9. Print the contents of the deque.  

---

### PROGRAM  

```python
import collections
  
n1=int(input())
n2=int(input())
n3=int(input())
# initializing deque
de = collections.deque([n1,n2,n3])

# inserts 14,15 at the rear of deque
de.append(14)

de.append(15)
# printing modified deque
print ("The deque after appending is : ")
print (de)

```

### OUTPUT

![image](https://github.com/user-attachments/assets/9ba6aa06-51a4-4315-a95b-602c90c02d99)



### RESULT

The deque contains the elements inserted at the rear end: The deque after appending at right is : deque([11, 12, 13, 14, 15])
