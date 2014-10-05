project-3
=========

Eecs Project 3
hello 

/****************************************************************************
 *                                                                          *
 * NOTE: For every function                                                 *
 *       The last line should end with an 'endl'.                           *
 *       No blank lines should be printed at the beginning nor at the end.  *
 *                                                                          *
 * See project specification for sample output.                             *
 *                                                                          *
 ****************************************************************************/


/**
 Requires: rows must be > 0, cols must be > 0.
 Modifies: Nothing.
 Effects:  Prints a rectangle of *'s.

 Example:

printRectangle(3, 2);
cout << endl;
printRectangle(1, 3);
cout << endl;

**
**
**

***

 Note: the blank lines are printed by test1.cpp and
       there are no spaces at the end of lines.
 */
void printRectangle(int rows, int cols);


/**
 Requires: rows must be > 0, cols must be > 0, offset must be >= 0.
 Modifies: Nothing.
 Effects:  Prints a rectangle of *'s each indented by 'offset' spaces.

 Example:

printRectangle(3, 2, 4);
cout << endl;
printRectangle(1, 3, 2);
cout << endl;

    **
    **
    **

  ***

Note: the blank lines are printed by test1.cpp and
      there are no spaces at the end of lines.
 */
void printRectangle(int rows, int cols, int offset);


/**
 Requires: str will not contain any control characters, i.e.,
           NO: \n, \t, \b, etc. allowed.
 Modifies: Nothing.
 Effects:  Prints the string str within a rectangle of *'s.
           On the left, there is one space between the * and the
           1st letter of the str. Same for the right.
           If the string is empty, nothing should print.
 Example:

printStringInBox("Hello World!");
cout << endl;

****************
* Hello World! *
****************

 */
void printStringInBox(string str);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints a right triangle of stars.

 Example (no spaces at the end of lines):

printRight(3);
cout << endl;

*
**
***

 */
void printRight(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints a right triangle of stars separated by spaces.

 Example (no spaces at the end of lines):

printRightWithSpaces(3);
cout << endl;

*
* *
* * *

 */
void printRightWithSpaces(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints an isosceles triangle (pointing up).
 
 Example (no spaces at the end of lines):

printIsosceles(3);
cout << endl;

  *
 ***
*****

 */
void printIsosceles(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints an isosceles triangle (pointing down).
 
 Example (no spaces at the end of lines):

printIsoscelesPointingDown(3);
cout << endl;

*****
 ***
  *

 */
void printIsoscelesPointingDown(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints a diamond.
 
 Example (no spaces at the end of lines):
 
printDiamond(1);
cout << endl;
printDiamond(2);
cout << endl;
printDiamond(3);
cout << endl;

*

 *
***
 *

  *
 ***
*****
 ***
  *

 */
void printDiamond(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints an arrow starting with one *
           the next row has 2 additional *'s, the longest row has 4 * n + 3 *'s
           and the the *'s decrease by 2 per row until it is back to one *.
 
 Example (no spaces at the end of lines and
          blank lines are printed by test1.cpp):
 
printArrow(2);
cout << endl;
printArrow(3);
cout << endl;
 
      *
      ***
***********
      ***
      *

        *
        ***
        *****
***************
        *****
        ***
        *

 */
void printArrow(int n);


/**
 Requires: val must be > 0.
 Modifies: Nothing.
 Effects:  Returns true if val is a prime number, false otherwise.
           A prime number is a natural number greater than 1 that has no
           positive divisors other than 1 and itself.
 */
bool isPrime(int val);


/**
 Requires: start must be > 0, end must be > 0.
 Modifies: Nothing.
 Effects:  Prints all primes numbers between start and end inclusive.
           Swaps start and end if start > end.
 
 Example (you also need to print commas, \b will not give you what you want):
 
printPrimes(5, 10);

5, 7
 */
void printPrimes(int start, int end);


/**
 Requires: start must be > 0, end must be > 0.
 Modifies: Nothing.
 Effects:  Prints all Mersenne primes between start and end inclusive.
           Swaps start and end if start > end.
           A Mersenne prime is a prime number of the form 2^n - 1
           where n is also a prime number. (2^n means 2 to the nth power.)
 
 Example:
 
printMersennePrimes(1, 50);

3
7
31
 */
void printMersennePrimes(int start, int end);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Returns the sum of all proper positive divisors of n.
           A positive proper divisor is a positive divisor of n
           excluding n itself.
 Example:  proper divisors of 6 are: 1, 2, 3.
           sumProperDivisors(6); // would return 6
 */
int sumProperDivisors(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Returns true if n is a perfect number, false otherwise.
           A perfect number is a positive integer equal to the sum of
           its proper divisors.
 */
bool isPerfect(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Returns true if n is an abundant number, false otherwise.
           An abundant number is a number for with the sum of its proper
           divisors is greater than the number itself.
 */
bool isAbundant(int n);


/**
 Requires: first must be > 0, second must be > 0.
 Modifies: Nothing.
 Effects:  Returns true if first and second are an amicable pair,
           false otherwise. An amicable pair consists of two integers for which
           the first is equal to the sum of proper divisors of the second and
           the second is equal to the sum of proper divisors of the first.
 */
bool isAmicable(int first, int second);


/*****************************************
 *                                       *
 *                S'mores                *
 *                                       *
 *****************************************/


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints an equilateral triangle starting with one *
           continuing until the last row has 'n' *'s
           The last row will start with a * and have one space between *'s
           Must be left justified and must NOT have any characters past
           the last * in any given line. Put one and only one blank line after
           the last line of the triangle. Do not begin with a blank line.
 
 Example:
 
printEquilateral(3);
cout << endl;

  *
 * *
* * *

 */
void printEquilateral(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints an isosceles triangle pointing right.
 
 Example (no spaces at the end of lines):
 
 
printIsoscelesPointingRight(1);
cout << endl;
printIsoscelesPointingRight(3);
cout << endl;
 
*

*
**
***
**
*

 */
void printIsoscelesPointingRight(int n);


/**
 Requires: n must be > 0.
 Modifies: Nothing.
 Effects:  Prints two arrows arrow starting with one *
           the next row has 2 additional *'s, the longest row has 4 * n + 3 *'s
           and the the *'s decrease by 2 per row until it is back to one *.
 
 Example (no spaces at the end of lines and
          blank lines are printed by test1.cpp):
 
printDoubleArrow(2);
cout << endl;
printDoubleArrow(3);
cout << endl;

      *         *
      ***     ***
*********** ***********
      ***     ***
      *         *

        *             *
        ***         ***
        *****     *****
*************** ***************
        *****     *****
        ***         ***
        *             *

 */
void printDoubleArrow(int n);


/**
 Requires: n must be > 0,
           inner and outer must be a printable non-whitespace character.
 Modifies: Nothing.
 Effects:  Prints a nested square altering characters between outer and inner.
           Characters in each row are separated by a single space.

 Example:

printNestedSquares(9, '*', '\'');  //will produce

* * * * * * * * *
* ' ' ' ' ' ' ' *
* ' * * * * * ' *
* ' * ' ' ' * ' *
* ' * ' * ' * ' *
* ' * ' ' ' * ' *
* ' * * * * * ' *
* ' ' ' ' ' ' ' *
* * * * * * * * *

printNestedSquares(5, 'x', '.'); // will produce

x x x x x
x . . . x
x . x . x
x . . . x
x x x x x
 
printNestedSquares(4, 'x', '.'); // will produce

x x x x
x . . x
x . . x
x x x x

 */
void printNestedSquares(int n, char outer, char inner);


#endif
