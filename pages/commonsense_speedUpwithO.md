- ((63f9642a-74ca-4b57-aff4-8ad4a9e4b0f6))
- Define Bubble sort: Bubble sort is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares adjacent elements and swaps them if they are in the wrong order. This process is repeated until no more swaps are needed, indicating that the list is sorted.
- Explain the algorithm step-by-step:
	- Compare the first two elements of the list. If the first element is greater than the second element, swap them.
	- Move to the next pair of elements and repeat step 1 until you reach the end of the list.
	- If any swaps were made in the previous pass, repeat step 1 again for the entire list.
	- Repeat steps 1-3 until no more swaps are needed.
- Analyze the performance of the algorithm:
	- Best case: O(n), where n is the number of elements in the list, when the list is already sorted.
	- Worst case: O(n^2), where n is the number of elements in the list, when the list is in reverse order.
	- Average case: O(n^2), where n is the number of elements in the list.
- Discuss ways to make Bubble sort faster:
	- One way to improve Bubble sort is to use a flag to check if any swaps were made during a pass. If no swaps were made, then the list is already sorted, and the algorithm can terminate early.
	- Another way to improve Bubble sort is to stop the algorithm once the nth pass is completed without any swaps. This is because the last n elements are already sorted, and there is no need to compare them again in subsequent passes.
- Using extra space can improve the time complexity of finding duplicates in a list.
	- If we simply use nested loops to compare each element of the list with every other element, the time complexity would be O(n^2), where n is the number of elements in the list. However, by using extra space to store elements in a hash set or dictionary, we can achieve a linear time complexity of O(n).
	- Here is an example algorithm to find duplicates using a hash set:
		- Initialize an empty hash set.
		- For each element in the list:
		  a. If the element is not in the hash set, add it.
		  b. If the element is already in the hash set, it is a duplicate.
		- Return the set of duplicates found.
		- In this algorithm, adding an element to a hash set takes constant time on average, so the time complexity of the entire algorithm is O(n) in the average case. In the worst case, where all elements are distinct, the time complexity would still be O(n), as we need to iterate through the entire list once.
		- Note that using extra space does increase the space complexity of the algorithm, which may be a consideration depending on the size of the input list and available memory.
- [Exercises](((63faaaca-58de-4f37-b300-74458f6f2a5e)))
	- 1. Replace the question marks in the following table to describe how many steps occur for a given number of data elements across various types of Big O:
	  |N elements|O(N)|O(log N)|O(N^2)|
	  |100|100|?|?|
	  |2000|?|?|?|
		- |N elements|O(N)|O(log N)|O(N^2)|
		  |100|100|about 7|(100)^2|
		  |2000|2000|about 11|(2000)^2|
			- To determine how many iterations of the loop are needed to reach this point, we can calculate the logarithm base 2 of 128:
			  $log_{2}N$ == steps
			  $log_{2}128$ = 7 steps
			  Therefore, the loop will iterate 7 times in total. On each iteration, `placedGrains` is multiplied by 2, starting from the initial value of 1. So the values of `placedGrains` on each iteration will be:
			  Iteration 1: 1
			  Iteration 2: 2
			  Iteration 3: 4
			  Iteration 4: 8
			  Iteration 5: 16
			  Iteration 6: 32
			  Iteration 7: 64
			  At this point, the loop terminates because `placedGrains` is greater than or equal to 100. Therefore, the function will return 7 as the number of steps that occur when N = 100.
	- 2. If we have an O(N^2) algorithm that processes an array and find that it takes 256 steps, what is the size of the array?
		- The size is sqrt(256) is 16 because O(N^2) mean we run nested for loop of N = 16 size.
	- 3. Use Big O Notation to describe the time complexity of the following func-
	  tion. It finds the greatest product of any pair of two numbers within a
	  given array:
	  ```python
	  def greatestProduct(array): 
	  	greatestProductSoFar = array[0] * array[1] 
	      for i, iVal in enumerate(array): 
	        for j, jVal in enumerate(array): 
	          if i != j and iVal * jVal > greatestProductSoFar: 
	            greatestProductSoFar = iVal * jVal 
	            return greatestProductSoFar
	  ```
		- This function will run O(N^2)
		- It takes two nested for loop to find largest product of two number
	- 4. The following function finds the greatest single number within an array, but has an efficiency of O(N2). Rewrite the function so that it becomes a speedy O(N):
	  ```python
	  def greatestNumber(array):
	    for i in array:
	      # Assume for now that i is the greatest:
	      isIValTheGreatest = True
	      for j in array:
	        # If we find another value that is greater than i,
	        # i is not the greatest:
	        if j > i:
	        	isIValTheGreatest = False
	      # If, by the time we checked all the other numbers, i
	      # is still the greatest, it means that i is the greatest number:
	      if isIValTheGreatest:
	      	return i
	  ```
		- ```python
		  def greatestNumber(array):
		  	maxValue = 0
		      for i in array:
		        if maxValue < i:
		          maxValue = i
		      return maxValue
		  ```