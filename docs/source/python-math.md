# 🖥️ 🔢 PYTHON AND MATH

Throughout contemporary history and since the birth of technology as we know it, it has provided education with innovative tools, which has made it possible to significantly improve teaching processes. Despite the fact that some mathematicians were antagonistic to the use of programming languages, because according to them "the pure essence of mathematics is lost"; In the last 20 years, the mathematical society has proven the great help that the use of computational tools supposes for its work. In addition to this, the use of programming languages such as Python has proven to be beneficial when carrying out specific applications in areas of science such as Physics, Chemistry or Biology; since, the capabilities of Python allow to perfectly model mathematical behaviors in the aforementioned sciences.

Additionally, many researchers have carried out scientific studies to verify how programming affects the teaching of mathematics; where it has been concluded that the use of a programming language such as Python would result in an essentially positive stimulus in the basic stage of education since it would provide the following benefits:

1. Development of reasoning, facilitates the learning of mathematics and the ability to solve problems. It even helps with language-related subjects.
2. It favors the creative process since, imagining a project, investigating how to carry it out and structuring it so that it works, inherently involves the development of the imagination.
3. Increase self-confidence and self-esteem by seeing how what you work on is paying off.
4. Stay focused. Helps in the development of skills such as logic.
5. promotes teamwork. By seeking help from colleagues and forming support groups to solve the problems raised.

But how much math do I need to know to learn programming? This disturbing question arises in the consciousness of most people and despite popular conception, mathematics is not used much in programming. And you don't really need to be a math expert. For general programming, you should know the following about Math:

- Know the basic operations and in which cases each of them is used.
- Know the rule of signs in operations with integers.
- Know what a Cartesian coordinate system is.
- Know the Pythagorean theorem, since you will have to use it to find the distance between two points in a Cartesian coordinate system.
- How to get the percentage of a number
- Master the decimal, binary and hexadecimal numbering systems.

You will only need to know mathematics to develop specific programs that do deserve it, but it would be more focused on the program than on the fact of programming itself.
Now, to solve a problem in any programming language, you must know the following:

- What does the problem ask of me?
- What data do I need? Y
- Perform the Pseudocode

Python has the module mechanism where the MATH module is located, which contains a good number of hyperbolic, trigonometric and logarithmic functions for real numbers, rounding, truncation and constants, among others and the CMATH module allows you to work with complex numbers.
Python's arithmetic operators are:

Addition (+), Subtraction (-), Multiplication (*), Division (/), Integer division (//); Module or remainder (%) and Empowerment (**).

Once you have your work environment fully installed on your PC, you are ready to solve basic problems; otherwise, you should go to the official Python site to download its latest version: <https://www.python.org>

Here are some basic routines for young people who want to venture into PYTHON:

## Script N° 1

**Task:** Synthesize function

```python
def fruit_distribution(s, n):
    """
    In this task, you will be given a string that represents a number of apples and oranges
that are distributed in a basket of fruit this basket contains apples, oranges, and   mango fruits.
Given the string that represents the total number of the oranges and apples and an integer that represent the total
number of the fruits, in the basket return the number of the mango fruits in the basket.
    for example:
    fruit_distribution("5 apples and 6 oranges", 19) ->19 - 5 + 6 = 8
    fruit_distribution("0 apples and 1 oranges",3) -> 3 - 0 + 1 = 2
    fruit_distribution("2 apples and 3 oranges", 100) -> 100 - 2 + 3 = 95
    fruit_distribution("100 apples and 1 oranges",120) -> 120 - 100 + 1 = 19
    """
   
 apples_and_oranges = []
    number_mango_fruits = 0
    for j in s.split():
        try:
            # getting apples and oranges ...
            apples_and_oranges.append(int(j))
        except ValueError:
            pass
    sum_apples_and_orange = (sum(apples_and_oranges))
    number_mango_fruits -= (sum_apples_and_orange - n)
    print('The number of the mango fruits in the basket are ->:', number_mango_fruits)
    return number_mango_fruits
# Function call ...
fruit_distribution("5 apples and 6 oranges", 19)
fruit_distribution("0 apples and 1 oranges", 3)
fruit_distribution("2 apples and 3 oranges", 100)
fruit_distribution("100 apples and 1 oranges", 120)

=>The number of the mango fruits in the basket are ->: 8
=>The number of the mango fruits in the basket are ->: 2
=>The number of the mango fruits in the basket are ->: 95
=>The number of the mango fruits in the basket are ->: 19
```

## Script N°2

**Task:** Synthesize function

```python
def triangle_area(a, b, c):
    """    Given the lengths of the three sides of a triangle. Return the area of
    the triangle rounded to 2 decimal points if the three sides form a valid triangle.
    Otherwise return -1
    Three sides make a valid triangle when the sum of any two sides is greater
    than the third side.
    Example:
    triangle_area(3, 4, 5) == 6.00
    triangle_area(1, 2, 10) == -1
    """
    d = a + b
    sum_ = (a + b + c) / 2
    if d > c:
        # Calculate the area ...
        area = (sum_*(sum_-a)*(sum_-b)*(sum_-c)) ** 0.5
        print('The area of the triangle is ->', "{:.2f}".format(area))
        return area
   else:
        area = -1
        print('The area of the triangle is ->', area)
        return area
# Function call ...
triangle_area(3, 4, 5)
triangle_area(1, 2, 10)
=>The area of the triangle is -> 6.00
=>The area of the triangle is -> -1
```

## Script N°3

**Task:** Synthesize function

```python
def f(n):
    """ Implement the function f that takes n as a parameter, and returns a list of size n, such that the value of the
    element at index i is the factorial of i if i is even or the sum of numbers from 1 to i otherwise.
    i starts from - the factorial of i is the multiplication of the numbers from 1 to i (1 * 2 * ... * i).
    Example:
    f(5) == [1, 2, 6, 24, 15]
    """
    factorial = 1
    List = []
    for i in range(n + 1):
        if i == 0:
            pass
        else:
            factorial *= i
            List.append(factorial)
    print(List)
#  Function Call
f(5)
=> [1, 2, 6, 24, 120]
```

## About the author

Clay Lanzino is a passionate former surfer, father of three children, husband and a 33-year-old IT professional who loves programming. In his spare time, he loves being in nature, hugging the trees, walking barefoot to take in the energy of the earth and doing meditations in the open air. If time permits, he does some Yoga, in his exclusive meditation room.
