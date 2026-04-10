# Playwright E2E learning notes

## This is a simple record of what I practiced and understood while learning Playwright using a to do app.

What I set up

* I installed Playwright and configured a few helpful options.
* I enabled trace on retry so I can debug failures.
* I set screenshots and videos to be saved only when a test fails.
* I used Chromium as the browser and added a small slow motion delay so I can actually see what is happening.

What I automated

* I wrote a test that interacts with a real to do app.

The test does the following

* Adds multiple tasks like Buy Grocery, Go for walk, Rest, and Play
* Marks some tasks as completed
* Switches between Completed, Active, and All views
* Clears completed tasks

## This helped me understand how to locate elements and simulate real user actions.

What I checked

* I added assertions to confirm the app behaves correctly

* I checked that certain tasks are visible
* I verified that expected items exist in the list
* I confirmed the final state after clearing completed items

### This showed me how important validation is in tests.

Reports

* I generated an HTML report after running tests

* npx playwright test --headed --reporter=html
* npx playwright show-report

### The report helped me see test results clearly and understand failures.

Debugging

* I learned a few ways to debug tests

UI mode
* npx playwright test todo --ui

Debug mode
* npx playwright test --grep @sanity --debug

Trace viewer
* npx playwright show-trace trace.zip

### These tools made it much easier to understand what went wrong step by step.

Running tests in different ways

* I tried different commands to run tests

Run specific file
* npx playwright test todo

Run only sanity tests
* npx playwright test --headed --grep @sanity

Run on Chromium
* npx playwright test --project=chromium

### This helped me see how flexible Playwright is.

What I learned

* I now understand how to write a basic end to end test
* I can interact with elements using different selectors
* I know how to add assertions and verify results
* I can debug failures using UI mode, debug mode, and traces
* I can generate and read test reports

Next steps

* Practice writing more tests with different scenarios
* Learn better locator strategies
* Try running tests on multiple browsers
* Understand test structure and reuse

### This is still early learning, but I now feel more comfortable working with Playwright.