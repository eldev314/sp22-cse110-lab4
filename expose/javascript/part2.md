# Part 2

### Variables and Scope

1. It will print 3 to the console because that's the value of i after the loop, and since it was declared with var then the scope is valid

2. It will print 150 to the console because that's the value of discountedPrice on the last iteration of the for loop, and since it was declared with var then the scope is valid

3. It will print 150 to the console because that's the value of finalPrice after the last iteration of the for loop

4. The function will return [50, 100, 150] because the function works as intended and all it does is apply the input discount to the input prices to return an array of the discounted prices. [100, 200, 300] with a discount of 0.5 (50%), will give us [50, 100, 150], which is what we also find when we trace through the code with these input values

5. This code will result in an error at line 12 because i is not declared in the scope at that line. Because it was declared with let in line 6, it's not valid to access it at line 12.

6. This code will result in an error at line 13 because discountedPrice is not declared in the scope at that line because it was declared with let at line 7 in the for loop, so it's not valid to access it at line 13.

7. Line 14 will print 150 to the console because even though finalPrice was declared with let, it was declared in the same scope so finalPrice is able to be accessed at line 14, and as mentioned previously 150 is the value of finalPrice after the for loop finishes executing.

8. The function will return [50, 100, 150] because the function works as intended and all it does is apply the input discount to the input prices to return an array of the discounted prices as described in answer 4. By declaring the variables with let instead of var, the function still works as intended, it just changes the scope of some of the variables to no longer be able to be printed at certain points. 

9. This code will result in an error at line 11 because i is not in the scope at that line. Because it was declared with let in line 6, it's not valid to access it at line 11.

10. Line 12 will print 3 to the console because length = prices.length = 3 and it's valid to access the variable length at line 12.

11. The function will return [50, 100, 150] because the function still works as intended and all it does is apply the input discount to the input prices to return an array of the discounted prices as described in answer 4. Even though the array is declared with const, the elements in the array can still be modified so we can push elements to it without problem because of how js works, which allows the function to work as intended.

### Data types

12.
- A: `student.name`
- B: `student['Grad Year']`
- C: `student.greeting()`
- D: `student['Favorite Teacher'].name`
- E: `student.courseLoad[0]`

### Operators and Type Conversion
13. 

- A: '3' + 2 = "32"  
Explanation: When using the + operator with a string and a number, js converts the number to a string and concatenates the two strings together.

- B: '3' - 2 = 1  
Explanation: When using the - operator with a string and a number, js converts the string to a number and performs the subtraction.

- C: 3 + null = 3  
Explanation: In js when using the + operator, the null is treated as a 0.

- D: '3' + null = "3null"  
Explanation: When using the + operator in js with a string and null, null is converted to the string "null" and concatenated with the string '3'

- E: true + 3 = 4  
Explanation: When using the + operator with a boolean and a number, js converts the boolean true to the number 1 and performs the addition normally after

- F: false + null = 0  
Explanation: When we use the + operator with a boolean and null, both of them are treated as 0

- G: '3' + undefined = "3undefined"  
Explanation: js converts undefined to the string "undefined" and concatenates it with the string '3'

- H: '3' - undefined = NaN  
Explanation: undefined is converted to NaN and any operation involving NaN always results in NaN.


14. 

- A: '2' > 1 -> true  
Explanation: js converts the string '2' to the number 2 and compares it to the number 1, which evaluates to true.

- B: '2' < '12' -> true  
Explanation: js compares the character codes of the corresponding characters from left to right, and '2' is less than '1' so the comparison evaluates to true.

- C: 2 == '2' -> true  
Explanation: js converts the string '2' to the number 2, which is then compared to 2, so the comparison evaluates to true.

- D: 2 === '2' -> false  
Explanation: The === operator convert '2' to 2, so the comparison between a number and a string evaluates to false.

- E: true == 2 -> false  
Explanation: js converts true to 1, so the comparison is between 1 and 2, which evaluates to false.

- F: true === Boolean(2) -> false  
Explanation: No type conversion, so the comparison between a boolean and the boolean value of 2 evaluates to false

15. In js, both == and === are used to check for equality but the == operator performs type coercion, meaning it tries to convert the operands to the same type before comparison. On the other hand, the === operator does not perform type coercion and only returns true if the operands are of the same type and have the same value.

### Loops

16. Code is in [part2-question16.js](part2-question16.js)

### Functions

17. The `modifyArray` function takes an array and a callback function as parameters. The function then creates a new empty array `newArr` and iterates through the input array using a for loop, passing each element to the callback function and pushing the resulting value to the `newArr`. In this case, the input array `[1, 2, 3]` is passed along with the `doSomething` callback function, which simply multiplies each element by 2. Therefore, the `newArr` that is returned consists of `[2, 4, 6]`, since each element in the input array was doubled by the callback function. Finally, this `newArr` is printed to the console using `console.log`.

18. Code is in [part2-question18.js](part2-question18.js)

19. The output of the code is
```
1
4
3
2
```