# Project Overview

In this project we are having a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite. That's where you come in.


## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

## What we did to test the applicaton without the testing code?

The application contest is wriiten in app.js file which we tested in feedreader.js context using jasmine
Used Jasmine to write a number of tests against a pre-existing application. These will test the underlying business logic of the application as well as the event handling and DOM manipulation.

#Steps  are with tests,suits in feed reader.js testing the application in app.js

1 A test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.
2 A test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.
3 A new test suite named `"The menu"`is there
4 In it test "The MEnu" menu element is hidden by default. we analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
5 Atest that ensures the menu changes visibility when the menu icon is clicked. This test has two expectations: does the menu display when clicked and does it hide when clicked again.
6 A test suite named `"Initial Entries"`.
7 In it test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container.
8 A test suite named `"New Feed Selection"`.
9 A test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes.
10  No test is dependent on the results of another.
11 Callbacks are used to ensure that feeds are loaded before they are tested.
