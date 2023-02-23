- ((63f7911c-f361-4cbf-9245-09815d2ba7ab))
- First question a programmer should ask - does the code actually work?
- Code maintainability involves 
  * readability, organization, and modularity of one's code.
- High quality code need - code efficiency
  * data structure
  * algorithm
- Data structures
  collapsed:: true
	- how data is organized
	- wrong data structure mean slower or not working at all
- ## The Array: The Foundational Data Structure
  collapsed:: true
	- ## How computer memory work?
		- When a program declares an array, it allocates a contiguous set of empty cells for use in the program.
		- Now, every cell in a computer’s memory has a specific address.
	- ### Ds operations
	  id:: 63f7924e-168b-4f3b-a7cb-be97301d8137
		- Read : With an array, this means looking up a value at a particular index.
		  id:: 63f7925e-0b90-42dd-afb4-6b7deb405efa
		  collapsed:: true
			- A computer can read from an array in just one step.
			  Example:  the computer would simply take the memory address at index 0 and add 3.
			- Facts that allow Read operation to jump
			  1. A computer can jump to any memory address in one step.
			  2. Whenever a computer allocates an array, it also makes note at which memory address the array begins.
		- Search : With an array, this means looking to see if a particular value exists within the array, and if so, at which index.
		  id:: 63f79261-434b-47e7-b14f-52dcd6a42b96
			- computer has no way to jump to a particular value. We have to rely on *linear* search
			- For N cells in an array, linear search would take a maximum of N steps
		- Insert : With an array, this means adding a new value to an additional slot within the array.
			- Insert in the end 
			  * take one step because no need to shift
			- insert in the middle or begging 
			  * take N + 1 steps we have to shift and insert
			- Worst case scenario - insertion in the start
		- Delete : With an array, this means removing one of the values from the array
			- Like insertion, the worst-case scenario of deleting an element is deleting the very first element of the array.
			- This is because index 0 would become empty, and we’d have to shift all the remaining elements to the left to fill the gap.
- ## Measuring speed
  collapsed:: true
	- when we measure how “fast” an operation takes, we measured in how many steps it takes.
	- Terms: speed, time complexity, efficiency, performance, and runtime interchangeably. They all refer to the number of steps a given operation takes.
	- Why do we measure code’s speed in terms of steps?
		- Measuring the speed of an operation in terms of time is undependable, the time will always change depending on the hardware it is run on.
- ## Sets: How a Single Rule Can Affect Efficiency
  collapsed:: true
	- A *set* is a data structure that does not allow duplicate values to be contained within it.
	- [Reading, Search](((63f7924e-168b-4f3b-a7cb-be97301d8137)))- operations have same steps as classical array
	- Insertion
		- Inserting a value at the end of a set - Best case scenario 
		  * every insertion into a set first requires a search. 
		  * For preventing duplicate
		  * takes N + 1 steps - contrast regular array take one step
		- Insert beginning of a set - Worst case scenario
		  *  needs to search N cells
		  *  another N steps to shift all the data to the right, and another final step to insert the new value. 2N + 1 steps
		  * regular array take N + 1 steps
		-
- ## Exercises
  ((63f7a74f-d0c3-4d0c-a571-84c127a2748a))
	- 1. For an array containing 100 elements, provide the number of steps the following operations would take:
		- a. Reading - 1 step because array's address addition take one step
		  b. Searching for a value not contained within the array - 100 elements because array doesn't have starting address to add
		  c. Insertion at the beginning of the array - take N + 1 step for shifting and inserting
		  d. Insertion at the end of the array - take only one step
		  e. Deletion at the beginning of the array -  N steps delete, then shift
		  f. Deletion at the end of the array - take only one step
	- 2. For an array-based set containing 100 elements, provide the number of steps the following operations would take:
		- a. Reading - take 1 step
		- b. Searching for a value not contained within the array - take N steps
		- c. Insertion of a new value at the beginning of the set - 2N + 1 steps
		- d. Insertion of a new value at the end of the set - N + 1 steps
		- e. Deletion at the beginning of the set - N steps
		- f. Deletion at the end of the set - 1 step
	- 3. Normally the search operation in an array looks for the first instance of a given value. But sometimes we may want to look for every instance of a given value. For example, say we want to count how many times the value “apple” is found inside an array. How many steps would it take to find all the “apples”? Give your answer in terms of N.
		- This will take N steps because we need to inspect everything