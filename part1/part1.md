## Part 1a 

1. 20
2. 20
3. 20
4. Error; the variables declared with let keyword have the block scope ({}). The `result` variable is declared inside the if block. It cannot be accessed from outside the block. 
5. Error; const variable cannot be reassigned. 
6. Error; const variable cannot be reassigned. 

## Part 1b
1. 3; var `i` increments to 3 and has function scope
2. 150; var `discountedPrice` has function scope and is finally assigned to the result of `prices`[2] * (1 - `discount`), which is at the last (3rd) iteration of the for loop
3. 150; var `finalPrice` has function scope and is finally assigned to the result of Math.round(`discountedPrice` * 100) / 100, where `discountPrice` is assigned to `prices`[2] * (1 - `discount`), which is at the last (3rd) iteration of the for loop
4. [50, 100, 150]; there are 3 iterations of for loop in total as length of `price` is 3. At each iteration of for loop, `finalPrice` is calculated and pushed to the array `discounted`. For example, at the 1st iteration, given `price`[0] and `discount`, `finalPrice` is 50 and it's pushed to `discounted`. And so on until for loop terminates. 
5. Error; let `i` is defined inside the for loop block. It cannot be accessed outside tha block. 
6. Error; let `discountPrice` is defined inside the for loop block. It cannot be accessed outside that block. 
7. 150; let `finalPrice` is defined at line 4, and it's in the block of whole function, so that it can be accessed at line 14. Also, `finalPrice` is finally assigned to the result of Math.round(`discountedPrice` * 100) / 100, where let `discountPrice` is assigned to `prices`[2] * (1 - `discount`), which is at the last (3rd) iteration of the for loop
8. [50, 100, 150]; let `discounted` is defined at line 3, and it's in the block of whole function. There are 3 iterations of for loop in total as length of `price` is 3. At each iteration of for loop, `finalPrice` is calculated and pushed to the array `discounted`. For example, at the 1st iteration, given `price`[0] and `discount`, `finalPrice` is 50 and it's pushed to `discounted`. And so on until for loop terminates. 
9. Error; let `i` is defined inside the for loop block. It cannot be accessed outside tha block. 
10. 3; const `length` is defined at line 4, and it's in the block of whole function so that it can be accessed at line 12. 
11. [50, 100, 150]; there are 3 iterations of for loop in total as const `length` = 3. At each iteration of for loop, const `discountedPrice` is assigned and pushed to the array `discounted`. `discountedPrice` only exists inside this block in this iteration. For example, at the 1st iteration, given `price`[0] and `discount`, `discountedPeice` is 50 and it's pushed to `discounted`. And so on until for loop terminates. 
12. A.  student['name']  
    B.  student['Grad Year']  
    C.  student.greeting()  
    D.  student['Favorite Teacher'].name  
    E.  student.courseLoad[0]  
13. A. '32'  
    B. 1  
    C. 3  
    D. '3null'  
    E. 4  
    F. 0  
    G. '3undefined'  
    H. NaN  
14. A. true
    B. false
    C. true
    D. false
    E. false
    F. true
15. == operator compares the numeric values between two variables. === operator not only compares the numeric values between two variables, but also the type of two variables. 
16. See part1b-question16.js for details
17. [2, 4, 6]; Here the callback function `doSomething` basically doubles the input variable and then returns it. In the function `modifyArray`, it firstly initializes an array `newArr`. Then, there are 3 iterations of for loop in total as the length of array is 3. At each iteration, the result of callback(array[i]), which is `doSomething`(array[i]), is pushed to the array `newArr`. And so on until the for loop terminates. Finally, it returns `newArr`. 
18. See part1b-question18.js for details
19. 1  
    4  
    3  
    2  