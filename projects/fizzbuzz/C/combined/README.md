## FizzBuzzBazz Program In C - Colaborated Version

This program takes prompts the user to enter an integer greater than 0 at runtime. The program will loop through each integer from 1 to the given value and checks each value to see if there is a remainder when you divide it by three or five.

* If the integer divides by 3 with no remainder:
	* Add "Fizz" to print statement
* If the integer divides by 5 with no remainder:
	* Add "Buzz" to print statement
* If the integer divides by 7 with no remainder:
	* Add "Bazz" to print statement
* If the integer has a remainder for dividing by 3, 5, and 7:
	* Print the current number being checked

#### Sample output:

```
w/ n = 25

1
2
Fizz
4
Buzz
Fizz
Bazz
8
Fizz
Buzz
11
Fizz
13
Bazz
FizzBuzz
16
17
Fizz
19
Buzz
FizzBazz
22
23
Fizz
Buzz
```

### Build steps for core FizzBuzzBazz:

```
$ git clone https://github.com/sleddog/methods.git FizzBuzzBazz
$ cd FizzBuzzBazz/projects/fizzbuzzbazz/C/C-combined/
$ ./fizzBuzzBazz.sh
```

### Build steps for unit testing FizzBuzzBazz:

* Install unit testing framework 'Criterion'
	* [Criterion Documentation Release 2.3.3](https://media.readthedocs.org/pdf/criterion/latest/criterion.pdf)
	* Criterion uses the [CMake](https://cmake.org/) build system
		* *Additional build dependencies may be required*

```
$ git clone --recursive https://github.com/Snaipe/Criterion
$ cd Criterion
$ mkdir build
$ cd build
$ cmake ..
$ cmake --build .
$ sudo make install
```

After the unit testing framework is successfully installed:

```
$ git clone https://github.com/sleddog/methods.git FizzBuzzBazz
$ cd FizzBuzzBazz/projects/fizzbuzzbazz/C/C-combined/
$ chmod +x runTests.sh
$ ./runTests.sh
```

Notes:
The script to run the unit tests of FizzBuzzBazz will clean the install by removing the compiled files after completing tests. The macro guard for print output will prevent FizzBuzzBazz from printing each iteration for the unit tests.

### How to add/remove key-value pairs in the program
there is a line that reads
```
struct KV keys[x];
```
change the value of x to the number of key-value pairs to the number of pairs you want the program to have

There is also a section that has code that looks like
```
keys[x].key = y;
strncpy(keys[x].value, "Word", 4);
```
follow this structure when adding more key-value pairs

Note: the number of key-value pairs that are declared must be equal to the x value in the struct KV keys[x] line.

### Thank you for using FizzBuzzBazz
