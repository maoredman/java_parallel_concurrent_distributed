# java_parallel_concurrent_distributed

Homework assignments of these online courses, completed in my own spare time
* [Parallel Programming in Java](https://www.coursera.org/learn/parallel-programming-in-java/): fork/join framework, futures, streams, parallel loops, barriers, chunking, phasers, pipeline parallelism, data flow computing with asyncAwait, functional and structural determinism

---

## Subdirectories

#### `parallel_loops_and_chunking`
Used the Java [PCDP library](https://github.com/habanero-rice/PCDP) written by Rice University to speed up matrix multiplication with parallel for loops. To avoid creating too many parallel tasks, I used chunking.

#### `parallel_streams`
Used the Stream API provided since Java 8 to implement filter-map-reduce operations. Methods used include:
* `parallel()` to speed up computation
* `filter()`
*  `map()` methods
*  reduction methods such as `average()`, `count()`, `max()`

#### `phasers_fuzzy_barrier`
Used the Phaser API provided since Java 7 to implement a fuzzy barrier. Methods used include:
* `phaser.arrive()`: declare finished computation of data that other threads depend on
* `phaser.awaitAdvance(curr_phase)`: wait for other threads to compute necessary data
