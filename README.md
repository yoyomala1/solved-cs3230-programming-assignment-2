Download Link: https://assignmentchef.com/product/solved-cs3230-programming-assignment-2
<br>
Space is very limited in NUS and assigning lectures to lecture halls efficiently is a pertinent problem. Due to the busy schedules of the lecturers, most of them can only give the lectures at a fixed time slot in the week.

Since there is a limited number of lecture halls, the lectures should be assigned such that the halls are well utilised. Hence, given all the lecture timings, you want to know what is the minimum number of lecture halls needed so that all the lectures can take place at their time slot.

However, there may not be enough lecture halls in the school to fit all the lectures, so you also want to know for a given fixed number of lecture halls, what is the minimum number of lectures that need to be cancelled so that all the lectures can take place at their time slot.

<h1>Details</h1>

There are a total of <em>N </em>lectures that need to be conducted labelled 0 to <em>N </em>− 1 and each lecture must be given at a fixed time slot but there are only <em>L </em>lecture halls. For convenience, the time slot for lecture <em>i </em>starts at <em>start<sub>i </sub></em>time units and ends at <em>end<sub>i </sub></em>time units where <em>start<sub>i </sub>&lt; end<sub>i</sub></em>. Another lecture can start right after a lecture ends in the same lecture hall which means if one lecture ends at 5 time units and another lecture starts at 5 time units, both can use the same lecture hall.

Given these limitations, you need to calculate 2 values.

<ol>

 <li>If you don’t want to cancel any lectures, what is the minimum number of lecture halls thatneed to be booked such that all the lectures can be scheduled in a way where no 2 lectures are in the same lecture hall at the same time.</li>

 <li>If there are only <em>L </em>lecture halls, what is the minimum number of lectures that need to be cancelled so that all the lectures can take place at their time slot using only <em>L </em>lecture halls.</li>

</ol>

<h1>Implementation</h1>

You need to implement 2 functions to calculate the 2 values described above. The functions will take in 4 parameters:

<ul>

 <li>N – The number of lectures</li>

 <li>L – The number of lecture halls</li>

 <li>start – A list of <em>N </em>integers integers where start[i] is <em>start<sub>i </sub></em>as described above</li>

 <li>end – A list of <em>N </em>integers where end[i] is <em>end<sub>i </sub></em>as described above</li>

</ul>

You are allowed to submit in either Java or C++11. Templates for both languages have been provided in the IVLE Workbin in the same folder as this task statement. The templates have implemented the I/O routines for you so you are strongly encouraged to use them. In addition, you are allowed to add other functions into your program to modularise your code but you must submit only ONE source file.

For testing purposes, the program will read in the parameters listed above from standard input in the exact order listed above for each test case with each parameter on a separate line. There can be multiple test cases within one run and the first integer gives the number of test cases. The program will output one line for each test case, which contains one integer that is the answer for that test case.

For example, if there are 5 lectures and 2 lecture halls where start = [3, 5, 4, 2, 1] and end = [4, 6, 7, 5, 5] then the input it expects will look like this:

1

5

2

<ul>

 <li>5 4 2 1</li>

 <li>6 7 5 5</li>

</ul>

<h1>Example</h1>

For the example given above, if no lectures can be cancelled then the minimum number of lecture halls required is 3. The first lecture hall would host lectures 4 and 1 in that order while the second lecture hall would host lectures 0 and 2 in that order and the third lecture hall would host lecture

<ol start="3">

 <li>The scheduling will look like the following diagram:</li>

</ol>

However, since area is only 2 lecture halls, the minimum number of lectures that need to be cancelled is 1. Specifically, cancelling lecture 3 will allow all the remaining lectures to fit into 2 lecture halls.