
Question 1: By default are django signals executed synchronously or asynchronously?

Ans: Django signals excutes synchronously, when the signal is send signal handlers called immediately. It can cause performance issues if the signal processing takes a long time, as it blocks the main execution flow.

Question 2: Do django signals run in the same thread as the caller?

Ans: By default django signals run in the same thread as the caller. That means the signal handler is executed in the same thread as the code that triggered the signal when it is been sent to receiver funtion.

Question 3: By default do django signals run in the same database transaction as the caller?

Ans: 
