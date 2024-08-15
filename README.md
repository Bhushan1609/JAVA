# Learning Java

Welcome to my Java learning repository! This repository contains my notes, code examples, and exercises as I progress through learning Java.
I hope you find it useful, whether you are also learning Java or just looking for some reference material.


1.Map in Java<br>
2.Create List like vector with Values<br>
3.Reference passing Variable<br>
4.Queue And Priority Queue<br>
5.Pair in Java


# 1.Map in Java
```java
/*Directly Adding Values in Mapp*/
mappName.compute( val , (k,v) -> (v==null) ? 1 : v+1);
/*Traversing in  Mapp*/
for(Map.Entry<Integer,Integer>iterator : mappName.entrySet() ){
    iterator.getKey();
    iterator.getValue();
}
```

# 2.Create List like vector with Values
```java
List<Integer> list = new ArrayList<>(Arrays.asList(1, 2));
```
# 3.Reference passing Variable
```java
class wrapper{
    int value;
    wrapper(int value){
        this.value=value;
    }
}
wrapper a=new wrapper(0);
```

# 4.Queue And Priority Queue

```java
import java.util.Queue;
import java.util.LinkedList;

Queue<Integer> queue = new LinkedList<>();

queue.add(element);

int size = queue.size();
System.out.println("Queue size: " + size);

Integer frontElement = queue.peek();
System.out.println("Front element: " + frontElement);

Integer removedElement = queue.poll();
System.out.println("Removed element: " + removedElement);


import java.util.PriorityQueue;

PriorityQueue<Integer> priorityQueue = new PriorityQueue<>();

priorityQueue.add(element);

int size = priorityQueue.size();
System.out.println("PriorityQueue size: " + size);

Integer frontElement = priorityQueue.peek();
System.out.println("Front element: " + frontElement);

Integer removedElement = priorityQueue.poll();
System.out.println("Removed element: " + removedElement);
```

# 5.Pair in Java
Declararion 
pair<Integer , String> a = new pair<Integer ,String>(16 , "Bhushan");

System.out.println(a.fi());

System.out.println(a.se());

```java
public class pair<T, U> {
    private T first;
    private U second;

    public pair(T first, U second) {
        this.first = first;
        this.second = second;
    }

    public T fi() {
        return first;
    }

    public U se() {
        return second;
    }

    public void setFirst(T first) {
        this.first = first;
    }

    public void setSecond(U second) {
        this.second = second;
    }
}
```
