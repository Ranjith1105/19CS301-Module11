# 19CS301-Module11
### EX: 11.a Singly Linked List (Traversal, Search and Delete)

### Aim: 
Write a function to traverse the linked list and display it in the following format.

### Algorithm:

STEP 1: Start.

STEP 2: Create a node class and object of the node.

STEP 3: Create another class to use the node object.

STEP 4 : Using data traversing traverse from first to last data element .

STEP 5 : Print the data.

STEP 6 : Stop.

### Program:
```
class Node:
      def     init (self, data=None):
            self.data = data
            self.next = None


class SLinkedList:
       def      init (self):
             self.head = None

       def listprint(self):
             printval = self.head
             while printval is not None:
                    print(printval.data)
                    printval = printval.next

 list = SLinkedList()
list.head = Node("Mon")
e2 = Node("Tue")
e3 = Node("Wed")

# Link first Node to second node list.head.next = e2

# Link second Node to third node e2.next = e3

list.listprint()

```
### Output:
![image](https://github.com/user-attachments/assets/f7547c51-0a61-45c2-93da-48fbb60de473)


### Result: Thus, the given program is implemented and executed successfully .
 


