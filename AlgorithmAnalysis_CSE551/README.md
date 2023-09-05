# CSE 551 Notes


## Module 2
### Interval Scheduling
- Interval Scheduling
   Job j starts at s~j~ and finished at f~j~
   Two jobs are compatible if they don't overlap.
   Goal: find max subset of mutually compatible jobs

### Interval Partitioning

- Interval Partitioning

   Lecture j starts at s_j and finished at f_j
   Goal: to find the minimum number of classrooms (or servers) to schedule all the lectures (or jobs), so that no two occur at the same time in the same room.

   * Observations *
    
   The *depth* of a set of open intervals is the maximum number of intervals that contain any given time.

   Number of classrooms needed is $\ge$ depth.
