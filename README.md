# EXPERIMENT-08
# <p align="center"> Create a program for Nested Array using JS </P> 
## Aim: 
The aim of the function is to determine whether the first array can be nested inside the 
second array based on specific conditions.
## Algorithm:
1. Initialize two arrays, num1 and num2, with the given values.
2. Set variables a_max and a_min to the first element of num1.
3. Iterate over each element in num1 using a for loop.
• If the current element is greater than a_max, update a_max to the current 
element.
• If the current element is less than a_min, update a_min to the current 
element.
4. Set variables b_max and b_min to the first element of num2.
5. Iterate over each element in num2 using a for loop.
• If the current element is greater than b_max, update b_max to the current 
element.
• If the current element is less than b_min, update b_min to the current 
element.
6. Check if the conditions (a_max < b_max && a_min > b_min) are satisfied:
• If true, return "TRUE".
• If false, return "FALSE".

## Programm:
```
function check()
{
 
 var num1 = [1,2,3,4]
 var num2 = [0,6] 
 
 for(var i = 0; i<num1.length; i+=1)
 {
 a_max = a_min = num1[0];
 if(a_max<=num1[i])
 {
 a_max = num1[i]
 }
 else
 {
 a_min = num1[i]
 }
 }
 for(var i = 0; i<num2.length; i+=1)
 {
 b_max = b_min = num2[0]
 if(b_max<=num2[i])
 {
 b_max = num2[i]
 }
 else
 {
 b_min = num2[i]
 }
 }
 (a_max < b_max && a_min > b_min)?console.log("TRUE"):console.log("FALSE")
}
check.call()
```

## OUTPUT:

![image](https://github.com/Sugan2002/Task-1-21-03-2023-Functions-JS/assets/77089743/a8634240-a9be-4c2d-ab01-90f53a3ebdb2)

## Result:
The function will return "TRUE" if the first array can be nested inside the second array based 
on the conditions, and "FALSE" otherwise.
