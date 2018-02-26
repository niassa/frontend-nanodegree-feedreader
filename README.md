# Front-end Nanodegree Feeds Testing Project 

In this project, I was given a web-based application that reads RSS feeds. The original developer of the application clearly saw the value in testing, as they included [Jasmine](http://jasmine.github.io/) and started writing their first test suite. Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite.

## About This Testing Project

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

## Using this App
Load the index.html file. The list of CSS Tricks feeds should load in a stack as the default. To change feeds, select the Menu button to show the Menu, then select a different feed from the Menu's list.

To view the Jasmine testing information, scroll to the bottom of the page. Jasmine will list any successes or failures as defined in the `feedreader.js` file of test specs.

## What I Learned

In working on this project, I learned how to use Jasmine to write various tests against a pre-existing application. These tests include:
* Underlying business logic of the application
* Event handling
* DOM manipulation

## How I completed this project:

1. I reviewed the Feed Reader Testing [Project Rubric](https://review.udacity.com/#!/projects/3442558598/rubric) provided by Udacity.
2. Forked and downloaded the required project assets.
3. Reviewed the functionality of the application (`index.html`) in my browser.
4. Reviewed each of the necessary files for all pertinent information
   * `index.html`
   * `style.css`
   * `app.js`
   * `feedreader.js`
5. Manually edited the `allFeeds` variable in **app.js** to make the provided test fail to double-check the provided test case, and also verify how Jasmine handles the failure.
6. Manually return the `allFeeds` variable back to what it was and ensure Jasmine handles the passing.
7. Wrote a test to loop through each feed in the `allFeeds` object to verify it has a URL and the URL isn't empty.
8. Wrote a test that loops through each feed in the `allFeeds` object to verify it has a name defined and the name isn't empty.
9. Wrote a new test suite named `"The Menu"`.
10. Wrote a test to ensure the menu element is hidden by default. Used jQuery to verify the DOM information.
11. Wrote a test to verify the menu changes visibility when the menu items is clicked. This test has two expectations:
    * The **menu** displays when clicked
    * The **menu** hides when clicked again
12. Wrote a new test suite named `"Initial Entries"`.
13. Wrote a test to verify that when the `loadFeed` function is called (found in `app.js`) and completes, there is at least a single `.entry` element within the `.feed` container. Used jQuery to verify the DOM information.
14. Wrote a new test suite named `"New Feed Selection"`.
15. Wrote a new test to verify when a new feed is loaded by the `loadFeed` function, the content actually changes.
16. No tests are dependent on the results of another---they are all individual.
17. Callbacks are used to verify feeds are loaded before they are tested.
18. Verified that all tests pass green.
19. Wrote this `README` file detailing all steps.