Instructor: Jason Ku - MIT

A problem is a set of inputs that translates to a set of outputs

o   o
o   o
o   o
o   o
    o

An input can map to multiple sets of outputs

===
Pegionhole principle states that if n items(pegions) are placed into m containers (holes),
and n > m, then atleast one container must contain more than one item.

Eg. Problem: In a classroom of 365 students, are there any two students
with same birthday. Answer: Yes. n (students) > (days in a year)

===
Algorithm - set of instructions that given an input generates a correct output
f : I -> O

Birthday problem

Potential algorithms

1.
- Maintain a record
- Interview students in some order
-- Check if birthday in record
--- Return a pair
-- Add a new student to record
- Return None

Proof that its correct: Induction
For inductive proof, we need a Best Case, and an Inductive step

Inductive hypothesis: If first k students contain a match, algorithm returned
a match before interviewing student k+1

Base case: K = 0 : does the hypothesis hold? Yes
Assume IH true for k = k' { if k' contains match -> already returned by induction else if k' + 1 contains match, alg k'+1 checks agains all strudent birthdays }

Proof that its efficient
Efficiency means how fast and algorithm runs and how much memory it uses

Measuring efficient
Time O - upper bound, Omega - lower bound, Theta for both

Data structures
- Focuses on storing a large amount of data and the actions that could be
perfomed in the data