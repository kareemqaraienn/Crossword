# AI Crossword Puzzle Solver
This is an AI-powered crossword puzzle solver built using Python. The solver uses a combination of constraint propagation and backtracking search to generate complete crossword puzzles.

## How It Works
There are two Python files in this project: crossword.py and generate.py. crossword.py contains two classes - Variable and Crossword - which define the structure of the puzzle. generate.py contains a class CrosswordCreator that solves the crossword puzzle using constraint propagation and backtracking search.

To generate a crossword puzzle, CrosswordCreator first enforces node consistency on the puzzle to ensure that every value in a variable's domain satisfies the unary constraints. It then enforces arc consistency to ensure that binary constraints are satisfied. Finally, it uses backtracking search to try to calculate a solution to the problem.

## How to Use It
To generate your own crossword puzzle, you can create a new Crossword object in crossword.py by providing a structure file and a words file. You can then create a new CrosswordCreator object in generate.py and call the solve function to solve the puzzle (this part is already coded for you).

Example: run this code -> `python generate.py structure_file words_file [output_file]`

- structure_file is the path to a file that contains the puzzle structure.

- words_file is the path to a file that contains the list of words to use in the puzzle, one word per line.

- output_file is an optional argument that specifies the file name to save the output image to. If not specified, the image will be displayed on the screen.

The final solution to the crossword puzzle will be printed to the console and/or saved as an image file based on whether the user gives an optional image argument.

Feel free to test it on your own structure_file and words_file but make sure the format is consistent with the example files


Have fun creating your own crossword puzzles!

## Credits
This program's relevant functions were written by me, and is based on a problem set for the course CS50AI from Harvard University. The course material and problem set were created by the staff at Harvard University, and are available at https://cs50.harvard.edu/ai/.
