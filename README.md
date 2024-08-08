# Learning Java

Welcome to my Java learning repository! This repository contains my notes, code examples, and exercises as I progress through learning Java. I hope you find it useful, whether you are also learning Java or just looking for some reference material.

1.Map in Java
2.Create List like vector with Values
3.Reference passing Variable

#1.Map in Java
```java
/*Directly Adding Values in Mapp*/
mappName.compute( val , (k,v) -> (v==null) ? 1 : v+1);
/*Traversing in  Mapp*/
for(Map.Entry<Integer,Integer>iterator : mappName.entrySet() ){
    iterator.getKey();
    iterator.getValue();
}
```

#2.Create List like vector with Values
```java
List<Integer> list = new ArrayList<>(Arrays.asList(1, 2));
```
#3.Reference passing Variable
```java
class wrapper{
    int value;
    wrapper(int value){
        this.value=value;
    }
}
wrapper a=new wrapper(0);
```
