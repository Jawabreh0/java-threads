# Java Threads

## Threads
1. A multithreaded program contains two or more parts that can run concurrently
2. Each part of such a program is called a thread, and each thread defines a separate path of
execution.
3. A thread is a single sequential flow of execution within a program.
i.e. a thread is a subset of process.
4. Thread is considered as “Light Weight Process” because it use less resource than process.
5. Threads share the address space of the process but process have their own address space.
6. JVM create the thread whose task is to define the main thread.
7. Threads may be executed either on a multi-processor machine, or (more common) in
simulated parallel on a single-processor machine on a time-sharing basis.

## Multithreading
1. Multithreading in java is a process of executing multiple threads simultaneously.
2. Thread is basically a lightweight sub-process, a smallest unit of processing.
Multiprocessing and multithreading, both are used to achieve multitasking.
3. But we use multithreading than multiprocessing because threads share a common
memory area.
4. Threads don’t allocate separate memory area so saves memory,
and context-switching between the threads takes less time than process.
5. Java Multithreading is mostly used in games, animation etc.

## Thread Creation

Two ways to create thread: 

1. Extending Thread Class: 

```java 
private class HelloThread{

public void run(){
System.out.println("Hello Thread");
}
public static void main(String args[]){
Thread t = new HelloThread();
t.start();
}
}
```
2. Implementing Runnable Interface:

```java 
private class HelloThread{

public void run(){
System.out.println("Hello Thread");
}
public static void main(String args[]){
Thread t = new Thread(new HelloThread());
t.start();
}
}
```







