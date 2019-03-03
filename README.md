# java_parallel_concurrent_distributed

Homework assignments of these online courses, completed in my own spare time
* [Parallel Programming in Java](https://www.coursera.org/learn/parallel-programming-in-java/)


---
## Subdirectories
#### `parallel_loops_and_chunking`
Used the Java [PCDP library](https://github.com/habanero-rice/PCDP) written by Rice University to speed up matrix multiplication with parallel for loops. To avoid creating too many parallel tasks, I used chunking.
#### `parallel_streams`
Used the Stream API provided by Java 8 to implement filter-map-reduce operations. Methods used include:
* `parallel()` to speed up computation
* `filter()`
*  `map()` methods
*  reduction methods such as `average()`, `count()`, `max()`
