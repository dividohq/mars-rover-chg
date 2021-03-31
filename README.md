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
* The square directly North from `(x, y)` is `(x, y+1)`.
* The square directly South from `(x, y)` is `(x, y-1)`.
* The square directly West from `(x, y)` is `(x-1, y)`.
* The square directly East from `(x, y)` is `(x+1, y)`.

### Input

The first line of input is the upper-right coordinates of the plateau, the lower-left 
coordinates are assumed to be `0 0`.

The rest of the input is information pertaining to the rovers that have been deployed. 
Each rover has two lines of input:

* The first line gives the rover’s position
* The second line is a series of instructions telling the rover how to explore the plateau.

The position is made up of two integers and a letter separated by spaces, corresponding to 
the x and y co-ordinates and the rover’s orientation. eg: `1 1 N`

Each rover will be finished sequentially, which means that the second rover won’t start to move until the first one has finished moving.

### Output

The output for each rover should be its final co-ordinates and heading.

### Example Input: 
```
5 5
1 2 N
LMLMLMLMM
3 3 E
MMRMMRMRRM
```

### Expected Output:
```
1 3 N
5 1 E
```

## Assessment Criteria

You may use any language or framework of your choice to complete this assessment. Whatever your choice, we
will use the following assessment criteria:

1. **Clean code**: we value readability and separation of concerns. Make your code as simple as it can
   possibly be, but no simpler than that.
   
2. **Unit tests**: we value testing; you should demonstrate that you understand the fundamentals of how
   to test your application, and be able to suggest ways in which the testing could be improved. We will
   assess both your code, and the tests.
   
3. **Idiomatic code**: all languages have their own community standards; you should be aware of these, and
   be able to write code that meets those standards. For example, the [PSR-12](https://www.php-fig.org/psr/psr-12/) format for PHP.

4. **Documentation**: the ability to write clear and concise documentation is a skill in and of itself;
   feel free to provide an expanded `README` file with instructions on how to run your application. Use
   code comments liberally, and explain the _why_, not the _what_.
   
5. **Clean commit history**: one of the best ways for us to understand how you think is to see how you
   approached the problem. Commit early and often; don't be afraid to use multiple branches and make changes
   as you go. Logical, understandable commit messages are a bonus.

## Extra Credit

Extra points if your code handles unexpected situations graciously and takes into account the plateu size when
calculating movements

# Good Luck !
