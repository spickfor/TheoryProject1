Team name: spickfor

Names of all team members: Seth PIckford

Link to github repository: https://github.com/spickfor/TheoryProject1.git

Which project options were attempted: Changed the algorithm in DumbSAT from BruteForcing to using Incremental Search

Approximately total time spent on project: 7 Hours

The language you used, and a list of libraries you invoked.  Python -- Used CSV and time libraries

How would a TA run your program (did you provide a script to run a test case?):  TA can Run the program by just Executing the file called Incremental_DumbSAT_spickfor.py

A brief description of the key data structures you used, and how the program functioned.
I will talk specifically about the Check function because that is the really the only thing  that was changed.  I used lists as the main data structure, with some embedding.  The function starts out with the assumption
that the wff is satisfiable. For each literal in the clause, it checks if it is satisfied, 1 for positive and 0 for negative.  If any clause is satisfied it marks it as satisfied and moves on.  The function uses a binary
counting method, which I didn't really remember until learning it for this project.  If a satifiable assigment is found it returns true, else false.

A discussion as to what test cases you added and why you decided to add them (what did they tell you about the correctness of your code). Where did the data come from? (course website, handcrafted, a data generator, other)
I didn't have any specific code run test cases.  I simply ran the original DumbSAT and then visually ran through and checked its outputs with those from my changed DumbSAT.  The data was all the same because it had the same
seed for the random generation meaning that the test data they created was the same.

An analysis of the results, such as if timings were called for, which plots showed what? What was the approximate complexity of your program?
The plot showed a large leap in the time to execute as they got more variable inputs.  In addition, the plot showed that the satifiable solutions were solved much quicker than the unsatisfiable ones.
The approximate comlexity of the program is 2^n * C * L where n is the number of variables, C is the clauses and L is the number of literals per clause.

A description of how you managed the code development and testing.
All the code development and testing was managed by me because I am the only one on the project.

Did you do any extra programs, or attempted any extra test cases
I originally attempted my own SAT solver but it wasn't giving me what I wanted so I switched to this because they organization of inputs and that stuff seemed to be the main issue.
