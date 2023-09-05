# CSE 551 Notes


# Module 2
## Interval Scheduling
Job j starts at s~j~ and finished at f~j~

Two jobs are compatible if they don't overlap.

Goal: find max subset of mutually compatible jobs

There are four different aspects of the jobs that we can consider, 
* ~~Earliest Start Time~~
* Earliest Finish Time
* ~~Shortest Interval~~
* ~~Fewest Conflicts~~

Those three above break with greedy method, as shown below:
![greedy breaks for scheduling](./images/IS_greedy_breaks.png "Greedy Breaks for Interval Scheduling")

We can solve this by ordering jobs by finish times first so that f1 $\lt$ f2 $\lt$ f3 and so on..

implementation:

![finish time implementation](./images/finish_impl.png "Greedy Implementation: Finish Times")

It says O(n log n) time, because though the algorithm itself only take n time, we have to sort the finish times first, and best case of sorting is always log n.

## Interval Partitioning

Lecture j starts at s_j and finished at f_j, and the **goal** is to find the **minimum number of classrooms to schedule all lectures, so that no two occur at same time in same room.**



Goal: to find the minimum number of classrooms (or servers) to schedule all the lectures (or jobs), so that no two occur at the same time in the same room.

![bad intervals](./images/badints.png)

into this:

![good intervals](./images/goodints.png)

   * Observations *
    
   The *depth* of a set of open intervals is the maximum number of intervals that contain any given time.

   Number of classrooms needed is $\ge$ depth.
