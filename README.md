Problem in Hackerrank:

Staircase detail

This is a staircase of size :
```
   #
  ##
 ###
####
```
Its base and height are both equal to . It is drawn using # symbols and spaces. The last line is not preceded by any spaces.

Write a program that prints a staircase of size .


Function Description

Complete the staircase function in the editor below.

staircase has the following parameter(s):

int n: an integer


Print

Print a staircase as described above.


Input Format

A single integer, , denoting the size of the staircase.


Constraints

0 < n <= 100


Output Format

Print a staircase of size  using # symbols and spaces.

Note: The last line must have  spaces in it.


Sample Input

6 


Sample Output
```
     #
    ##
   ###
  ####
 #####
######
```

Explanation

The staircase is right-aligned, composed of # symbols and spaces, and has a height and width of .

--------------------------------------------------------------------------------------------------

Solution:
```
function staircase(n){
  for(let i = 0; i < n ; i++){
    const line = Array(i+1)
    .fill('#')
    .join('')
    .padStart(n);
    console.log(line);
  }
}
console.log(staircase(6)); //Test 6 rows
```
Explanation:
By using for loop, the result will be six times output of the function as I test with variable 6. The Array syntax set the length of # with fill and join syntaxs, 
and padStart determine # starts from end of the row.
