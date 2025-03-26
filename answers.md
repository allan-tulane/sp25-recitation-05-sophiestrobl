# CMPS 2200 Reciation 5
## Answers

**Name:** Sophie Strobl


Place all written answers from `recitation-05.md` here for easier grading.





- **1b.**
The running times generally match their theoretical bounds: selection sort is consistently slow with O(n²) behavior regardless of input, while Quicksort with a random pivot performs closer to O(n log n) on average. Quicksort with a fixed pivot (first element) can degrade to O(n²) on already sorted lists, poor performance. In contrast, random inputs allow randomized Quicksort to shine, highlighting how input type significantly affects sorting efficiency.



- **1c.**
When comparing the fastest of the sorting implementations—Quicksort with a random pivot—to Python’s built-in sorted() function (which uses Timsort), sorted() consistently outperforms Quicksort in both randomly shuffled and already sorted input cases. This is expected, because Timsort is a hybrid algorithm optimized for real-world data. It combines the speed of mergesort and the efficiency of insertion sort on small or partially sorted data. While randomized Quicksort performs well on average with O(n log n) time, Timsort is highly optimized in Python’s C implementation and adapts to existing order in the list, making it faster and more stable in practice.