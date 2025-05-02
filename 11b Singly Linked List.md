### EX: 11.b Singly Linked List (Insertion and all operation)
Reg no: 212223020021
Name: Ranjith P

### Aim:
To Write a python program to add new element at the start of the list.


### Algorithm:

STEP 1: Start.

STEP 2: Create a node class and object of the node.

STEP 3: Create another class to use the node object.

STEP 4 : The new node is always added before the head of the given Linked List. And newly added node becomes the new head of the Linked List.

STEP 5 : Print the result.

STEP 6 : Stop.

### Program:
```
class Node:
            def     __init__ (self, data):
                  self.data = data
                  self.next = None

class LinkedList:
            def      __init__ (self):
                      self.head = None

            def push_front(self, newElement):
                    newnode = Node(newElement)
                    newnode.next=self.head
                    self.head = newnode
 
              def PrintList(self):
                     temp = self.head
                     if(temp != None):
           
                           print("The list contains:", end=" ")
                           while (temp != None):
                                print(temp.data, end=" ")
                                temp = temp.next
                                print()
                            else:
                                print("The list is empty.")


MyList = LinkedList()
MyList.push_front(10)
MyList.push_front(20)
MyList.push_front(30)
MyList.PrintList()
```
### Output:
![image](https://github.com/user-attachments/assets/4dae3c02-c85a-4294-9c03-294102d7fd9c)



### Result: 
Thus, the given program is implemented and executed successfully .
 


