# merge-sort-performance-analyzer
This Python script implements the Merge Sort algorithm and measures its performance on different sizes of input datasets. 
The code is designed to explore the relationship between the theoretical time complexity of Merge Sort and its actual runtime for various input sizes.



Code Overview

1. Recursive Merge Sort Implementation
   
	dziel(c): This function recursively divides the input list c into smaller sublists until each sublist contains only one element. It then merges the sublists back together in sorted order using the scal(a, b) function.
	
	scal(a, b): This function takes two sorted sublists a and b, and merges them into a single sorted list c. It repeatedly compares the smallest elements of a and b, appending the smaller one to c until one of the sublists is empty. The remaining elements of the other sublist are then appended to c.

3. Performance Testing Loop
	   
	The script generates random datasets of increasing sizes, starting from 5,000 elements and doubling the size in each iteration up to 80,000 elements.
	
	time.perf_counter(): The script uses this function to measure the time taken to sort each dataset.
	The actual runtime is printed for each dataset size, along with the theoretical 𝑛log𝑛
	time complexity for comparison.
