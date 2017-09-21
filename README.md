# Devloment-Material



Program Title --- Random number generation


Source Algorithm  ---  Basically we know that, we can generate random number with different- different ways but here we are following a very common algorithm LCG(Linear Congruential Generator ).
https://en.wikipedia.org/wiki/Linear_congruential_generator


Program Algorithm ----

Step 1-  There are two balnk list minlist and maxlist which is use to fill the result data.

Step 2- Execute a loop to 100 time to get the data(from Step 5) from the following generate methods if data is less than 5 than fill into minlist and else if data is greater than 5 than fill into maxlist.

Step 3- There are two argument in generate method first one is modulus and second one is increment.

Step 4 – With the help of generate method we are getting multiplier and seed from a validate_inputs method which has two arguments modulus and increment.

a) validate_inputs method will return multiplier and seed (specific no) . In here multiplier and seed will get from get_seed() method.

b) get_seed() method is using time functions of python for generating a specific seed and multiplier values.

c) In validate_inputs method , we can validate the multiplier and seed using a specific following relation:
             if increment is less than modulus and seed is also less than modulus and multiplier is having 1,3,7,9 (prime no less than 10) than validate_input function will return the multiplier and seeds otherwise not.

Step 5- After getting the multiplier and seed in generate method it will follow the LCG algorithm (Xn = (aXn-1 + c) mod m).
    In the program  
 current_iteration = (current_iteration * multiplier) +    increment     
     if current_iteration > modulus:
     current_iteration %= modulus

 
    

