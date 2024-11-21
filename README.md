# Second Largest Number Finder

## Project Overview

This project is designed to take an array of integers and return the second largest number among them. The main functionality is implemented in C++ using a simple sorting approach.

## Features

* Accepts an array of integers.
* Returns the second largest number from the array.
* Demonstrates basic usage of C++ Standard Library functions.

## Code Structure

### Source Code

```cpp
#include <bits/stdc++.h>

using namespace std;

// Function to find the second largest number in an array.
// Takes a vector of integers and its size as parameters.
// Returns the second largest integer in the array.
int secondlargest(vector<int> arr, int n)
{
    // Sort the array in ascending order
    sort(arr.begin(), arr.end());
    // Return the second last element which is the second largest
    return arr[n - 2];
}

int main()
{
    // Initialize a vector with sample integers
    vector<int> arr = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    
    // Call the secondlargest function and store the result
    int ans = secondlargest(arr, 10);
    
    // Output the result to the console
    cout << ans;
    
    return 0;
}
```

### Function Documentation

#### `int secondlargest(vector<int> arr, int n)`

* **Description**: Finds the second largest number in a given array of integers.
* **Parameters**:
    * `vector<int> arr`: A vector containing integer values.
    * `int n`: An integer representing the size of the array.
* **Returns**: The second largest integer in the array.
* **Usage Example**:

    ```cpp
    vector<int> numbers = {5, 2, 8, 1, 7};
    int result = secondlargest(numbers, numbers.size());
    // result will be 7
    ```

### Instructions for Compilation and Execution

1. Ensure you have a C++ compiler and development environment set up.
2. Copy the code into a `.cpp` file (e.g., `secondlargest.cpp`).
3. Open your terminal or command prompt.
4. Navigate to the directory where the file is saved.
5. Compile the code using the command:

    ```sh
    g++ -o secondlargest secondlargest.cpp
    ```
6. Run the compiled program:

    ```sh
    ./secondlargest
    ```

### Output

* The program will print the second largest number from the predefined array to the console.
* For the provided sample array `{1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`, the output will be:

    ```
    
    ```

9

```

## Dependencies
- C++ standard libraries (e.g., `<bits/stdc++.h>`).

## Notes
- The current implementation assumes that the input array will always have at least two distinct elements to find the second largest number.
```
