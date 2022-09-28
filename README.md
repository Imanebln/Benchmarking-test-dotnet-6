# Benchmarking-test-dotnet-6

## Benchmarking LINQ Performance
 - This is a simple exmaple that benchmarks the performance of the Single and First methods of LINQ.

###### Interpreting the Benchmarking Results
 - For each of the benchmarked methods, a row of the result data is generated. Because there are two benchmark methods called using three param values, there are six rows of benchmark result data. The benchmark results show the mean execution time, garbage collections (GCs), and the allocated memory.

The Mean column shows the average execution time of both the methods. As is evident from the benchmark results, the First method is much faster than the Single method in LINQ. The Allocated column shows the managed memory allocated on execution of each of these methods. The Rank column shows the relative execution speeds of these methods ordered from fastest to slowest. Because there are two methods here, it shows 1 (fastest) and 2 (slowest) for the First and Single methods respectively.

Here's what each of the legends represent:

 - Method: This column specifies the name of the method that has been benchmarked.
 - Mean: This column specifies the average time or the arithmetic mean of the measurements made on execution of the method being benchmarked.
 - StdDev: This column specifies the standard deviation, i.e., the extent to which the execution time deviated from the mean time.
 - Gen 0: This column specifies the Gen 0 collections made for each set of 1000 operations.
 - Gen 1: This column specifies the Gen 1 collections made for each set of 1000 operations.
 - Gen 2: This column specifies the Gen 2 collections made for each set of 1000 operations. (Note that here, Gen 2 isn't shown because there were no Gen 2 collections in   this example.)
 - Allocated: This column specifies the managed memory allocated for a single operation.
