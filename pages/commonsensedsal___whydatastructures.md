- ((6373daed-2f7c-4c05-8a8c-b86f3f8ca72b))
	- How we organize our data can effect the speed of operations.
	- ((6373db10-844f-4809-b25a-6be0362f05c6))
		- Array - Foundational ds
			- Random access with O(1)
		- Ds Operations
			- Read:
			  Looking up a value at particular index
			  Read operation use jumping mem address in one step. 
			  Time Complexity: O(1)
			- Search:
			  Looking to see if a particular value exists within the array
			  Linear search is perform on classic array
			  Time Complexity: O(N)
			- Insert:
			  Adding a new value to an additional slot within the array
			  We insert the data at the end or between. But we have to shift elements and it take O(N)
			  Then O(N+1) to insert it.
			  Time Complexity: O(N+1)
			- Delete:
			  Removing one of the value from the array
	- Measuring speed
		- we measure code's speed in terms of steps.
		- How many steps it takes as the data N get larger?
		- measuring algorithm speed with steps will not change in any other machine.