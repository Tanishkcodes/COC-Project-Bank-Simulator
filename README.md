**---------------------------------------------------COC-Project-Bank Queue-Simulator------------------------------------------------**


## 📖 Project Description:-
---------------------------
The **Bank Queue (Poisson) Simulator** is a C program that models how customers arrive and are served at a bank throughout a typical 8-hour working day (480 minutes).  
The simulation helps the bank’s management analyze customer wait times and decide whether hiring additional tellers is necessary.

This program uses the **Poisson distribution** to realistically simulate customer arrivals and **linked lists with dynamic memory** (`malloc()` / `free()`) to manage the queue efficiently.  
At the end of the simulation, the program calculates key statistical metrics — **mean, median, mode, standard deviation**, and **Longest wait time** — to provide actionable insights.


## Concepts Used:- 
-----------------
# 💻 C Programming Concepts
- `struct` (to represent customers and queue)
- Dynamic Memory Management: `malloc()`, `free()`
- Pointers and Linked Lists
- Modular Functions (`customer_arrives()`, `serve_customer()`, etc.)
- Control Structures: {`for`, `if/else`, `while`}
- Random Number Generation (`rand()`, `srand()`)
- Math Library (`<math.h>`)

# 📊 Mathematical Concepts
- **Poisson Distribution** (models customer arrivals per minute)
- **Central Tendencies**:
  - Mean
  - Median
  - Mode
- **Standard Deviation** (measure of variation in wait times)
- **Data Analysis** of customer waiting patterns


## How to Compile:-
Use the following commands to compile and execute the program:

[gcc bank_queue.c -o bank_queue -lm]
[./bank_queue]


## How to Run:-
After Executing, the terminal will show as:-

**Example Terminal Session:-**
$ gcc bank_queue.c -o bank_queue -lm
$ ./bank_queue

======================================
    BANK QUEUE SIMULATOR (8-hour day)

Enter the average number of customers arriving per minute (λ): 1
Enter the number of tellers: 3
Enter the service time per customer (min.): 3

Simulating 8-hour day (480 minutes)...
== WAIT TIME ANALYSIS ==
Mean wait time: 16.30 minutes
Median wait time: 18.00 minutes
Mode wait time: 25 minutes
Standard Deviation: 8.38 minutes
Longest wait time: 31 minutes
========================================

RECOMMENDATION: Average wait time exceeds 10 minutes.
Consider hiring additional tellers.





