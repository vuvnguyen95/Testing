
# Compiling Instructions

## Overview
This README provides instructions for compiling the QuickSort program and the Input File Generator, both of which are part of this project.

## Requirements
- GCC Compiler (g++)
- Make
- C++11 standard support

## Structure
The project includes two main executables:
1. **Nguyen_Vu_QuickSort** - The main sorting program.
2. **InputFileGenerator** - A utility to generate input files for the sorting program.

## Compilation Steps

### QuickSort Program
- **File**: `Nguyen_Vu_QuickSort.cpp`
- **Executable**: `Nguyen_Vu_QuickSort`

### Input File Generator
- **File**: `InputFileGenerator.cpp`
- **Executable**: `InputFileGenerator`

### Compile Both Programs
1. To compile both the QuickSort program and the Input File Generator, simply run:
   ```
   make
   ```
2. This will create the `Nguyen_Vu_QuickSort` and `InputFileGenerator` executables.
   It will also automatically process all of the input files and generate output files accordinngly.
   Moreover, it also will generate `Nguyen_Vu_executionTime.txt` and `Nguyen_Vu_averageExecutionTime.txt` right after the output files are generated.
### Generate Input Files and Run QuickSort
- After compilation, you can automatically generate input files and run the QuickSort program on them by using:
  ```
  make run_sort
  ```

### Cleaning Up
- To clean up all compiled files (executables and object files), run:
  ```
  make clean
  ```

## Customization
You can customize the input file sizes and counts in the Makefile under the `SIZES` and `COUNT` variables. Default sizes are 10, 100, 1000, and the default count is 25.

## Notes
- The Makefile is set up with C++11 standards and includes flags for debugging and warnings.
- It's recommended to run `make clean` before recompiling to ensure a clean build.
- My generated files are in generated_files directory containing:
    - 3 input files (one for each input size)
    - 3 output files (one for each input size)
    - `Nguyen_Vu_executionTime.txt`
    - `Nguyen_Vu_averageExecutionTime.txt`
  to avoid being overwritten by other users.
- My plotting image is in the root directory of my project.

