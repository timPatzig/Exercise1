The parallel threads have access to the same memory at the same time. That leads to one Thread reads the variable, while the other is writing. 
For expample, Thread A reads the data, then it calculates the result and writes it back. Meanwhile Thread B changed the value of the variable. So the result of B is ignored.
