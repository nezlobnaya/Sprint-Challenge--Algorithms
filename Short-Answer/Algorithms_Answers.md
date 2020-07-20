#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)
    The time complexity for a = 0 is O(1), since it's simply an assignment operator. The while loop has time complexity O(n)Over all, the result of the input increases as a constant of the input.


b) O(n^2)
 We have entered two for loops that are both n based. The performance is the square of the input data.


c) O(n) 
 It goes down by 1 every time so it will reach n in the same number of runs. Steps required increase with the number of inputs.

## Exercise II
 What we're doing is searching for the highest floor on which the egg won't get broken, 
 we want to find it with lowest number of eggs dropped and broken. Because the floors are sorted, we can use a binary search algorithm to do this.
 
Psuedocode:
    1. lowest flow  = 0
       highest floor = len(n) - 1
    2. While you haven't narrowed it down to one floor, 
        drop an egg from the middle floor n //2
        if does not break return middle floor
    3. Depending on weather the eggs break or not, 
        going down high = mid -1
        or up low = mid +1
         by half of the remaining floors of the building.
    4. At one point we have two consecutive floors checked from which we have different outcomes: egg breaks from the higher of the two, doesn't get broken if dropped off from the lower. These are floor n and floor (n - 1)
     Runtime complexity is O(log n).




