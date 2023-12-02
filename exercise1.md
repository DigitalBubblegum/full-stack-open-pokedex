# Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked? You can search for the answers by google.

For linting in python we have the following two options available pylint and mypy.

Pylint analyses your code without actually running it. It checks for errors, enforces a coding standard, looks for code smells, and can make suggestions about how the code could be refactored.

Mypy is an optional static type checker for Python that aims to combine the benefits of dynamic (or "duck") typing and static typing. Mypy combines the expressive power and convenience of Python with a powerful type system and compile-time type checking. Mypy type checks standard Python programs; run them using any Python VM with basically no runtime overhead. 

For testing therer are manny test runners available for python. some of them are: unittest, nose2, pytest.

unittest is built into python, and requires that you put the tests into classes as methods and that you use methods in the unittest.TestCase class.

nose2 is compatible with any tests written using the unittest framework and can be used as a drop-in replacement for the unittest test runner this is useful because as you write hundreds or even thousands of tests for your application, it becomes increasingly hard to understand and use the output from unittest.

pytest supports execution of unittest test cases although the real advantage of pytest comes by writing pytest test cases. it has many features kuje support for the built in assert statement, filtering test cases and ability to rerun from the last failing test.

Flask can be used for developing web applications using python. The advantages of the flask framework are that it is lightweight, it has built in support for unit testing, it dipatches requests with REST.
Flask is quite versatile and it is used in API development, web apps, microservices, webhooks, dashboards etc.

# What alternatives are there to set up the CI besides Jenkins and GitHub Actions? Again, you can ask google!

Circleci, Travis, Semaphore, GitlabCI are some alternatives to Jenkins and Github Actions.

# Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?

You can go very far with self-hosted for personal or small projects but we have to be take on the hassle of managing our self-hosted machine. this solution does not scale very easily.

Meanwhile the advantages of the cloud-based environment come at a premium. Using this as an enterprise solution makes more sense.

ultimately the decision rests on the factors of what your requirements are. self hosted is a low or no cost solution. which is perfect for small scale, and the cloud-based enivironment offers a managed platform which is perfect for a large scale solution, with zero or low downtime. 