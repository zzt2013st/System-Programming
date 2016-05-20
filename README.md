# System-Programming
Practice C pointers


This machine problem will be divided up into two pieces. In the first piece, you will be modifying functions originally with errors such that the outputs match the given output. In the second piece, you will need to write some code to call some ‘creatively defined’ functions so that those functions produce the desired output.


Part 1:
There are erroneous/unimplemented functions in part1-functions.c. Your task is to modify functions according to comment above each function such that the output of part1 looks exactly as follows:

== one() ==
3^2 + 4^2 = 25
10^2 + 10^2 = 200
== two() ==
20 not passed!
100 passed!
== three() ==
The value of p is: 4
== four() ==
The value is between zero and one.
The value is not between zero and one.
== five() ==
x and y are equal.
x and y are different.
== six() ==
4 == 4.000000
432 == 432.000000
== seven() ==
a is a letter.
a is not a letter.
== eight() ==
Hello
== nine() ==
The value of p is: 12.500000
== ten() ==
0 == 0?
== eleven() ==
Hello World!
== twelve() ==
0.000000 0.100000 0.200000 0.300000 0.400000 0.500000 0.600000 0.700000 0.800000 0.900000
== thirteen() ==
0 10 40 90 160 250 360 490 640 810
== fourteen() ==
orange and blue!
ORANGE and blue!
Orange and BLUE!
orange and blue!
== fifteen() ==
You passed in the value of one!
You passed in the value of two!
You passed in some other value!
== sixteen() ==
Hello
== seventeen() ==
The radius of the circle is: 17.500000.
The radius of the circle is: 10.000000.
== eighteen() ==
Result: 323
Result: 2499
== clear_bits() ==
170
0
171
0
20
0
== little finite automatons
5
4
6
7


##Part 2:
We have pre-uploaded some files to your mp0 svn directory, including part2-functions.c. Inside part2-functions.c, you will see twelve different functions, including first_step() (re-printed below).

void first_step(int value) {
  if (value == 81)
    printf("1: Illinois\n");
}
To complete Part 2, you must complete the program part2-main.c so that part2-main.c makes calls to all twelve functions in part2-functions.c such that they print their “Illinois” line. When running ./part2, your output should look exactly like:

1: Illinois
2: Illinois
3: Illinois
4: Illinois
5: Illinois
6: Illinois
7: Illinois
8: Illinois
9: Illinois
10: Illinois
11: Illinois
You should NOT edit the part2-functions.c file. In fact, when we grade your program, we will replace the part2-functions.c file with a new version of the file (and we’ll change the “Illinois” string so printing out “Illinois” in a for-loop will get you no credit).

Compile and Run
To compile the release version of the code run:

make clean
make
This will compile your code with some optimizations enabled, and will not include debugging information (if you use a debugger on the ‘release’ build, it will not be able to show you the original source code, or line numbers). Optimizations sometimes expose some bugs in your code that would not show up when no optimizations are enabled, but since optimizations tend to reorder your code while compiling, an optimized version of your code is not optimal for debugging.

You probably don’t need to worry about the different build types very much for this assignment, but the distinction will become more important on future assignments.

To compile your code in debug mode, run make debug instead of make

To run Part 1:

./part1
or

./part1-debug
To run Part 2:

./part2
or

./part2-debug
