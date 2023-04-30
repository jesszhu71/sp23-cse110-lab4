## Part 2

1. At line 12, the code prints out **"3"**. This is because there are three elements in the array parameter being passed into the function discountPrices() which makes the for loop end when variable i, which has functional scope, is greater than or equal to 3. So when the for loop ends, i = 3, thus making the function print "3". 
2. At line 13, the code prints out **"150"**. This is because in the last iteration of the for loop, line 7 assigns discountedPrice = 300 * (1 - 0.5). Since discountedPrice has a functional scope, at line 13, discountedPrice still takes on the value 150 and so that prints out 150 to console. 
3. Line 14 prints out "150" as well. Similar to question 2, the last iteration of the loop is still the same. At line 8, the final iteration of the loop assigns finalPrice to the value of Math.round(150*100)/100, which essentially rounds a number as you would with money. Since finalPrice has a functional scope, at line 14, finalPrice still takes on the value 150 and so that prints out 150 to console. 
4. This function will return the array **[ 50, 100, 150 ]**, which are the corresponding new values of the input prices after being discounted using the specified discount. In each iteration of the for loop, line 9 adds the new calculated value of each original price into the new array, so array that gets returned contains each of the values calculated at line 9. 
5. An **error** is thrown at line 12. Because the variable i is created within the scope of the for loop, once we are outside in line 12, it no longer exists and will throw an error for referencing an undefined variable. 
6. An **error** is thrown at line 13. Because the variable discountedPrice is created within the scope of the for loop, once we are outside in line 13, it no longer exists and will throw an error for referencing an undefined variable. 
7. At line 14, the code prints out **"150"**. The variable finalPrice is created on line 4 and has block scope. The for loop from line 6-10 alters this value and in the last iteration of the for loop, it takes on the value of 150. Since line 14 is within the same scope that finalPrice was created in, it will print 150. 
8. This function will return the array **[ 50, 100, 150 ]**, which as the corresponding new values of the input prices after being discounted using the specified discount. Line 1 creates discounted to have block scope, and since the return statement is the same scope, it should contain the new values that are being created in the for loop. In each iteration of the for loop, line 9 adds the new calculated value of each original price into the new array, and so the array that gets returned contains each of the values calculated at line 9. 
9. The code will have an **error**. Line 11 should throw an **error** since the variable i has block scope and does not exist outside the for loop. Thus at line 11 i doesn't exist and throws an error for referencing an undefined variable. 
10. Line 12 prints out the value of length **"3"** as it doesn't get altered anywhere in the code and it is in the same scope. It is defined on line 4. 
11. The function returns the array [ 50, 100, 150 ]. The array discounted is of const type, but because the const is how the array is referenced we can still alter the contents of the array. Since the for loop populates the array with the new price values with the discount, that is what gets returned. 
12. how to:
    a. student.name
    b. student["grad year"]
    c. student.greeting()
    d. student["Favorite Teacher"].name
    e. student.courseLoad[0]
13. arithmetic
    a. 32
    b. ERROR
    c. 3
    d. ERROR
    e. 4
    f. 0
    g. 3undefined
    h. NaN
14. comparison
    a. true
    b. ERROR
    c. ERROR
    d. ERROR
    e. false
    f. true
15. "==" operator checks whether the items on each side of the comparison are equal and returns a boolean. It will convert data types to compare operands that are of different types. The "===" operators also checks whether the items on each side of the comparison are equal, but this operator does not convert data types if they are different, meaning that both operands must be of the same type to be true. 
16. (code)
17. We are passing in an array and a function into the modifyArray function. In line 2, we create an empty array newArr. Line 3 we iterate through the parameter array, and call the callback function, doSomething, for each item in the array and aadd it to the newArr. Then we return the newArr which contains an array with the transformed numbers. 
18. (code)
19. 1
    4
    3
    2
    