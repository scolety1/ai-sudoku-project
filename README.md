# Sudoku Search Experiments

A coursework/research collection exploring constraint-satisfaction and stochastic search for Sudoku. The repository contains notebooks, puzzle fixtures, genetic-search implementations, tuning scripts, and recorded results.

## Start reading

- [CSP notebook](sudoku_solver.ipynb) and [second notebook](sudoku_solver2.ipynb).
- [Standalone genetic solver](reliable_ga_solver.py): puzzle parsing, conflict scoring, and retry strategies.
- [Standalone tuning](standalone_ga_tuning.py) and [tuning notes](GA_TUNING_README.md).
- [Puzzle fixtures](puzzles/).

The previously documented `sudoku_solver.py` and `test_sudoku.py` are absent from this public snapshot. Some tuning scripts depend on that missing module. Use the standalone entry point below; this is not a complete, uniformly runnable package.

## Run the standalone experiment

With Python and NumPy installed, from the repository root:

```sh
python -m pip install numpy
python reliable_ga_solver.py
```

Choose a strategy when prompted. It uses `puzzles/Easy-P1.txt`; genetic search can take time and does not guarantee a solution. The module import and 9×9 fixture parser were verified on November 14, 2026; full stochastic convergence and notebook execution were not re-certified. Recorded result files are historical evidence, not current performance guarantees.

## Contribution and scope

Collected by Spencer Colety. This archive includes coursework, examples, or starter material; the bulk-upload history does not establish sole authorship of individual methods. Preserve source credits and course-sharing restrictions. This README update was AI-assisted and does not change the exercise code.
