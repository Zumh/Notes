- ((63792318-c9bf-45fe-b556-a96f1db9b63d))
- Repeatedly Execute
	- Make the next recursive call
	  ```js
	  function countdown(number) { 
	    console.log(number); 
	    if(number === 0) { 
	      // number being 0 is the base case return;
	      return
	    } else { 
	      countdown(number - 1); // call another function
	    }
	  }
	  ```
	- Recursive tricks
	  * Passing Extra Parameters
	  * Double and in place modification
	  ```python
	  def double_array(array, index=0):
	    # 3 Base case: when the index goes past the end of the array 
	    if (index >= len(array)): 
	      return 
	    # 2 do what we want with the data. In this case double it and assign back into array
	    array[index] *= 2 
	    # 1 pass same array each function call and keep track of index value
	    double_array(array, index + 1)
	  ```
- Calculations
	- it is able to make a calculation based on a subproblem of the problem at hand.
	- imagine the solution is iterative solution first
	- subproblem strategy : 
	  * using same calculation 
	  * feeding smaller data each time the function is call
	  * till we reach the base then return
	- e.i factorial
	  ```python
	  def factorial(number):
	    # 3 we trap with the base value and return back to where it came from
	    if number == 1 :
	      return 1 
	    else:
	      # 1 we imagine of this recursive function call
	      # 2 then we calculate the factorial
	      return number * factorial(number - 1) 
	  ```
	- bottom up strategy
		- bottom up approach can be done in classic loop.
		- also factorial calculation can be done in recursive function
		  ```python
		  def factorial(n, i=1, product=1):
		  	# 3 the base return the final product if i or 1-n number got larger than n
		   	if i > n :
		        return product
		  	# 1 keep track of n and i = 1 to n and product
		      return factorial(n, i + 1, product * i)
		  ```
		- Disadvantage is we have to track and think about all the values
	- top down recursion
		- top down approach is good for recursive thinking and don't need to think about detail of how a function work
		- Top-down strategy - though process
		  1. Imagine the function you’re writing has already been implemented by someone else.
		  reverse "abcde"
		  ```python
		  reverse(string[1, string.length - 1])
		  ```
		  2. Identify the subproblem of the problem.
		  ```python
		  def reverse(string):
		  	return reverse(string[1, string.length - 1]) + string[0]
		  ```
		  3. See what happens when you call the function on the subproblem and go from there.
		  ```python
		  def reverse(string):
		   	# Base case: string with just one character 
		   	return string[0] if string.length == 1 
		  	return reverse(string[1, string.length - 1]) + string[0]
		  ```
		- array sum
-