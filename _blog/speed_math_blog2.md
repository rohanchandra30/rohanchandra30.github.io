---
layout: blog
name: Squaring Made Easy
description: This article presents an easy way of being able to compute two digit squares of the form 10x + y where x lies between 0 and 9 and y is greater than 5, x and y being integers. The content and idea in this paper is based on a very common Vedic math shortcut of squaring two digit numbers.
---

For Vedic mathematicians and enthusiasts, it is very important to be able to compute two digit squares quickly as it forms the basis for most advanced mental computations like squaring of 3 digit and 4 ¬digit numbers. The following example illustrates the importance of being able to square a 2 digit number quickly.

####Example 1:   

The technique used to compute this problem is as follows:

1.)	We need to round 653 to the nearest hundred. So we add and subtract 47 from 653 to get 700 and 606.  
2.)	Multiply the 606 and 700 to arrive at 424200.  
3.)	We next simply add   to 424200 to get the final answer as 424200 + 2209= 426409  

From step 3 it can be observed that while calculating 606 times 700 may be easy, calculating   while keeping in mind the result of 606 times 700 that is, 424200 may be a bit difficult. But what if there was a way to easily calculate 47x47. It would make the computation of  so much easier.  
Almost in all the literature, the Vedic math shortcut is universal. It is the deviation method where you:  

1.)	Take the distance of the given number from the nearest multiple of ten and add and subtract that distance from the number.  
2.)	Multiply the two numbers and add the square of the distance to get the final answer.

####Example 2:  
1.)	Add and subtract the distance 3 to get 90 and 84  
2.)	Multiply the two to get 7560 and add   to get 7569

###II.	AN EASY WAY TO USE THE DEVIATION METHOD

The method in this article is based on the following algebraic manipulation:
 , where .    			(1)
R.H.S of (1) =   which is equal to L.H.S.
Using the above formula, we reduce a multiplication problem to that of a simple addition problem. The simplicity of the formula lies in the fact that we do not have to plug in values and calculate every time. There is a pattern based on this formula and once the pattern is understood, this method becomes a much easier scenario of adding three numbers together.
From (1) let   be A,   be B,   be C. Values for A, B and C are given in table 2. 
The pattern is explained with the help of the following table:
[The table can be found in this article](https://drive.google.com/file/d/0B6liApN8RVRnQXgtbGxYZ2RhQjA/view?usp=sharing)

After studying the pattern and correlating it with the formula, we infer that for A and C, no heavy calculations are needed and can be figured out almost instantly. 
For B, it will take some to practice and get the hang of it but after a while one can see that all we are doing is first taking  and multiplying it with 10 and doubling it. We then make use of our new found understanding of the pattern and figure out how far  is from  and multiply it with that distance.  
This will become clear through the following two examples:

####Example 3:  
1.)	Find A: Multiply 6 and 7 and append two 0’s to get 4200.
Find C: The unit’s digit is 8, therefore C will be 4 (from table 2)  
2.)	Find B: 
Take 7 and multiply it first by 10 and then by 2 to get 140. 68 is 3 units away from 65. So multiply 140 by 3 to get 420  
3.)	Add A, B and C to get the final answer. 4200 + 420 + 4 = 4624.  

####Example 4:  
1.)	Find A: Multiply 4 and 5 and append two 0’s to get 2000.
Find C: The unit’s digit is 6 therefore C will be 16 (from table 2)  
2.)	Find B: 
Take 5 and multiply it first by 10 and then by 2 to get 100. 46 is 1 unit away from 45. So multiply 100 by 1 to get 100.  
3.)	Add A, B and C to get the final answer. 2000 + 100 + 16 = 2116.
