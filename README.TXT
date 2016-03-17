Big Data in Finance final exam, Part B1, calculating PI using MPI
=================================================================

The MPI program has several bugs. These bugs can be in the C code,
the makefile, or the PBS job file. Your task is to find these bugs,
fix them, compile and run the program, then share your results.

In this file, write any thoughts or comments that might help
improve your grade.

A hint to help you on your way. Remember that make uses tabs to indent
the commands below targets.

And, remember, to use Git you must first load Git:

  module load git
  
These may also be useful commands:

  module list
  
  module avail

Comment: there are 5 mistakes:
1. the main function within mpi.c doesnt have an return value
2. the makefile doesnt have indent
3. the formula should be divided by  4/(1+x*x) instead of x*x*x
4. the makefile should have source of mpi.c
5. if (myid = 0) should be myid == 0
