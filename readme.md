## Suduko Game
  This is a Bootcamp Prep Project.
 Sudoku is a logic puzzle played on a 9x9 grid subdivided into 9 3x3 subgrids. 


The player is presented a partially filled puzzle, and must complete it following these rules:

- Each column must contain the numbers 1-9 (no repeats!)
- Each row must contain the numbers 1-9 (no repeats!)
- Each 3x3 subgrid must contain the numbers 1-9 (no repeats!)
// If you've never played sudoku before, try an "easy" puzzle from the New York Times' puzzle section.



## GOAL
 The ultimate goal of this project is to create a "sudoku checker". The sudoku checker will be a function that accepts a single sudoku grid (represented by an array of arrays) and returns true if the grid follows the rules above and false if not.

##APPROACH
 Your final sudoku checker function will be relatively complex. To build it, we're going to write several simple functions that combine to perform a larger complex operation. The concept of building complicated functions by combining simple ones is referred to as function composition).

 We know that our final function will need to check whether a given grid follows the three rules above. This provides an excellent "separation of concerns".

## SEPARATION OF CONCERNS
 Separation of concerns is another programming design principle, which states that a program should be split into distinct sections, such that each section addresses a separate concern.

There are several benefits to writing code with good separation of concerns. First, your code becomes more expressive. When describing the problem of sudoku in plain English, we split the puzzle into three rules. By mirroring that organization, your code becomes easier for you and other developers to interpret.

Second, separation of concerns leads to modular code. With modular code, individual sections can be re-used easily. So if we were tasked with solving a similar problem (such as writing a checker for the sudoku-variant nonomino) we could quickly and easily develop a solution by reusing the code we've already written.

Modular code also allows you to improve or modify one section of code without having to know (or change) the details of other sections. This benefit, and the others listed, will become clearer as you write more, increasingly complex code.

## GETTING STARTED
 To start, using an empty CodePen or repl.it, write the following functions:
 
 getRow: This function should accept two arguments: a sudoku grid (represented by an array of arrays) and a row index. The function should return an array containing the numbers in the specified row.