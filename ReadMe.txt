Greetings Yash!
Here's a brief explanation of the code that I've uploaded for the coding question given below:

Make a message scheduling program which takes in a number of messages sent by
users and schedules them in uniform distribution. For example take a list of users with
messages
A. 3
B. 2
C. 1
For the users A, B, and C, with message count 3, 2 and 1 respectively; The messages
can get scheduled in sequence ‘ABCABA’, note that there may be more than one
possible sequence or in some cases no perfect sequence..
The program should be able to parse a CSV of input messages and generate the
sequence of message schedule as uniformly distributed as possible.

So, first starting with the uniform distribution, the way I see in the example provided, we slice out the user when
the message count is zero.

So the process which I designed works like this:

First the count value is checked if it's greater than 0, we append that user to the sequence 

A: 3   B: 2   C: 1 --> ABC     (Iteration 1)
A: 2   B: 1   C: 0 --> ABCAB   (Iteration 2)
A: 1   B: 0   C: 0 --> ABCABA  (Iteration 3)

For this, the arrangement of the data frame was in descending order based on count.

