# Answer for Part2
### Accessing the value of the name property in the student object
student.name
### Accessing the value of the Grad Year property in the student object
student["Grad Year"]
### Calling the function for the greeting property in the student object
student.greeting()
### Accessing the name property of the object in the Favorite Teacher property in student
student["Favourite Teacher"].name
### Access index zero in the array of the courseLoad property of the student object
student.courseLoad[0]
 
## Basic Operators & Type Conversion 
## Question 13:
Output:
```
zhangyuqin@MacBook-Pro javascript % node part2-question13.js
32
1
3
3null
4
0
3undefined
NaN
```
A:

## Question 14:
A: true String '2' becomes a number 2
B: false The first letter of '2' is 2 which is greater than the first letter of '12' which is 1.
C: true It is because == converts '2' to number 2, then 2 == 2 is true.
D: false It is because 2 and '2' are different types so === immediately returns false
E: false The value of true is 1 where 1 == 2 is false.
F: true Since boolean() is true when inside variable has a value, where in this case is 2. Thus, true == true is true.

## Question 15:
If a and b are of different types, then a === b immediately returns false without an attempt to convert them, while operands of different types are converted to numbers by the equality operator ==.

## Question 17:
The result will be that function modifyArray will return an array where the value of every element is twice as it in the array, which is [2,4,6]. In the for loop callback pass the ith element in the array and in doSomething function, it doubles the value and return it to callback. Then, we push the value to newArr. Finally, it doubles the value in the given array and stores them in the newArr.

## Question 19:
The output is :
```
zhangyuqin@MacBook-Pro javascript % node part2-question19.js
1
4
3
2
```
Which is because it prints 1 at first, then there are two timeouts, then we output 4. Then we go back to time out, 2 has 1 second delay and 3 has 0 second delay. Thus, we output 3 first then 2. The output is 1,4,3,2.