### PriorityQueue and LinkedList
    most important classes for queue in java
    NOT thread safe, PriorityBlockingQueue is thread safe

```public interface Queue extends Collection```
```Java
// Obj is the type of the object to be stored in Queue 
Queue<Obj> queue = new PriorityQueue<Obj> ();
```
#### Queue interface follow FIFO order, some of its important methods are - 

1. add(element) - if full throw exception
2. offer(element) - if full returns false
3. remove() - remove element form front, if empty throw error
4. poll() - remove, if empty return null
5. element() - returns element in front, if empty throw exception
6. peek() - returns element in front, if empty returns null.

#### classes implementing queue interface - 

1. LinkedList - order is maintained
2. ArrayDequeue 
3. PriorityQueue - insertion order based on priority, default is ascending.
4. PriorityBlockingQueue - same as PriorityQueue but unbounded, blocking, thread safe.

#### iterating the queue
```java
// Java program to iterate elements
// to a Queue

import java.util.*;

public class GFG {

	public static void main(String args[])
	{
		Queue<String> pq = new PriorityQueue<>();

		pq.add("Geeks");
		pq.add("For");
		pq.add("Geeks");

		Iterator iterator = pq.iterator();

		while (iterator.hasNext()) {
			System.out.print(iterator.next() + " ");
		}
	}
}

```

# Must see methods in Queue
https://www.geeksforgeeks.org/queue-interface-java/

