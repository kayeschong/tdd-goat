# tdd-goat

Notes and code for working through tdd with python book.

https://www.obeythetestinggoat.com/

## Chapter 1

Install python, Django, Firefox, geckodriver and selenium

Setup virtual environment, git repository and django startproject superlists .

Write first functional test to check if django is installed and runnable.

### Useful TDD Concepts

Always start with a test

1. Write the test
2. Run it and check that it fails as expected.
3. Only then do we go ahead and build some of our app.
4. Repeat to yourself in a goat-like voice.

## Chapter 2

Write user story for MVP using comments.

Rewrite functional test to use unittest module and close cleanly.

## Useful TDD Concepts

User story

> A description of how the application will work from the point of view of the user. Used to structure a functional test.

Expected failure

> When a test fails in the way we expect it to.

## Chapter 3

Start Django app and create Django unit test runner with `python manage.py test`.

Resolving URLs with urls.py and simple regex.

Django view functions, request and response objects. 

Return basic HTML page.

### TDD approach for web app

1. We start by writing a *functional test*, describing the new funcionality from the user's point of view.
2. Once we have a functional test that fails, we start to think about how to write code that can get it to pass (or at least to get past its current failure). We now use one or more *unit tests* to define how we want our code to behave - the idea is that each line of production code we write should be tested by (at least) one of our unit tests.
3. Once we have a failing unit test, we write the smallest amount of *application code* we can, just enough to get the unit test to pass. We may iterate between steps 2 and 3 a few times, until we think the functional test will get a little further.
4. Now we can rerun our functional tests and see if they pass, or get a little further. That may prompt us to write some new unit tests, and some new code, and so on.

Functional tests should help you build an application with the right functionality, and guarantee you never accidentally break it. Unit test should help you to write code that's clean and bug free.

