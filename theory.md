Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 > Concurrency is only the illusion of simultaneity. The tasks are processed one after the other, respectively it is switching between the tasks. Parallelism is about doing more than one task at the same time to increasing the speed.
 
 ### Why have machines become increasingly multicore in the past decade?
 > Increaing the clock speed of processors caused some problems. So for increaing the speed of machines mulicore systemes became necessary. 
 . 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > To solve more than one problem at the same time and to work at different tasks. 
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Harder, because the programmer must look after the variables and their accesses in programs. So a system to handle this is necessary.
 
 ### What is the conceptual difference between threads and processes?
 > Processes do not share memory, threads do it.
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > Fibers (sometimes User Thread) are Threads inside of Threads. It's easy to switch between theese fibers, because they are not on the Kernel-Level, the OS doesn't know about theri existence. Because of that, the scheduling has to be done inside the programm. There is only one OS scheduler for handling the Threads, possibily more for handling the fibers.
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 >A goroutine is a lightweight thread/ fiber. Pthread creates a new Thread.
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > It sets the maximum number of CPUs that can work ´parallel.
 If n = 1; the result of the task in this exercise becomes corrred, because there occurs no simultaneously access on the data. 
 However the callulation is not parallel.



 
 
 
 
