**Part 1a**
1. Line 9 prints    values added: 20
2. Line 13 prints   final result: 20
3. Line 9 prints    values added: 20
4. Line 13 returns an error because the result variable only exists in the scope of the if statement.
5. Line 9 returns an error because we are reassigning a constant on line 7.
6. Line 13 returns an error because the result variable only exists in the scope of the if statement.
   
**Part 1b**
1. Line 12 will print the value of i which is 3 to the console. This will occur because var i exists outside of the for loop which exits after 3 loops because the length of the price array is 3.
2. Line 13 will print the value of discountedPrice which is 150 to the console. This will occur because the variable exists outside of the for loop it was declared in. The variable can also be reassigned. The last thing the variable is assigned is prices[2] * (1 - 0.5) which is 300 * 0.5 = 150.
3. Line 14 will print the value of finalPrice which is 150. The variable finalPrice can be altered in the for loop, holding the final discounted price of each number in the array in each loop. The last loop of the for loop saw discountedPrice = 150, where we then multiply by 100 to get 150000 and then divide by 100 back to 150. We round this to the nearest integer which is just 150 again.
4. The function will return the array discounted, [50, 100, 150]. The array is a var and is used in the for loop to store the final price of each value in the input variable *prices* after the applied discount. We push the final price at the end of each loop onto the array on line 9.
5. The code causes an error because the variable *i* is declared using the *let* keyword in line 6 which means that it exists only in the scope of the for loop. We are printing a variable that does not exist in the scope of line 12.
6. The code causes an error because the variable *discountedPrice* is declared using the *let* keyword in line 7 which means that it exists only in the scope of the for loop. We are printing a variable that does not exist in the scope of line 13.
7. Line 14 will print the value of finalPrice which is 150. The variable finalPrice can be altered in the for loop because it was declared on the global scale on line 4. The variable holds the final discounted price of a number. The last loop of the for loop saw discountedPrice = 150, where we then multiply by 100 to get 150000 and then divide by 100 back to 150. We round this to the nearest integer which is just 150 again.
8. The function will return the array discounted, [50, 100, 150]. The array was declared using the *let* keyword in the global scope on line 3. Thus, the push operation done on line 9 works the same way as if the array was declared using *var* as explained in the answer to question 4.
9. The code causes an error because the variable *i* is declared using the *let* keyword in line 6 which means that it exists only in the scope of the for loop. We are printing a variable that does not exist in the scope of line 11.
10. Line 12 prints the constant variable which was assigned the length of the prices input array on line 4. In this case, the input array was of length 3 so line 12 prints the number 3.
11. The function returns the discounted array [50, 100, 150] as explained in the previous iterations of this question. However, it is important to notice that we are able to *manipulate* const variables, such as pushing to an array, but not *reassign* them. 
12. a) student['name']
    
    b) student['Grad Year']

    c) student.greeting()

    d) student['Favorite Teacher'].name

    e) student.courseLoad[0]
13. a) '32' because joining 2 to '3' concatenates 2 as a string, automatically applying string conversion
    
    b) 1 because numeric conversion is applied to non-numbers, in this case subtraction to '3'

    c) 3 because numeric conversion is applied to null which becomes 0

    d) '3null' because joining null to '3' concatenates null as a string, automatically applying string conversion

    e) 4 because numeric conversion is applied to true which becomes 1

    f) 0 because numeric conversion is applied to false and null, both becoming 0

    g) '3undefined' because joining undefined to '3' concatenates undefined as a string, automatically applying string conversion

    h) NaN because numeric conversion is applied to '3' which becomes 3 and undefined which becomes NaN
14. a) true because when comparing different types, JavaScript converts the values to numbers and 2 > 1

    b) false because we compare strings in lexicographical order and 2 is greater than 1

    c) true because when comparing different types, JavaScript converts the values to numbers and 2 == 2
    
    d) false because a strict equality check returns false if the compared types are different

    e) false because when comparing different types, Javascript converts the values to numbers and 1 != 2

    f) true because Boolean(2) is true and true ==== true is true.
15. == is an equality check that converts any non-numbers into numbers when compared to a number.
    
    === is a strict equality check that does not convert anything and returns false on type mismatch
17. The function will return an array [2, 4, 6]. We came to this conclusion by tracing the function. We create a newArr and loop 3 (the length of input array [1, 2, 3]) times. In each of these loops, we call the callback function doSomething on each number in the input array which multiplies the input number by two. We push the result into newArr and return it after we exit the loop.
19. The output of the above code is, in descending order, 1 4 3 2. The console prints 1, 4 and waits 1 second and 0 seconds to print 2 and 3 respectively.