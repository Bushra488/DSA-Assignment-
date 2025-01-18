# Implementation of Binary Search and Linear Search

def linear_search(arr, target):
    """Linear search implementation."""
    for index, value in enumerate(arr):
        if value == target:
            return index
    return -1

def binary_search(arr, target):
    """Binary search implementation."""
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1

def main():
    """Main function to run searches and demonstrate time complexities."""
    print("\n*** Binary Search and Linear Search Demonstration ***\n")

    # Input array and target
    arr = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
    target = 70

    print("Array:", arr)
    print("Target:", target)

    # Linear Search
    print("\nPerforming Linear Search...")
    linear_result = linear_search(arr, target)
    if linear_result != -1:
        print(f"Target found at index {linear_result} using Linear Search.")
    else:
        print("Target not found using Linear Search.")

    # Binary Search
    print("\nPerforming Binary Search...")
    binary_result = binary_search(arr, target)
    if binary_result != -1:
        print(f"Target found at index {binary_result} using Binary Search.")
    else:
        print("Target not found using Binary Search.")

    # Demonstrating worst-case for Binary Search (O(n))
    print("\nDemonstrating Binary Search Worst-Case (O(n))...")
    unsorted_arr = [100, 90, 80, 70, 60, 50, 40, 30, 20, 10]
    print("Unsorted Array:", unsorted_arr)
    binary_result_unsorted = binary_search(unsorted_arr, target)
    print("Target not found correctly because Binary Search requires sorted data.")
    print("This demonstrates the worst-case time complexity O(n) if the array is not sorted.")

if __name__ == "__main__":
    main()
