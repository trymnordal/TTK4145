# Exercise 9


**Task 1:**
  1. We assign priorities to tasks because some tasks are more urgent or important than other.
  
  2. For a scheduler to be usable in real-time systems all deadlines have to be met at the right time and the scheduling have to be predictable.
  
**Task 2:**
  1. Without priority inheritance:
  
|Task|0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|
|----|-|-|-|-|-|-|-|-|-|-|--|--|--|--|--|
| a  | | | | |E| | | | | |  |Q |V |E |  |
| b  | | |E|V| |V|E|E|E| |  |  |  |  |  |
| c  |E|Q| | | | | | | |Q|Q |  |  |  |E |

  2. With priority inheritance:
  
|Task|0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|
|----|-|-|-|-|-|-|-|-|-|-|--|--|--|--|--|
| a  | | | | |E| | |Q| |V|E |  |  |  |  |
| b  | | |E|V| | | | |V| |  |E |E |E |  |
| c  |E|Q| | | |Q|Q| | | |  |  |  |  |E |

**Task 3:**
  1. Priority inversion is when a high-priority task is waiting for shared resources from a low-priority task. Unbounded priority inversion is when a task prevents the low-priority from releasing a shared resource, and the high-priority task ands up waiting forever.
  
  2. Priority inheritance does not prevent deadlocks.
  
**Task 4:**
  1. Assumptions:
    - Tasks are periodic with known time. Realistic.
    - There are a fixed set of tasks. May require workarounds.
    - Tasks are independent. Realistic.
    - There is no overhead. Depends on the system.
    - The deadline equal the period. Pretty realistic.
    
  2. U = 15/50 + 10/30 + 5/20 
