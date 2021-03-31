# Mars Rovers Coding Challenge

Hi! If you're reading this, it's because you've been invited to 
take a coding challenge for an engineering role at Divido.

We anticipate that you will spend around 2 hours working on
this challenge. If you don't manage to complete everything in
time, that's ok; it's not a race.

## Scenario

A squad of robotic rovers are to be landed by NASA on a plateau on Mars. 
This plateau, which is curiously rectangular, must be navigated by the 
rovers so that their on-board cameras can get a complete view of the 
surrounding terrain to send back to Earth.

A rover’s position and location is represented by a combination of x and y 
co-ordinates, and a letter representing one of the four cardinal compass 
points (`N`, `S`, `E`, `W`). 

The plateau is divided up into a grid to simplify navigation. 
An example position might be `0 0 N`, which means the rover is in 
the bottom left corner and facing North.

In order to control a rover, NASA sends a simple string of letters. 
The possible letters are:

* `L` - makes the rover spin 90 degrees left without moving from its current spot
* `R` - makes the rover spin 90 degrees right without moving from its current spot
* `M` - means move forward one grid point, and maintain the same heading.

Assume that :
* The square directly North from (x, y) is (x, y+1).
* The square directly South from (x, y) is (x, y-1).
* The square directly West from (x, y) is (x-1, y).
* The square directly East from (x, y) is (x+1, y).

### Input file
The first line of input is the upper-right coordinates of the plateau, the lower-left 
coordinates are assumed to be `0 0`.

The rest of the input is information pertaining to the rovers that have been deployed. 
Each rover has two lines of input:

* The first line gives the rover’s position
* The second line is a series of instructions telling the rover how to explore the plateau.

The position is made up of two integers and a letter separated by spaces, corresponding to 
the x and y co-ordinates and the rover’s orientation. eg: ` 1 1 N`

Each rover will be finished sequentially, which means that the second rover won’t start to move until the first one has finished moving.

### Output
The output for each rover should be its final co-ordinates and heading.

We expect your program to output a position per line

### Example Input: 
5 5

1 2 N

LMLMLMLMM

3 3 E

MMRMMRMRRM

### Expected Output:

1 3 N

5 1 E

## Assumptions

* Your code should accept a file path to load.
  

* Your code must be able to detect invalid file format, and reject
   the file. This should be handled gracefuly and the app should not crash


* You are free to use any language, framework and libraries that you see fit. Although  we expect you not to use
   any that might defeat the purpose of this test.

## Assessment Criteria

* This repository contains a input file named `input.dat` We expect that file to be properly parsed.
  

* You will be expected to provide unit tests asserting the correct behaviour of your code


* You will be assessed both on the quality of tests, and on
the quality of the code that you write to pass them. 
  

* We're looking for concise, readable code.
  

* Documentation and ease of running your code will be taken into consideration

# Good Luck !