 ## In Tests We Trust — TDD with Python
 
 ### What is test-driven development?
   TDD is a software development technique based on very short recurrent cycles 
    

### AAA Testing
The AAA pattern is a pattern for structuring tests. It breaks each test down into three parts – Arrange, Act, and Assert – where each part is a step leading to the next. The arrange step sets up the test’s input values. The act step prompts the primary function being tested. And finally, the assert step verifies that the output of the function is what was expected.

---

## If name equals main :
##### Pythong files can be excuted in 2 ways : 
- as a Scripts : is a collection of commands in a file designed to be executed like a program.
- as a module : is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 

We use the if __name__ == “__main__” to avoid running codes that should not be excuted when we use the same file in different places (module or script)
In the case of having the file as a module the  __name__ will be module name if not , then the __name__  will be __main__ . 

---

# Recursion 

What is Recursion? 
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function. Using a recursive algorithm, certain problems can be solved quite easily.

Recursion is made for solving problems that can be broken down into smaller, repetitive problems.

#### Why not to use recursion
- It is usually slower due to the overhead of maintaining the stack.

#### Why Recursion

- it Reducing the length of our code and make it easier to read and write, instead of writing a loop.

- Reduces time complexity.

### Sources 


https://developers.mews.com/aaa-pattern-a-functional-approach/
https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/