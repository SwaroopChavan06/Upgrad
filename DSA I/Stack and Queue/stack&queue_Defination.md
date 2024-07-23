*Stack*

Stacks and queues are linear data structures that follow a particular order to add or remove entities.
1. A Stack is a list of element in which as element may be inserted or deleted only at one end, called TOP os the stack.
2. Best example is like the dinner plates in the wedding ceremony.

Example:

import java.util.Stack;
public class StackExample {
    public static void main(String[] args) {
        // Create a stack
        Stack<Integer> stack = new Stack<>();
        // Push an element onto the stack
        int element = 42;
        stack.push(element);
        // Pop the top element from the stack
        int topElement = stack.pop();
        System.out.println("Popped element: " + topElement);
        // Peek at the top element of the stack
        int peekElement = stack.peek();
        System.out.println("Top element: " + peekElement);
        // Check if the stack is empty
        boolean isEmpty = stack.isEmpty();
        System.out.println("Is stack empty? " + isEmpty);
        // Get the size of the stack
        int size = stack.size();
        System.out.println("Size of the stack: " + size);
    }
}

METHODS IN STACK CLASS
Several methods are available to modify and access stack elements in the Java Stack class. Among the most common methods are:

1. push(element): Adds a new element to the stack's top.

2. pop(): Removes and returns the topmost element in the stack.

3. peek(): Returns the topmost stack element without deleting it.

4. empty(): Returns a boolean result that determines if the stack is empty.

5. size(): Gives the stack's element count.



WHAT IS THE QUEUE?
A queue is a basic data structure representing a group of elements in a predetermined sequence. It adheres to the First-In-First-Out (FIFO) principle, which states that the first element added is also the first one taken out. And this is where the difference between stack and queue (in data structure terms) comes into the picture — while queue follows FIFO, stack follows LIFO data structure type.

In Java, we can use the Queue interface to represent a queue. Several classes implement the Queue interface in the Java Collections Framework, such as LinkedList and ArrayDeque.

Example:

import java.util.Queue;
import java.util.LinkedList;
public class QueueExample {
    public static void main(String[] args) {
        // Create a queue
        Queue<Integer> queue = new LinkedList<>();
        // Add an element to the queue
        int element = 42;
        queue.add(element);
        // Remove the element from the front of the queue
        int frontElement = queue.remove();
        System.out.println("Removed element: " + frontElement);
        // Peek at the element from the front of the queue
        int peekElement = queue.peek();
        System.out.println("Front element: " + peekElement);
        // Check if the queue is empty
        boolean isEmpty = queue.isEmpty();
        System.out.println("Is queue empty? " + isEmpty);
        // Get the size of the queue
        int size = queue.size();
        System.out.println("Size of the queue: " + size);
    }
}

METHODS OF QUEUE IN JAVA
Java's Queue interface offers several ways to interact with queues. Here are a few of the common methods:

1. add(element): Adds a piece to the rear of the queue.

2. remove(): Removes and returns the element at the front of the queue.

3. isEmpty(): Checks if the queue is empty and returns a boolean value.

4. size(): Returns the number of elements in the queue.


TYPES OF QUEUES IN JAVA
In Java, queues can be implemented using the java.util.Queue interface or its subclasses. Here are some common types of queues:

1. LinkedList Queue: It provides efficient insertion and removal of components at both ends of the queue

2. ArrayDeque Queue: It provides dynamic array-based operations for adding and removing elements.

3. Priority Queue: It orders elements based on their natural ordering or a custom comparator, allowing for removal based on priority.

4. Blocking Queue: Provides additional blocking and synchronization operations for thread safety.

5. Synchronous Queue: It enables simultaneous element passing by acting as a meeting point between two threads.


JAVA STACK AND QUEUE DIFFERENCE
Stack
Queue

1.

Follows the Last-In-First-Out (LIFO) principle.

Follows the First-In-First-Out (FIFO) principle.

2.

Elements are added and removed from the top (end) of the stack.

Elements are added at the rear (end) and removed from the front (start) of the queue.

3.

Examples of Stacks include function call stack and undo/redo functionality.

Examples in Queue include task scheduling and message passing.

4.

Only the top element is accessible and removable at a time.

Both the front and rear elements are accessible and removable.

5.

There is no easy way to access or eliminate middle-of-the-stack items.

When objects are in the middle of the line, it is difficult to access or remove them.


CONCLUSION
Stacks and queues are essential Java data structures with specific functions. Counting function calls, doing undos and redos, and evaluating expressions are popular uses for stacks. Queues, on the other hand, are helpful for sequential data management, message passing, breadth-first search, and job scheduling.

By understanding its features, applications, and implementations, you can use stack and queue in Java to arrange and modify data methodically and efficiently.


Wednesday -> Practice Session
Thursday -> Test- Mock test(Easy Level)
Friday -> Changes