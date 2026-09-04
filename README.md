# Laboratory Activity: Recursion — Recursive Binary Search

## Description
This program implements the recursive binary search algorithm in Java. It accepts
a user-input array size, array elements, and a target value. It automatically
sorts the entered array in ascending order (required for binary search), then
recursively searches for the target. At every recursive call, the program prints
the current `low`, `high`, `mid`, and `arr[mid]` values so the shrinking search
interval can be traced. The program outputs the index of the target if found,
or `-1` if it is not in the array.

## Programming Language
Java (JDK 21)

## How to Compile and Run
```
javac Binary_search.java
java Binary_search
```

## Sample Input and Output
```
Enter the number of elements: 7
Enter 7 numbers in sorted (ascending) order:
Element 1: 40
Element 2: 10
Element 3: 70
Element 4: 20
Element 5: 50
Element 6: 30
Element 7: 60
Sorted array: 10 20 30 40 50 60 70

Enter a number to search: 50

Trace
bSearch(low=0, high=6) -> mid=3, arr[mid]=40
50 > 40 -> search right half
bSearch(low=4, high=6) -> mid=5, arr[mid]=60
50 < 60 -> search left half
bSearch(low=4, high=4) -> mid=4, arr[mid]=50
arr[4] == 50 -> found!

Target found.
Index: 4
```

## AI Disclosure
Claude (Anthropic) was used to help structure the recursive method's supporting
code (input handling, sorting, trace print statements), build the recursion
trace table, and write the explanation of the base cases for this laboratory
activity. All code was compiled and run to verify the outputs shown above.
