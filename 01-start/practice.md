## 练习题

### 1. 计算距离
> Write the function distance(x1, y1, x2, y2) that takes four int or float values x1, y1, x2, y2 that represent the two points (x1, y1) and (x2, y2), and returns the distance between those points as a float.
>> distance(x1, y1, x2, y2)



### 2. 两圆是否相交
>Write the function circlesIntersect(x1, y1, r1, x2, y2, r2) that takes 6 numbers (ints or floats) -- x1, y1, r1, x2, y2, r2 -- that describe the circle centered at (x1,y1) with radius r1, and the circle centered at (x2,y2) with radius r2, and returns True if the two circles intersect and False otherwise.
>> circlesIntersect(x1, y1, r1, x2, y2, r2)  


### 3. getInRange(x, bound1, bound2)  
> Write the function getInRange(x, bound1, bound2) which takes 3 int or float values -- x, bound1, and bound2, where bound1 is not necessarily less than bound2. If x is between the two bounds, just return it unmodified. Otherwise, if x is less than the lower bound, return the lower bound, or if x is greater than the upper bound, return the upper bound. For example:
> - getInRange(1, 3, 5) returns 3 (the lower bound, since 1 lies to the left of the range [3,5])
> - getInRange(4, 3, 5) returns 4 (the original value, since 4 is in the range [3,5])
> - getInRange(6, 3, 5) returns 5 (the upper bound, since 6 lies to the right of the range [3,5])
> - getInRange(6, 5, 3) also returns 5 (the upper bound, since 6 lies to the right of the range [3,5])

#### 4. isFactor(f, n)
> Write the function isFactor(f, n) that takes two int values f and n, and returns True if f is a factor of n, and False otherwise. Note that every integer is a factor of 0.


#### 5. isLegalTriangle(s1, s2, s3)
> Write the function isLegalTriangle(s1, s2, s3) that takes three int or float values representing the lengths of the sides of a triangle, and returns True if such a triangle exists and False otherwise. Note from the triangle inequality that the sum of each two sides must be greater than the third side, and further note that all sides of a legal triangle must be positive. Hint: how can you determine the longest side, and how might that help?

#### 6. triangleArea(s1, s2, s3)
> Write the function triangleArea(s1, s2, s3) that takes 3 floats and returns the area of the triangle that has those lengths of its side. If no such triangle exists, return 0. Hint: you will probably wish to use Heron's Formula.

#### 7. triangleArea(s1, s2, s3)
> Write the function triangleAreaByCoordinates(x1, y1, x2, y2, x3, y3) that takes 6 int or float values that represent the three points (x1,y1), (x2,y2), and (x3,y3), and returns as a float the area of the triangle formed by those three points. Hint: you should make constructive use of the triangleArea function you just wrote above.


#### 8. nearestBusStop(street)
> Write the function nearestBusStop(street) that takes a non-negative int street number, and returns the nearest bus stop to the given street, where buses stop every 8th street, including street 0, and ties go to the lower street, so the nearest bus stop to 12th street is 8th street, and the nearest bus stop to 13 street is 16th street.

#### 9. isEvenPositiveInt(x)
> Write the function isEvenPositiveInt(x) that takes an arbitrary value x, return True if it is an integer, and it is positive, and it is even (all 3 must be True), or False otherwise. Do not crash if the value is not an integer. So, isEvenPositiveInt("yikes!") returns False (rather than crashing), and isEvenPositiveInt(123456) returns True.


#### 10. nthFibonacciNumber(n)
> Background: The Fibonacci numbers are defined by F(n) = F(n-1) + F(n-2). There are different conventions on whether 0 is a Fibonacci number, and whether counting starts at n=0 or at n=1. Here, we will assume that 0 is not a Fibonacci number, and that counting starts at n=0, so F(0)=F(1)=1, and F(2)=2. With this in mind, write the function nthFibonacciNumber(n) that takes a non-negative int n and returns the nth Fibonacci number. Some test cases are provided for you. You can use Binet's Fibonacci Number Formula which (amazingly) uses the golden ratio to compute this result, though you may have to make some small change to account for the assumptions noted above.

#### 11. lineIntersection(m1, b1, m2, b2)
> Write the function lineIntersection(m1, b1, m2, b2) that takes four int or float values representing the 2 lines:
>>    y = m1*x + b1

>>    y = m2*x + b2

>This function returns the x value of the point of intersection of the two lines. If the lines are parallel, or identical, the function should return None.
