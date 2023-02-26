- ((63f908d4-8fa3-412a-844d-e58be863054b))
- [Big O: How Many Steps Relative to N Elements?](((63f90b1c-203f-490d-92d9-dfddab400626))) (p.36-37)
	- Big O notation is a way of measuring how fast an algorithm is relative to the number of elements it has to process (N).
	- Big O notation only cares about the most dominant factor that affects the speed of an algorithm, not the exact number of steps or seconds.
	- Big O notation uses mathematical expressions to describe how the number of steps grows as N increases.
	- For example, O(N) means that the number of steps grows linearly with N, O(N^2) means that it grows quadratically with N, and so on.
- [The Soul of Big O](((63f90b33-eac3-44bc-ba96-c294b7b8a81c))) (p.37-40)
	- The soul of Big O notation is to compare different algorithms based on how they scale with larger inputs.
	- Big O notation helps us choose the most efficient algorithm for a given problem by looking at their worst-case scenarios.
	- Big O notation also helps us avoid wasting time on optimizing insignificant parts of our code that have little impact on the overall speed.
- [An Algorithm of the Third Kind](((63f90b4e-72b2-4c30-9917-1fbbbb085e06))) (p.40-42)
	- An algorithm of the third kind is one that does not grow linearly or quadratically with N, but rather logarithmically.
	- Logarithms are mathematical functions that tell us how many times we have to divide a number by a base until we get 1.
	- For example, log base 2 of 8 is 3, because we have to divide 8 by 2 three times until we get 1 (8/2 = 4, 4/2 = 2, 2/2 =1).
- [Logarithms](((63f90b5c-d15a-474f-929b-7f3f2fd9773a))) (p.41-42)
	- Logarithms are useful for measuring how fast some processes grow or shrink over time.
	- For example, logarithms can measure how long it takes for bacteria to double in population, or how many digits a number has in a certain base.
	- Logarithms have some properties that make them easy to manipulate algebraically, such as log(a*b) = log(a) + log(b), and log(a^b) = b*log(a).
- [O(log N) Explained](((63f90b6e-2bb8-4df9-af75-9a386f1bca68))) (p.42-43)
	- O(log N) is a very efficient category of algorithms that can handle large inputs very quickly.
	- O(log N) algorithms work by reducing the problem size by half at each step until they find the solution or reach the base case.
	- For example, binary search is an O(log N) algorithm that can find an element in a sorted array by comparing it with the middle element and discarding half of the array at each step.
- [Practical Examples](((63f90b79-2d44-4d18-87bb-56669c50d02e))) (p.43-45)
	- Some practical examples of where we can use Big O notation to compare different algorithms are:
	- Finding duplicates in an array: We can use a nested loop (O(N^2)) or a hash table (O(N)).
	- Finding anagrams: We can sort each word and compare them (O(N*log N)) or count their letter frequencies and compare them (O(N)).
	- Finding common elements in two arrays: We can use two nested loops (O(N^2)) or sort both arrays and use pointers (O(N*log N)).
- [Exercises](((63fa9fc6-a768-411e-bad7-22326c1bf94e)))
- 1. Use Big O Notation to describe the time complexity of the following function that determines whether a given year is a leap year: 
  ```python
  function isLeapYear(year) { 
    return (year % 100 === 0) ? (year % 400 === 0) : (year % 4 === 0);
  }
  ```
	- This will take Big O of 1. It needs only one operation no matter the data size.
- 2. Use Big O Notation to describe the time complexity of the following function that sums up all the numbers from a given array: 
  ```javascript
  function arraySum(array) { 
    let sum = 0; 
    for(let i = 0; i < array.length; i++) { 
      sum += array[i];
    } 
    return sum;
  }
  ```
	- This function will take Big O of N
	- Steps of operation for adding array's element increase as the data get larger in linear.
- 3. The following function is based on the age-old analogy used to describe the power of compounding interest: Imagine you have a chessboard and put a single grain of rice on one square. On the second square, you put 2 grains of rice, since that is double the amount of rice on the previous square. On the third square, you put 4 grains. On the fourth square, you put 8 grains, and on the fifth square, you put 16 grains, and so on. The following function calculates which square you’ll need to place a certain number of rice grains. For example, for 16 grains, the function will return 5, since you will place the 16 grains on the fifth square. Use Big O Notation to describe the time complexity of this function, which is below: 
  ```javascript
  function chessboardSpace(numberOfGrains) { 
    let chessboardSpaces = 1; 
    let placedGrains = 1; 
    while (placedGrains < numberOfGrains) { 
      placedGrains *= 2; 
      chessboardSpaces += 1;
    } 
    return chessboardSpaces;
  }
  ```
	- This function will take Big O(log N).
	- On each iteration of the loop, `placedGrains` is multiplied by 2. Therefore, the loop will iterate a number of times equal to the logarithm base 2 of `numberOfGrains`.
	- As the data numberOfGrains larger the step to find the chessboardSpaces larger logarithmically.
- 4. The following function accepts an array of strings and returns a new array that only contains the strings that start with the character "a". Use Big O Notation to describe the time complexity of the function:
  ```python
  function selectAStrings(array) { 
    let newArray = []; 
    for(let i = 0; i < array.length; i++) { 
      if (array[i].startsWith("a")) { 
        newArray.push(array[i]);
      }
    } 
    return newArray;
  }
  ```
	- This function will run Big O of N.
	- In worst case scenario, element doesn't start with "a" we still have to traverse till the end.
- 5. The following function calculates the median from an ordered array. Describe its time complexity in terms of Big O Notation:
  ```python
  function median(array) { 
    const middle = Math.floor(array.length / 2);// If array has even amount of numbers: 
    if (array.length % 2 === 0) { 
      return (array[middle - 1] + array[middle]) / 2;
    } else { 
      // If array has odd amount of numbers: 
            return array[middle];
           
    }
  }
  ```
	- This function will run Big O of 1.
	- It take only constant operation of one to calculate median from ordered array.