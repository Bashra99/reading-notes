# Reading 4: Classes, Objects, Recursion, and Pytest

## [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

- classes in python are conceptionally the same to JS
- all methods must include `self` as a parameter
- method use: obj_name.function_name()
- variable use: obj_name.variable_name
- the `__inti__` function must be used when the class is declared. This is similar to constructor in class
- variables can go inside methods

## [Thinking Recursively](https://realpython.com/python-thinking-recursively/)

- a recursive function is defined by calling itself
- the recursive function structure can often times mirror the recursive data structure definition
- keep scope in mind when using recursion, remember the action doesn't happen once
- each recursion adds a stack to the stack frame and then runs until the end to get the result
- there are multiple recursive data structures
- a list is a recursive data structure

## [Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

- to define a fixture decorate your function with `@pytest.fixture`
- fixtures are objects that contain data that all of the tests in the "test suite" may need
- the fixture will then look like a variable and function like a defined function
- `@pytest.fixture(scope='module')` will keep the scope of that fixture to the module it is defined in
- code coverage ensures that you have checked all the possible code executions
- to use coverage on pytest:
  - download `pytest-cov` using `PyPl`
  - to invoke: `pytest --cov=module`
  - convert to human readable: `coverage HTML`
    - this will create a dir called htmlcov, open the index.html from that dir in the browser to see the report

## Bookmarks

- [Pytest Fixtures](https://docs.pytest.org/en/latest/fixture.html)