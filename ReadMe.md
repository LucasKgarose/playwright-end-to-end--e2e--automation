# Playwright End-to-End (E2E) Automation using a real-world To-do App.

## Goals
* install PLaywright
* Automate adding 3 todos, mark 1 as completed, delete,
* Generate Playwright *HTML report* and open it
* Add assertions and check failure in report
* Take screenshots and video on failure and attach to report
* Run with inteactive UI
* Run in debug mode
* Run with trace on# playwright-end-to-end--e2e--automation

# Commands
# Run all Playwright tests in files matching "todo"
npx playwright test todo

# Run only tests tagged with @sanity in "todo" files, with browser UI visible (headed mode)
npx playwright test todo --headed --grep @sanity

# Run all tests tagged with @sanity across the project, with browser UI visible (headed mode)
npx playwright test --headed --grep @sanity

# Run all tests using the Chromium project configuration
npx playwright test --project=chromium

# Open Playwright Test UI to interactively run and debug "todo" tests
npx playwright test todo --ui

# Run all tests in headed mode and generate an HTML report
npx playwright test --headed --reporter=html

# Open the last generated Playwright HTML report in the browser
npx playwright show-report

# show the trace
npx playwright show-trace trace.zip

# Run in debug mode
npx playwright test --grep @sanity --debug