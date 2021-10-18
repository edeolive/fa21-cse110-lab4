1. `3` will be printed, because `i` is a function scoped variable that is incremented to the length of the input array `prices` by line 12. The length of `prices` when it is run is 3.
2. `150` will be printed, because `discountedPrice` is a function scoped variable and `discountedPrice` is last set to the value of the last item in `prices` times `1 - discount`, printing `discountedPrice` on line 13 will return 150.
3. `150` will be printed. On the last iteration of the for loop, `discountePrice = 150` as we found in question 2. Then, the calculation on line 8 will result in a value of `150` as well. `finalPrice` is declared on the base level of the function and so there is no conflict in scope.
4. The function will return the array `[50, 100, 150]`. For every number in the input array `prices`, the function calculates that number times the difference between 1 and the discount parameter, then rounds the value as shown on line 8. This result is pushed to `discounted`. Since the input array is `[100, 200, 300]` and the input discount is `0.5`, this is simply half of each value in the input.
5. The code will throw an error. The only `i` in the function is block scoped to the for loop on line 6, so it is inaccessable from line 12, which is outside the loop.
6. The code will throw an error. The only `discountedPrice` in the function is block scoped to the for loop on line 6, so it is inaccessable from line 13, which is outside the loop.
7. The function will print `150`. The value is calculated by the same logic as question 2. Since `finalPrice` is declared in the main body of the function, it does not matter whether it is block scoped or function scoped, and therefore there is no difference in the result from question 2.
8. this function will return the array `[50, 100, 150]`. The logic operates the same as question 4. The change of each variable from function scoped to block scoped does not affect the output of the function, since each variable is accessed in the same scope from which it was declared.
9. The code will cause an error for the same reason as 5.
10. The code will print `3`. The code does not have scope or reassignment errors so it is printed correctly.
11. The array `[50, 100, 150]` will be returned. The calculation is the same as question 4 and there are no reassignment or scope errors in the code. `const` means that the variable cannot be reassigned, not that it cannot be manipulated, so `discounted` and `length` are both fine. Each iteration of a for loop destroys and creates `discoutnedPrice`, to that constant variable is also not actually reassigned either. So, the function works.
12. A. `student.name`\
    B. `student.['Grad Year']`\
	C. `student.greeting()`\
	D. `student['Favorite Teacher'].name`\
	E. `student.courseload[0]`
13. A. `32` 2 was implicitly cast to a string so the plus operator concatenates them.\
    B. `1` the minus operator caused 3 to be automatically converted to an integer so the value of 3 - 2 = 1 was set\
	C. `3` null is converted to 0 by the plus operator for math, so 3 + 0 is 0\
	D. `3null` null is converted to the string 'null' and concatenated with the string '3'\
	E. `4` true is converted to the number 1 so we have 3 + 1 = 4\
	F. `0` false is converted to the number 0 and null is then converted to 0 so we have 0 + 0 = 0\
	G. `3undefined` undefined is converted to a string because '3' is a string and the plus operator concatenates them\
	H. `NaN` the minus operator wants to convert the two terms to numbers, but undefined is not a number so the number `NaN` is returned.
14. A. `true` String '2' becomes number 2 and comparison occurs\
	B. `false` The two values are compared as strings so in lexigraphical order, '2' comes after '12'\
	C. `true` String 2 becomes number 2 so they are equal since `==` does type conversion before comparison\
	D. `false` `===` does not do type conversion so they are not equal\
	E. `false` true is converted to 1 and they are not equal\
	F. `true` the boolean function converts any singular value to true, and so the comparison is true
15. `==` does type conversion before comparison and `===` does not.
16. js file
17. The function returns `[2, 4, 6]`. For each item in the input array the function runs `doSomething` on the number in the array and then pushes the item into the output array. This results in an array of the values of the input doubled.
18. js file
19. output:

```
1 
4
3
2
```