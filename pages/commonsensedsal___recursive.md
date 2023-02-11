- ((63790a2b-a5cf-436f-a7df-12073ff1114f))
- **Recursion** is the term for a function calling itself. Indeed, infinite recursion, as in the above example, is utterly useless. When harnessed correctly, though, recursion can be a powerful tool.
- ((637915f7-16f0-4939-a344-4500ebbead71))
	- ((63791607-5f62-416c-92f2-960a87b8c70e))
	- if number is currently 0, we don’t call countdown() again.
	- 0 is a base case countdown
- This code can look somewhat confusing at first glance. To walk through the code to see what it does, here’s the process I recommend:
	- 1. Identify the base case. Note: no function calling itself but return something
	  2. Walk through the function for the base case. 
	  3. Identify the “next-to-last” case. This is the case just before the base case, as I’ll demonstrate momentarily. Note: function calling itself
	  4. Walk through the function for the “next-to-last” case.
	  5. Repeat this process by identifying the case before the one you just analyzed, and walking though the function for that case.
- ((637918b7-5ed7-4966-ab57-9093448dc59f))
	- Computer keep track of functions call
		- The Call Stack: stack in memory is use for keeping tracks of function calls
		- computer push variablee vaules, which line it's in the middle of,
		- when the function hit the base it pop the last function it was push on the stack and return.
- ((63791b59-f9a1-4c32-9273-8f9a0af3479d))
	- stack over flow happened when RAM run out of memory because stack over flow RAM.
	- either the code doesn't have base condition for recursion or by pass the base
- Recursion usefulness
	- Filesystem traversal
	- ((63791ce7-2c8b-41d2-8f7d-1babf42883a3))
- ((63791d8d-a48c-4fb8-beb7-b1b71a58f08f))
	- 1. Base case:
	  if low > high : stop the recursion once low has exceeded hgih
	- 2. if we change factorial of n * (n - 1) to n * (n - 2)
	  we will get infinite loop because it the base condition if n == 1 will not be true
	  we will be skipping even number by 1 or every other number till we hit the base
	  if n = 5 then factorial will be 5 * 3 * 1 = 15 ...
	- 3. 
	  ```python
	  def sum(low, high):
	    if high <= low:
	      return low
	    else:
	      return high + sum(low, high - 1)
	    
	  ```
	- 4. Recursive function for traversing nested lists and number
	  ```python
	  array = [ 1,2,3,
	           [4, 5, 6],
	           7,
	           [8,[9, 10, 11,[12, 13, 14]]],
	           [15, 16, 17, 18, 19,[20, 21, 22,[23, 24, 25,[26, 27, 29]], 30, 31], 32], 
	           33]
	  def traverse_lists(array):
	    for value in array:
	      # keep traversing if the value is a list
	      #if type(arr) == []:
	      if isinstance(value, list):
	        return traverse_lists(value)
	      else:
	        # print the value if it is no longer a list
	       print(value)
	      
	  ```