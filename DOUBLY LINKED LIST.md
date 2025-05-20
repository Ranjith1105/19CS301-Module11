### 11 e. SEB : DOUBLY LINKED LIST (FORWARD AND REVERSE DIRECTION)

### Aim:
     To implement a doubly linked list in Python and traverse it in both forward and reverse directions.

###  Algorithm:

Step 1: Define the Node class
Create a node with three attributes:

     data: stores the element value.

     next: points to the next node.

     prev: points to the previous node.

Step 2: Define the DoublyLinkedList class
Initialize the list with head = None.

Step 3: Define push(new_data)
Create a new node with new_data.

Set new_node.next to current head.

If the head exists, set head.prev to new_node.

Set the head to the new node.

Step 4: Define append(new_data)
Create a new node with new_data.

If the list is empty, set head to the new node and return.

Otherwise, traverse to the last node of the list.

Set last.next to the new node.

Set new_node.prev to the last node.

Step 5: Define printList(node)
Forward Traversal:

Starting from the head, print each node’s data until the end (node.next is None).

Reverse Traversal:

After reaching the last node in the forward loop, print data in reverse by moving using node.prev.

Step 6: Main Program Execution
Create an object llist of class DoublyLinkedList.

Input elements from the user:

Use append() to add elements at the end.

Use push() to add elements at the beginning.

Call printList() with the head node to display the list:

First in forward direction.

Then in reverse direction.


### PROGRAM :
 Name: RANJITH . P
 Reg.no : 212223020021

 class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        self.prev = None
  
class DoublyLinkedList:
    def __init__(self):
        self.head = None
  
    def push(self, new_data):
        new_node = Node(new_data)
        new_node.next = self.head
        if self.head is not None:
            self.head.prev = new_node
        self.head = new_node
        
    def append(self, new_data):
        new_node = Node(new_data)
        if self.head is None:
            self.head = new_node
            return
        last = self.head
        while last.next:
            last = last.next
        last.next = new_node
        new_node.prev = last
        return
  
    def printList(self, node):
        print("\nTraversal in forward direction")
        while node:
            print(node.data)
            last = node
            node = node.next
        print("\nTraversal in reverse direction")
        while last:
            print(last.data)
            last = last.prev
  
llist = DoublyLinkedList()
a1 = int(input("Insert the element to add at the end\n"))
llist.append(a1)
p1 = int(input("Insert the element to add at the beginning\n"))
llist.push(p1)
p2 = int(input("Insert the element to add at the beginning\n"))
llist.push(p2)
a2 = int(input("Insert the element to add at the end\n"))
llist.append(a2)
print ("Created DLL is: ")
llist.printList(llist.head)

### OUTPUT:
![Screenshot 2025-05-20 222432](https://github.com/user-attachments/assets/822d91a2-10f4-4239-9ef2-4a282d3253e4)

### RESULT:
     The program is implmented and executed successfully
