# 42philosophers

## I never thought philosophy would be so deadly

![](media/philo.gif)

This project simulates the classic **Dining Philosophers** problem. In this scenario, several philosophers are seated around a dining table. They alternate between **thinking**, **eating**, and **sleeping**, but there is a limited number of forks placed between them. To eat, a philosopher must acquire both forks adjacent to their seat. The objective is to design the program to ensure that no philosopher starves due to a lack of access to forks.

More information about the problem can be found ***[here](https://en.wikipedia.org/wiki/Dining_philosophers_problem)***.

The challenge is to implement a solution that avoids **deadlocks** and ensures proper synchronization when philosophers access the shared forks, ensuring that none of our thinkers meet an untimely demise. This project provides a **multithreaded** approach to solving the **Dining Philosophers** problem by leveraging **mutex locks** to manage resource access efficiently and safely.

This was my seventh project in **Hive Helsinki** and it mainly introduced the concept of **Concurrency** in the way of **Multithreading** and **Multiprocessing**.
I actually completed this task in mid **2023**, but I wanted to redo the commit history and make some minor changes.

## 📖 Topics
  - Multithreading
  - Multiprocessing
  - Mutex locks
  - Semaphores
  - Dataraces
  - Deadlocks
  - Memory management
  - Unit testing

## 🛠️ Langs/Tools
  - C
  - Makefile

## 🦉 Getting started

  1. ```git clone https://github.com/kenlies/42philosophers```
  2. ```cd 42philosophers```
  3. ```cd philo``` or ```cd philo_bonus``` featuring the process solution
  4. ```make```

  Usage: ```./philo <philosophers> <time_to_die> <time_to_eat> <time_to_sleep> <[number_of_times_each_philosopher_must_eat]>```, the last argument being optional
  
  Example: ```./philo 5 410 100 100```, where the simulation stops when a philosopher dies

  Example: ```./philo 5 410 100 100 10```, where the simulation stops when all philosophers have eaten atleast 10 times

## 💸 Bonus section

Introduces **processes** and **semaphores** to the **Dining Philosophers** problem. Instead of individual forks placed between philosophers, a central pile of forks is placed on the table. This fork pile is represented by a **semaphore**, which manages access to the shared resource. Each philosopher is implemented as a separate **process**, ensuring concurrent execution while the semaphore ensures proper synchronization and prevents resource conflicts. Instead of **multithreading**, use **multiprocessing**.

## 🔨 To improve

The code execution flow isn't clear in some places and code modularity can be improved.
