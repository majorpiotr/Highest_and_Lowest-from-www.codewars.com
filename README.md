# Highest_and_Lowest-from-www.codewars.com
My solution for problem from www.codewars.com. 

In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.

Example:

highAndLow("1 2 3 4 5"); // return "5 1"
highAndLow("1 2 -3 4 5"); // return "5 -3"
highAndLow("1 9 3 4 -5"); // return "9 -5"
Notes:

All numbers are valid Int32, no need to validate them.
There will always be at least one number in the input string.
Output string must be two numbers separated by a single space, and highest number is first.
 
 
 
 My solution :
function highAndLow(numbers){
  // ...
numbers_array=numbers.split(" "); // we write numbers to array
var  max = Math.max.apply(null, numbers_array); // find gratest number by Math.max
var  min = Math.min.apply(null, numbers_array); // find lowest number by Math.min
var out = max + " " + min ; // we write numbers to "out" 
return (out); // and return "out"
}
