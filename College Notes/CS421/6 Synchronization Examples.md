Only one thread can do its critical section of code at a time.

Bounded buffer problem
n buffers, each can hold one item
Semaphore mutex initialized to the value 1
Semaphore full initialized to the value 0
Semaphore empty initialized to the value n

