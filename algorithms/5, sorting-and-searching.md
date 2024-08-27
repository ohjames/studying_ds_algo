# Sorting and Searching

https://www.techinterviewhandbook.org/algorithms/sorting-searching/

## Definition
Sorting is the act of rearranging elements in a sequence in order, either numerical or lexicographical order, and either ascending or descending.

## Characteristics
- On sorted array of elements, leverage on its sorted property, searching can be faster than `O(n)` time via binary search.

## Time Complexities
| Algorithm | Time | Space |
| :--------: | :-------: | :-------: |
| Bubble sort   | O(n^2^) | O(1) |
| Insertion sort   | O(n^2^) | O(1) |
| Selection sort | O(n^2^) | O(1) |
| Quicksort   | O(n log n) | O(log n) |
| Mergesort   | O(n log n) | O(n) |
| Heapsort   | O(n log n) | O(1) |
| Counting sort   | O(n + k) | O(k) |
| Radix sort   | O(nk) | O(n + k) |
| Binary search   | O(log n) |  |

## Review
1. Know time/space complexities of language's default sorting algorithm `O(n log n)` typically.
    a. Python's sort is called `Timsort`

## Corner Cases
- Empty sequence
- Sequence with one element
- Sequence with two elements
- Sequence containing duplicate elements

## Techniques
- Sorted inputs
    - Given sequence in sorted order, use binary search
- Sorting input with limited range
    - Counting sort is non-comparison based sort use on numbers where we know range of values beforehand.