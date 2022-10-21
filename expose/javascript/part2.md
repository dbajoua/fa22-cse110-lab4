# part 2 #
1. 3 will be outputted. i is of type var and thus has function scope so its
    accesible anywhere inside the function. i was incremented up to 3 in the function. 

2. 150 will be outputted. Upon the end of the for loop, discountedPrice contains
    150, evaluated from the last value marked down 300. discountedPrice is of 
    type var and thus has function scope so its accesible anywhere inside the function.

3. 150 will be outputted. Upon the end of the for loop, finalPrice contains
    150, evaluated from the last value to be marked down 300. discountedPrice is of 
    type var and thus has function scope so its accesible anywhere inside the function.

4. The function returns the discounted array. discounted is of type var, and 
   can be accessed anywhere inside the function its defined. The return statement 
   was within the function.

5. Will get reference error for i not being defined. Since i is of type let, it's
only accessible in the block its defined in, not outside where line 12 is.

6. Will get reference error for discountedPrice not being defined. Since 
    discountedPrice is of type let, it's only accessible in the block its defined in, 
    not outside where line 13 is.

7. finalPrice outputs 150. It is of type let, and line 14 is accessible because
    console.log(finalPrice) is in the same block.

8. The function returns the discounted array. discounted is of type let, but
   the return statement is in the same block and thus the variable was accessible. 

9. Will get reference error for i not being defined. Since i is of type let, it's
   only accessible in the block its defined in, not outside where line 11 is.

10. 3 gets printed. length is of type const, which is the same scope as let. length is 
    accesible within the block its defined in, thus line 12 gets printed as its in the 
    same block.

11. the function returns the discounted array. discounted is of type const, which is 
    the same scope as let (block scope). The return statement is in the same block as 
    discounted is defined in, and thus could access discounted.

12. A: student.name;
    B: student['Grad Year'];
    C: student.greeting(); 
    D: student['Favorite Teacher'].name;
    E: student.courseLoad[0];

13. A: '32', integers map to their exact string representation
    B: 1, 
    C: 3, null becomes 0. 3-0 '= 0
    D: 3null, null becomes a string
    E: 4, true becomes 1. true + 3 = 4
    F: 0, false and null become 0
    G: 3undefined, undefined becomes a string
    H: NaN, undefined becomes NaN

14. A: true, string '2' becomes number 2, so 2 > 1
    B: false, dictionary comparison. first char '2' greater than first char '1'
    C: true, string '2' becomes number 2, so they're equal
    D: false, === doesn't do type conversion, so 2 does not equal '2'
    E: false, true equals 1
    F: true, values considered "empty" like 0, null, undefined make Boolean false.
            other values are considered true like 2.
    
15. === is a strict equality operator meaning it checks equality without type 
    conversion. 
    == is a regular equality operator, and tries to convert operands of different
    types to compare them.

16. 
    let statistics = {
    redCars: 21,
    blueCars: 45,
    greenCars: 12,
    raceCars: 5,
    blackCars: 40,
    rarecars: 2


    };

    for (const car in statistics) {
         if (  car[0] == "r"  ||  statistics[car] % 2 != 0 ) {
             console.log(statistics[car]);
         }  
    }

17. The array [1,2,3] creates newArr [2,4,6]. We start by passing in 2 arguments
    into the modifyArray function, array and callback. callback is used to pass
    in a function as an argument for another function. For each iteration of the
    for loop, callback executes function doSomething which multiplies num by 2.
    Thus, each element added to newArr is the result of what is returned from the 
    doSomething function. Finally, we get our newArr [2,4,6].