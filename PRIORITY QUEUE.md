# Exp.No:37  
## PRIORITY QUEUE

---

### AIM  
To write a Python program for simple implementation of Priority Queue using Queue.

---

### ALGORITHM

1. Start the program.  
2. Define a class `PriorityQueue` with an initializer to create an empty list `queue`.  
3. Define the `__str__` method to return queue elements as a string separated by spaces.  
4. Define the `isEmpty()` method to check if the queue is empty.  
5. Define the `insert(data)` method to append the given data to the queue.  
6. Define the `delete()` method to:  
   - Initialize `max_val` as 0.  
   - Loop through the queue and find the index of the maximum value.  
   - Delete and return the element at that index.  
7. In the main code, take integer input `n` for number of elements.  
8. Loop `n` times to take input values and insert them into the priority queue.  
9. Print the contents of the queue.  
10. While the queue is not empty, call `delete()` and print each returned element.  
11. End the program.

---

### PROGRAM

```python


class PriorityQueue:
    def __init__(self):
        self.queue = []

    def insert(self, item, priority):
        self.queue.append((item, priority))

    def delete(self):
        if not self.queue:
            print("Queue is empty.")
            return None
        
        # Find the element with the highest priority (lowest number)
        min_priority_index = 0
        for i in range(1, len(self.queue)):
            if self.queue[i][1] < self.queue[min_priority_index][1]:
                min_priority_index = i
        
        item = self.queue.pop(min_priority_index)
        print(f"Deleted item: {item[0]} with priority {item[1]}")
        return item[0]

```

### OUTPUT

![431401244-6ad489c7-6a72-40a3-a535-a1364264be3e](https://github.com/user-attachments/assets/a342024b-b2f1-45b7-a458-81fa6a150e90)


### RESULT

The delete() function removes the element with the highest priority from the priority queue and displays it.
