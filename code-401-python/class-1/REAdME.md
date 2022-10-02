# Big O Notation

### Big O Notation is used to measure or describe the performance of any algorithm by providing the order of growth of the function.
  ![O1&On](https://miro.medium.com/max/581/1*YKanRKXFdrQOIM8BrL3Q7Q.png)



1.**O(1)**: No matter how big your collection is, the time it takes to perform an operation is constant. This is the constant time complexity notation. These operations are as fast as we can get. As an instance, operations that check whether a collection has any items inside it is an O(1) operation.

2.**O(log n)**: When the size of a collection increases, the time it takes to perform an operation increases logarithmically. This is the logarithmic time complexity notation. Potentially optimised searching algorithms are O(log n).

3.**O(n)**: The time it takes to perform an operation is directly and linearly proportional to the number of items in the collection. This is the linear time complexity notation. This is some-what in-between or medium in terms of performance. As an instance, if we want to sum all of the items in a collection then we would have to iterate over the collection. Hence the iteration of a collection is an O(n) operation.

4.**(n log n)**: Where the performance of performing an operation is a quasilinear function of the number of items in the collection. This is known as the quasilinear time complexity notation. Time complexity of optimised sorting algorithm is usually n(log n).

5.**O(n square)**: When the time it takes to perform an operation is proportional to the square of the items in the collection. This is known as the quadratic time complexity notation.

6.**(n!)**: When every single permutation of a collection is computed in an operation and hence the time it takes to perform an operation is factorial of the size of the items in the collection. This is known as factorial time complexity notation. It is very slow.

# Names and Values in Python
----------------------------------


1. **Names in Python are reassigned independently**
2. **Assignments never copies data**
3. **Refrences can be more than names**
4. **Mutable Aliasing**
5. **Values have no scope but a type**
6. **Names has no type but a scope** 
----------------------------------

## Sources 
 1. [Big O Notation](https://medium.com/fintechexplained/time-complexities-of-python-data-structures-ddb7503790ef)