# csis10a-final-review

## Instructions

For these problems you will be working alone.

Clone this repository and on in BlueJ, Visual Studio Code, or your favorite IDE

### Problem 1 - Create a Point class

You will need to create a class named Point that will represent 2D cartesian coordinates

Do the following:

1. Create a class called `Point`
2. Add private instance variables to your Point class called `x` and `y` of type `double`
3. Create a no-arg constructor
4. Create a parameterized constructor that takes x and y
5. x and y should be encapsulated. Create accessor (get) and mutator (set) methods for x and y
6. Override the `toString` method so that it returns a string in the format of `(x, y)`, where x, and y are the instance values for the point. The signature of toString is `public String toString()`
7. Override the `equals` method so that it compares the x and y values with those of another point. The signature of equals is: `public boolean equals(Object obj)`

### Problem 2 - Equality vs. Reference checking

Do the following:

1. Create a class called `PointCheck`
2. Create a main method. You should be able to rattle the signature off in your sleep by now, but just in case: `public static void main(String[] args)`
3. In your main method, create 3 instances of your point class with the following values:
    1. x = 2, y = 4
    2. x = 2, y = 4 // yes the same value
    3. x = 4, y = 2
4. Also in your main method use reference checking _and_ equality checking to compare point #1 with points #2 and #3. You should print out the result of each in a user-friendly manner.
5. Run `PointCheck` using 

### Problem 3 - Arrays

Do the following:

1. Create a class called `PointMover`
2. Create a main method.
3. Inside the main method create an array to hold 20 Points.
4. Write a for loop to fill the array of points where `x` starts at 20 and goes to 39, `y` should start at 39 and go to 20. e.g. #1 is (20, 39), #2 is (21, 38), #3 is (22, 37) ... #20 is (39, 20)
5. Write a for loop to changes the y value of every other point in the array to 10.5. For example, the first point in the array will be unchanged. The second point will become (21, 10.5). The third point will be unchanged. The forth point will be (23, 10.5), etc.
6. Write a for loop that interates over the array of points and prints out any point with an x value between 25 and 30. Make sure you are using the points toString method when printing.
7. At the end of your main method, print out the 6th point in your array using the points toString method.

### Problem 4 - Garbage Collection

Do the following:

1. Create a class called `PointGC`
2. Create a main method.
3. Inside the main method create 2 variables that point at 2 different point instances
4. Create an alias variable to one of your points.
5. Now add code that can cause one of your point instances to be garbage collected.