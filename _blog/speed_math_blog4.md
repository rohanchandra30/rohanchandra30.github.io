---
layout: blog
name: Divisibility tests of primes upto 100
description: Here's a different way of checking whether an N digit number is divisible by a prime number below 100.
---

I.	THE METHOD

Here is a list of divisibility tests for all primes up to 100 (except 2). The tests here are different from conventional tests. With these rules, not only can you check its divisibility, you can also find the remainder.
The rules say that for each prime p, say for a four digit number N, we use a specific set of base number for each digit. We multiply each digit by its corresponding base number and add the product. If the result is divisible by p, then the N is divisible by p.

####Example 1:
Let N=8497 and p=17
The base numbers are 1 for units digit, 10 for tens, -2 or 15 for hundreds (whichever’s easier to you), and -3 or 14 for the thousands place. For simplicity, we can use the last two digits of N as it is. This is applicable for all p > 13.
Let’s get started.
8 times -3 = -24 as remainder or +10 
4 times -2 = -8 as remainder
97 gives 12 as remainder.
Add all these to get (+10) + (-8) + (12) to get 14 as remainder which is not divisible by 17. Hence 8497 is not divisible by p.

The final remainder when we divide N by p is the result obtained by adding the individual remainders calculated by using the base number. In this case, it is 14

####Example 2:
Let’s divide 7896 by 7
The base numbers are 6, 2, 3 and 1
7 times 6 is 42 which leaves remainder 0
8 times 2 is 16 which leaves remainder 2
9 times 3 is 27 which leaves remainder 6
6 times 1 is 6 which leaves remainder 6
Adding them up gives 14 which is divisible by 7. 
Hence, 7896 is divisible by 7.
The final remainder when we divide N by p is the result obtained by adding the individual remainders calculated by using the base number. However, in the case, when the final sum of these remainders is a multiple of p, then the remainder of Nmodp can be taken as zero.


II .DETERMINATION OF BASE NUMBERS

We can generalize a 4-digit number ABCD by adding the 4 components 1000A +100B +10C +D. Finding ABCDmodp, where p is a prime number, is the same as finding the remainder for the 4 components separately and adding them together.
Calculations of base numbers are done by manual testing. For testing divisibility of ABCD by a prime number, p, we primarily determine 1000modp, 100modp, 10modp and so on. The resulting digits become the base numbers.
To perform the divisibility test, we simply multiply 1000modp by A, 100modp by B, 10modp by C, and 1 by D. This can be summarised by the following property of modular arithmetic,
 

Here, we take a = A, n = p, b = 1000, 100, 10 and 1.

Let us consider the first example we took.
Test the divisibility of 8497 by 17.

Here, A = 8, B = 4, C = 9, and D = 7. 
p = 17.
To find the base digits, we find 1000mod17, 100mod17, 10mod17 and 1mod17. These are given as 14 or -3, 15 or -2, 10 and 1 respectively. 



III. EXTENSION FOR AN N DIGIT NUMBER

The following list in this article is limited to a 4 digit number. However, the method works for any large number. In this section, a shortcut will be explained to calculate base numbers for any N digit number.
Method:  Let the N digit number be ,
Where n = N and 0   9

Step 1: first figure out 10modp.  
Step 2: for subsequent base numbers, simply perform    where i   2. 

####For example, for p = 7,
10modp or the base number for the 10th place is 3. The base numbers for the subsequent digits can be found by first analysing   for the 100th, 1000th …place in N
Step 3: The base numbers for the 100th 1000th …places in N can thus be shown as ... and so on.
Step 4: To test divisibility, simply follow the method 
 The base number for the 100th, 1000th place for p = 7 can be found as   … and so on, which is far easier than calculating 100modp and 1000modpas done in the previous section.

IV.	MAKE IT EASIER WITH VEDIC MATHS!

The principle used in this article can be strongly related to that by “Shesanyankena Charamena” or “Remainder by the last digit”. This is the twelfth Vedic Math sutra and is essentially multiplying each digit by a remainder.
The Shesanyankena Charamena can be explained in the following example:
Example:

####Express 1/7 as a decimal

1.) Add 'zero' to the numerator which makes 1 as 10  
2.) If the numerator is less than the denominator, add another ‘zero’, else proceed as follows ...  
3.) Divide: (10)/7 = 1 remainder 3  
4.) Adding zero to the remainder (since it is less than the denominator), we divide as (30)/7= 4 remainder 2  
5.) We continue taking the remainder the following the steps from the start as follows:

 (20) /7 = 2 remainder 6  
 (60) /7 = 8 remainder 4  
 (40) /7 = 5 remainder 5  
 (50) /7 = 7 remainder 1

6.) Now note that the remainder is '1' which is same as the numerator '1'.This means we would get the repetition of the answers again and again. So we will stop here.  
7.) Using the numbers (remainders) 3, 2, 6,4,5,1 got above, we multiply them with the denominator '7',

7 x 3 = 21  
7 x 6 = 42  
7 x 4 = 28  
7 x 5 = 35  
7 x 1 = 7  

8.) Now we take the red shaded numbers from the above steps as sequence, 142857 (which would be our final result)

Therefore, Result (1/7) = 0.142857142857

The process of multiplying an integer by a remainder as is the case in step 7 in the example above can be tweaked and used in my principle used in this article. In the second example of section 1,

7 times 6 is 42 which leaves remainder 0  
8 times 2 is 16 which leaves remainder 2  
9 times 3 is 27 which leaves remainder 6  
6 times 1 is 6 which leaves remainder 6

can be shown to be using Shesanyankena Charamena once compared to the example given in this section.
Sometimes it might be hard and/or time consuming to find remainders when dealing with large numbers. The complexity occurs when we have to perform division of these large numbers to figure out the remainder.
In such scenarios, we can use several Vedic math techniques to help us in our calculations.
We can employ the following Sutras to help us divide large numbers quickly:

1.)	Nihilam Sutra : This is a specific method of division in Vedic Maths which gives us a trick to divide numbers when the divisor is closer to a power of ten but less than ten. We can use this when dealing with primes like 7 or 5.  
2.)	Paravartya Sutra:  This is a specific method of division in Vedic Maths which gives us a trick to divide numbers when the divisor is closer to a power of ten but greater than ten. We can use this when dealing with prime numbers like 97. 

We can make use of some other relatable Sutras like Anurupyena and Vinculum when the above Sutras don’t apply.

V.	LIST OF BASE NUMBERS

Following is a list of all primes up to 100 (except 2) and their corresponding base numbers. For sake of demonstration I have taken a 4 digit N.

[The list can be found in this article](https://drive.google.com/open?id=0B6liApN8RVRnRHBldzlsX3VJWGs)
