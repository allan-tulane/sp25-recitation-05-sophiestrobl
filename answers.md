# CMPS 2200 Reciation 5
## Answers

**Name:** Sophie Strobl


Place all written answers from `recitation-05.md` here for easier grading.





- **1b.**
| n      | qsort-fixed-pivot | qsort-random-pivot | tim-sort |
|--------|-------------------|--------------------|----------|
| 100    | 0.110             | 0.119              | 0.008    |
| 200    | 0.214             | 0.234              | 0.015    |
| 500    | 0.545             | 0.647              | 0.041    |
| 1000   | 1.107             | 1.265              | 0.092    |
| 2000   | 2.380             | 2.698              | 0.171    |
| 5000   | 5.804             | 6.067              | 0.426    |
| 10000  | 10.557            | 11.568             | 0.838    |
| 20000  | 20.836            | 23.317             | 1.718    |
| 50000  | 56.506            | 62.884             | 4.776    |
| 100000 | 116.435           | 131.134            | 10.238   |




- **1c.**
When comparing the fastest of the sorting implementations—Quicksort with a random pivot—to Python’s built-in sorted() function (which uses Timsort), sorted() consistently outperforms Quicksort in both randomly shuffled and already sorted input cases. This is expected, because Timsort is a hybrid algorithm optimized for real-world data. It combines the speed of mergesort and the efficiency of insertion sort on small or partially sorted data. While randomized Quicksort performs well on average with O(n log n) time, Timsort is highly optimized in Python’s C implementation and adapts to existing order in the list, making it faster and more stable in practice.