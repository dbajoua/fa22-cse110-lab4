# part 1 #
1. values added: 20
    Note: result is of type var and thus has function scope

2. final result: 20
   Note: result's value is preserved within function scope

3. values added: 20
   Note: result is of type let and thus has block scope

4. ReferenceError because result is not defined. Since result has block scope,
   it can only be accessed with the block its defined in.

5. TypeError because result is of type const and cannot be reassigned, so 
   result = num1 + num2 is not allowed.

6. line 13 cannot be excuted, line 9 has error. 

