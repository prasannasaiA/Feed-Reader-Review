# Feed Reader Testing with jasmine

# Table of content

- [Download](#download)
- [Instructions](#instructions)
- [Project Overview](#project-overview)
- [Why this Project?](#why-this-project)
- [How to Run?](#how-to-run)
- [Tests in this project](#tests-in-this-projects)
- [Benefits](#benefits)
- [Development Strategy](#development-strategy)
- [Contributing](#contributing)

----------------

## Download

- The starter code for this project can be downloaded from:

    * The Feed Reader Review Project repository on GitHub : <https://github.com/udacity/frontend-nanodegree-feedreader>

- You can download or clone them from the repository.

----------------

## Instructions

- The Feed Reader Review Project is totally about testing the already created web-based application.

- The test suits should contain some specifications which makes sure that they satisfy with the given code without missing any test suites.

------------------

## Project Overview

- In this project we are given a web-based application that reads RSS feeds.

- The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/).

- The developer started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite.

- The remaining test suites are to be identified and complete them.

---------------

## Why this Project?

- Testing is an important part of the development process and many organizations practice a standard of development known as **test-driven development**.

- This is when developers write tests first, before they ever start developing their application.

- All the tests initially fail and then they start writing application code to make these tests pass.

- Whether we work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!

-------------------

## How to run?

- On downloading the project from repository, the project was initially provided with a test suite satisfied.

- We should write the remaining test suites and prove them they are satisfied, using `Jasmine`.

- For each test suite there should be some specs which specifies the specification satisfied.

----------------------

## Tests in this projects

The tests which are performed in this project are:

    1. A test to make sure that the `allFeeds` variable has been defined.

    2. A test to make sure that the `allFeeds` variable is not empty.

    3. A test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.

    4. A test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.

    5. A test that ensures the menu element is hidden by default.

    6. A test to analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.

    7. A test that ensures the menu changes visibility when the menu icon is clicked.

    8. The above test should have two expectations: does the menu display when clicked and does it hide when clicked again.

    9. A test that ensures when the `loadFeed` function is called and completes its work, there is at least a single .entry element within the .feed container.

    10. A test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes.

---------------------

## Benefits

- We will learn how to use `Jasmine` to write a number of tests against a pre-existing application.

- These will test the underlying business logic of the application as well as the **event handling and DOM** manipulation.

- Writing effective tests requires analyzing multiple aspects of an application including the HTML, CSS and JavaScript - an extremely important skill when changing teams or joining a new company.

- Good tests gives us the ability to quickly analyze whether new code breaks an existing feature within the codebase, without having to manually test all of the functionality.

----------------

# Development Strategy

For a refresher (or reference) before we begin writing code, it will be helpful to refer the content from [JavaScript Testing](https://www.udacity.com/course/javascript-testing--ud549).

1. Familiarize yourself with the starter code
    * Open up `index.html` and review the functionality of the application within your browser
    * What is all the code in `app.js` doing? Be sure to read all code comments
    * Check out `style.css`. How is styling applied to the application?
2. Explore the Jasmine spec file in `feedreader.js`
    * This is the file in which you'll be writing your tests
    * Make sure to read all code comments here as well
    * Review the [Jasmine documentation](http://jasmine.github.io) if needed
3. Edit the `allFeeds` variable in `app.js` to make the provided test fail
    * See how Jasmine visualizes this failure in your application
    * Return the `allFeeds` variable to a passing state after reviewing the failed test
4. Write a test that loops through each feed in the `allFeeds` object and ensures it has a URL defined _and_ that the URL is not empty
    * For example, how would you use a `for...of` loop in this test?
5. Write a test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty
    * Think about how you wrote the previous test. What are you testing for this time?
6. Write a new test suite named `"The menu"`
    * What are you `describe`-ing in this test suite?
7. Write a test that ensures the menu element is hidden by default
    * You'll have to analyze the HTML and the CSS to determine how the hiding/showing of the menu element is implemented
    * What code in `app.js` is directly involved with toggling the menu on and off?
8. Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: does the menu display itself when clicked, and does it hide when clicked again?
    * Think about how you wrote the previous test. What is different this time around?
    * Which clickable element are you checking for?
    * How do you "simulate" a mouse click that element without actually clicking it?
9. Write a test suite named `"Initial Entries"`
    * What are you `describe`-ing in this test suite?
10. Write a test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container
    * How does Jasmine's `beforeEach()`function work?
    * How does the `loadFeed()` function in `app.js` work? Is it synchronous or asynchronous?
11. Write a test suite named `"New Feed Selection"`
    * What are you `describe`-ing in this test suite?
12. Write a test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes
    * How is this test different from the previous test?

Additionally, note that:

 * No test should be dependent on the results of another
 * Callbacks should be used to ensure that feeds are loaded before they are tested
 * Error handling should be implemented for undefined variables and out-of-bound array access
 * When complete, all of your tests should pass

When you're all finished, write a `README` file detailing all steps required to successfully run the application. If you have added additional tests, provide documentation for what these future features are and what the tests are checking for.

-----------

# Contributing

This repository is the starter code for _all_ coders who are interested in testing using **Jasmine**.
