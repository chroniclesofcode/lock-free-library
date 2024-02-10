# lock-free-library

A library of lock-free high performance data structures in C++.

They are designed to be simple data structures which do what they are meant to 
do with simple interfaces. If you are looking for complex lock-free data structures
that have many functionalities, you can let me know and I will try to implement it
or you can look for another repo with the desired requirements.

Anything prefixed with 'ub' is noted as 'unbounded' - which means it is
implemented as a linked list and has flexible sizing. Anything not prefixed,
you can assume is bounded - so it is important to specify a starting size, and
the size cannot be changed once the data structure is created.

# How to use

It is a header only library - so just copy the contents of the 'include' folder
into your project, and you will be able to use it immediately. Inside src there
will be main functions for testing and benchmarks, however it is mainly for 
my own purposes: only the 'include' directory matters if you are looking to use
these data structures.

# How to run tests

To run the tests in the code:

`./run [FILENAME]`

e.g. to test the SPSC Queue, you would run

`./run spsc_queue`
