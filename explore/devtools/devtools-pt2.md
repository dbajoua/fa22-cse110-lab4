# devtools part 2 #
1. The bug was that num1 and num2 were strings that when added together resulted in a string. Ex. "2" + "3" = "23". 
   This is wrong as the goal was to sum to values such that we get 5.
2. To fix the bug, num1 and num2 needed to be summed as ints such as that result would become their summed 
   integer value. This could be fixed by replacing line 11 to let result = parseInt(num1) + parseInt(num2).