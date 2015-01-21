# NDKThreads

A thread is a mechanism enabling a single process to perform multiple tasks concurrently. Threads are
lightweight processes sharing the same memory and resources of the same parent process. A single
process can contain multiple threads executing in parallel. As part of the same process, threads can
communicate with each other and share data. Android supports threads in both Java and the native
code. In this chapter, you will be exploring different strategies and APIs that can be used for concurrent
programming pertaining to native code. The following key topics are covered in this chapter:
 Java vs. POSIX Threads
 Thread synchronization
 Controlling the thread lifecycle
 Thread priorities and scheduling strategies
 Interacting with Java from within native threads




Before going into the details of having multithreading in native code, you will create a simple
example application that will act as a testbed. The example application will provide the following:
 An Android application project with native code support.
 A simple GUI to define the number of threads, the number of iterations per
worker, a button to start threads, and a text view showing the progress
messages from the native workers during runtime.
 A native worker function mimicking a long-lasting task.
While working through the chapter, you will expand this example application to demonstrate different
techniques and APIs pertaining to multithreading in native code.
