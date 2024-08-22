# Arrays

## Definition
Arrays hold values of the same type at contiguous memory locations.

## Characteristics
- We only care about position/index of an element and element
- In Python, JS, Ruby, PHP, the array size is dynamic and we don't need to have size defined beforehand when creating array.
- Most array strategies can be applied to string problems.

## Advantages
- Store multiple elements of the same type with one single variable name
- Accessing elements is fast as long as we have index `O(1)`

## Disadvantages
- Addition and removal of elements into/from middle of array is slow because remaining elements need to be shifted to accommodate the new/missing element.
    - Exception is if position to be inserted/removed is at end of array.
- Certain languages where array size is fixed, array cannot alter its size after initialization. If insertion causes total number of elements to exceed the size, new array has to be allocated and existing elements have to be copied over.
    - Act of creating new array and transferring elements over takes `O(N)`.

## Time Complexities
| Operation | Big-O     | Note      |
| --------  | -------   | -------   |
| Access   | O(1) | |
| Search  | O(n) | |
| Search (sorted array) | O(log(n)) | |
| Insert  | O(n) | Shifts all subsequent elements to right by one |
| Insert (at end)  | O(1) | No other elements need to be shifted |
| Remove  | O(n)    | Shifts all subsequent elements to left by one |
| Remove (at end)  | O(1)    | No other elements need to be shifted |

## Review
1. Clarify if there are duplicate values in the array. Would the presence of duplicate values affect the answer? Does it make the question simpler or harder?
2. When using an index to iterate through array elements, be careful not to go out of bounds.
3. Be mindful of slicing or concatenating arrays in code. Typically, slicing and concatenating subarrays take `O(n)` time. Use start and end indices to demarcate subarray/range where possible

## Corner Cases
- Empty sequence
- Sequence with 1 or 2 elements
- Sequence with repeated elements
- Duplicated values in the sequence

## Techniques
[ ] Sliding window
[ ] Two pointers
[ ] Traversing from the right
[ ] Sorting the array
[ ] Precomputation
[ ] Index as a hash key
[ ] Traversing the array more than once