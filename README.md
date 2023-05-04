Download Link: https://assignmentchef.com/product/solved-csc332-task4-simple-command-interpreter
<br>
<h1>PART 1: Simple Command Interpreter</h1>

Recall: In Task 3, we worked with <sup>exec() </sup>​ system calls for specific commands such as ​ <sup>date</sup><sup>​ </sup>​, and <sup>ls</sup>​ .​

Write a special simple command interpreter that takes a command and its arguments. This inter- preter is a program where the main process creates a child process to execute the command using exec() family​ functions. After executing the command, it asks for a new command input (i.e., parent

wait for child). The interpreter program will get terminated when the user enters <sup>quit</sup>​ .​

<h1>PART 2: Average Grade Calculator</h1>

There are 10 students enrolled in a course. The course covers x number of chapters from a textbook (x &gt;​ 1).​     In each chapter y number of homework(s) are assigned (y ≥​ 1).​   The average grade for each homework in all the chapters need to be found out.

To solve this, write a program that has the main process as Director process, which reads a file containing grades of all homework of all chapters and creates x number of Manager processes. Each Manager process will take care of solving a chapter. Each manager process will create y number of Worker processes and pass one homework to each of them and they calculate and print the average. The input file should contain the data according to the value of x and y. For example, the input text file and the process tree for x =​ 2​ and y =​ 2​ will look like the following:







The Director process is responsible for opening and closing the input text file. It stores the values in a two dimensional integer array with 10 rows. You may need to use the following C functions (in addition to the necessary file &amp; process management system calls): <sup>fopen()</sup>​ ,​ <sup>fscanf()</sup>​ ,​ <sup>fseek()</sup>​ ,​ fclose().​