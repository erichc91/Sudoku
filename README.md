# Sudoku
Sudoku as an Integer Linear Program written in Julia 1.1.0

## Requirements
* Julia
* JuMP package
* GLPK package

## Usage
The intent of this code uses the integer programming method to solve the Sudoku model as a feasibility problem. This eliminates clunky code and unneccaasary loops and a syntax that can get technically heavy fast.
Additionally the advantage of this code is eliminating the use of multiple packages that change independently and relies heavily on julia's list comprehension to create the constraints.

```julia
initial_grid = [
    3 0 0 0 0 0 0 0 9;
    0 0 0 9 0 0 0 7 5;
    0 0 0 0 0 0 0 0 0;
    0 0 4 8 0 6 0 0 2;
    5 0 0 1 0 0 0 0 0;
    8 0 6 0 3 0 4 5 0;
    0 0 8 0 0 0 0 0 0;
    0 0 0 0 0 0 0 0 0;
    0 0 0 0 0 0 0 3 0;
]
```

This initial matrix can be modified and replaced with any matrix and my notebook file will solve the sudoku.
