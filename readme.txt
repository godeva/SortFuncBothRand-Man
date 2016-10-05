Program Description: 

In the “assig2” folder, there are 20 files/directories. Note: Objects files will not be included in this guide as all the descriptions would be simply compiled code from the corresponding code files.

NOTE: IF YOU WANT TO USE DOXYEGEN COMMAND "Make Docs", TAKE THE READ ME FILE OUT OF THE ZIP IN A SEPERATE DIRECTORY SO THAT DOXYGEN DOESN'T REGISTER readme.txt syntax as file members online. Thanks! 

at: This file is an executable that prints two types of consecutive numbers from 0 to 9. It first prints integer data type consecutive numbers line by line. Then it prints double data type consecutive numbers line by line. You can run the executable by typing ./at on the command line. 

at.c: This is human readable code file for at. All the code from this file was compiled to create the executable.

at2: This file is an executable that takes 10 number inputed by the user in the command line and prints them line by line. It then takes those same numbers and sorts them in ascending order and then prints out the sorted array line by line. You can run the executable by typing ./at2 and entering a maximum of 10 numbers on the command line. 

at2.c: This is human readable code file for at. All the code from this file was compiled to create the executable.

at3: This file is an executable that prints out random numbers line by line. It then takes those random numbers and prints them in ascending order. You can run the executable by typing ./at3 on the command line. 

at3.c: This is human readable code file for at3. All the code from this file was compiled to create the executable.

print_arrays.c: This is the code file that runs the functions print_int_array, print_double_array, and readToIntArray. Function print_int_array stores integer data type numbers in an array, function print_double_array stores double data type number in an array, and function readToIntArray stores numbers from the command line into an array. In order to calculate values, this file must be linked with at1, at2, at3 and print_arrays.h.

print_arrays.h: This is the header file and contains the function prototype. This requires the program print_arrays.c to work since it’s needed when compiling a source file that uses a function from a different file. 

sortingFunction.c: This is the code file that runs the functions sortingFunction, numGenerator, and randomArray. Function sortingFunction  sorts numbers in ascending order, function numGenerator generates a random integer from zero to some specified maximum inclusive (In this file it's set to 100 max), and function randomArray creates a list of random numbers (In this file it's 10 numbers) using function numGenerator for each number. In order to calculate values, this file must be linked with at1, at2, at3 and sortingFunction.h.

sortingFunction.h: This is the header file and contains the function prototype. This requires the program sortingFunction.c to work since it’s needed when compiling a source file that uses a function from a different file. 

Makefile: Makefile takes all of the code files and compiles them so that they are ready to be used for the computer to read. In the contents of the file, makefile shows the files that that are told to be compiled and link together and cleaned. This include the files at.c, at2.c, at3.c, sortingFunction.c, and print_arrays.c. To activate the contents of Makefile, type “make” on the command line which will allow the code files to be compiled to run the program. If you wish to un-compile the code files which removes the .o file, type “make clean” on the command prompt.

How to compile: 

Unzip the tar file and type "make" in the command prompt inside the assign2 directory. This will compile all the files in the folder as well as link the header files with the same named code file. If you wish to uncompile, type "make clean" and it will delete all the object files and leave you with the code files, header files, Doxyfile, and makefile.

Test Data:

at: 

//Check if the program runs


Input: ./at


What to Expect: 

0
1
2
3
4
5
6
7
8
9
0.000000
1.000000
2.000000
3.000000
4.000000
5.000000
6.000000
7.000000
8.000000
9.000000

_________________________________________________________

at2: 

//Check if no numbers are given

Input: ./at2

What to Expect:

Must enter a number on the command line!



//Check if at2 works

Input: ./at2 2 3 45 2 7 68 42 5 0 9

What to Expect:

Original numbers!
2
3
45
2
7
68
42
5
0
9
Sorted numbers in ascending order!
0
2
2
3
5
7
9
42
45
68



//Check if at2 prompt message if numbers entered are more than array size

Input: ./at2 2 3 45 2 7 68 42 5 0 9 5 5 65 6 6 66 6 6

What to Expect:

This program can only test a max number of 10 numbers
Original numbers!
2
3
45
2
7
68
42
5
0
9
Sorted numbers in ascending order!
0
2
2
3
5
7
9
42
45
68

_________________________________________________________

at3: 

//Check if at3 works

Input: ./at3

What to Expect:

Original random numbers!
32
32
54
12
52
56
8
30
44
94
Sorted random numbers in ascending order!
8
12
30
32
32
44
52
54
56
94_______________________________________________________
