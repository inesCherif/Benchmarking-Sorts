# Benchmarking-Sorts

This repository provides implementations of various sorting algorithms in Python and benchmarks their performance across different types of input data (random, sorted, reverse-sorted, and nearly sorted). The purpose of this repository is to compare the efficiency of different sorting algorithms in terms of execution time under different conditions. The benchmarking results are displayed using plots that visualize the performance of each algorithm across varying input sizes.

### Algorithms Included:
- **Merge Sort**
- **Quick Sort**
- **Heap Sort**
- **Shell Sort**
- **Radix Sort**

These algorithms are tested using a variety of input data sizes and are benchmarked based on their mean, median, and standard deviation of execution times.

## Code Overview

### 1. **Generating Random Data**
   The `generate_array(n)` function creates an array of size `n` with random integers between 1 and 10,000.

### 2. **Sorting Algorithms**
   The sorting algorithms included in this repository are implemented in separate functions:
   - `merge_sort(arr)`
   - `quick_sort(arr)`
   - `heap_sort(arr)`
   - `shell_sort(arr)`
   - `radix_sort(arr)`

### 3. **Benchmarking Functionality**
   - The `benchmark_sort(sort_func, arr, num_runs=5)` function benchmarks a given sorting function over a specified number of runs and calculates statistics such as the mean, median, and standard deviation of the execution time.

### 4. **Test Case Generation**
   The function `generate_test_cases(size)` generates different types of arrays for testing:
   - Randomly shuffled array
   - Sorted array
   - Reverse-sorted array
   - Nearly sorted array (with small random perturbations)

### 5. **Main Functionality**
   The `main()` function runs the benchmark tests across different sizes of arrays (`100`, `1000`, and `10,000`), and plots the benchmarking results using **Matplotlib**. The results show the performance of each sorting algorithm under different types of input data.

### Benchmarking Results:
The results are displayed in the form of a grid of logarithmic plots, where:
- The X-axis represents the array size.
- The Y-axis represents the time taken to sort the array (log scale for better visualization).
