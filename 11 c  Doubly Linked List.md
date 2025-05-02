### EX: 11.C Doubly Linked List (Traversal, Search and Delete)

### Aim: 
To Write a python program to traverse the elements in doubly linked list.

### Algorithm:

STEP 1: Start.

STEP 2: Create a node class and object of the node.

STEP 3: Create another class to use the node object.
STEP 4 : Traverse the list from start to last data element.

STEP 5 : Print the data.

STEP 6 : Stop.

### Program:
```
class Node:
          def    __ init__ (self, data):
               self.item = data
               self.nref = None
               self.pref = None

class DoublyLinkedList:
         def    __ init__ (self):
               self.start_node = None

          def insert_in_emptylist(self, data):
                 if self.start_node is None:
                    new_node = Node(data)
                    self.start_node = new_node
                  else:
                     print("list is not empty")


           def insert_at_start(self, data):
                   if self.start_node is None:
                           new_node = Node(data)
                           self.start_node = new_node
                            print("node inserted")
                            return
new_node = Node(data)
new_node.nref = self.start_node
self.start_node.pref = new_node
self.start_node = new_node

def insert_at_end(self, data):
          if self.start_node is None:
                new_node = Node(data)
                self.start_node = new_node return
           n = self.start_node
         while n.nref is not None:
                 n = n.nref
                 new_node = Node(data)
                 n.nref = new_node
                new_node.pref = n

def traverse_list(self):
         if self.start_node is None:
              print("List has no element")
              return
          else:
              n = self.start_node
         while n is not None:
                   print(n.item, " ")
                   n = n.nref
new_linked_list = DoublyLinkedList()
new_linked_list.insert_in_emptylist(50)
new_linked_list.insert_at_start(10)
new_linked_list.insert_at_start(5)
new_linked_list.insert_at_start(18)
new_linked_list.insert_at_end(29)
new_linked_list.insert_at_end(39)
new_linked_list.insert_at_end(49)
new_linked_list.traverse_list()
```
### Output:
![image](https://github.com/user-attachments/assets/151c84f1-3971-46a7-a040-bed7bde5df09)

### Result: Thus, the given program is implemented and executed successfully.
 


