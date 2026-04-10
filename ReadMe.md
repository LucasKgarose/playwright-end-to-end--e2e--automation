# Playwright End to End E2E Automation using a real world To do App

## Goals

* Install Playwright
* Automate adding 3 todos, mark 1 as completed, and delete
* Generate Playwright HTML report and open it
* Add assertions and check failures in the report
* Take screenshots and videos on failure and attach them to the report
* Run with interactive UI
* Run in debug mode
* Run with trace enabled

---

## Commands

### Run tests

Run all Playwright tests in files matching "todo"
npx playwright test todo

Run only tests tagged with @sanity in "todo" files in headed mode
npx playwright test todo --headed --grep @sanity

Run all tests tagged with @sanity across the project in headed mode
npx playwright test --headed --grep @sanity

Run all tests using the Chromium project configuration
npx playwright test --project=chromium

---

### UI and debugging

Open Playwright Test UI to interactively run and debug tests
npx playwright test todo --ui

Run tests in debug mode
npx playwright test --grep @sanity --debug

---

### Reports and trace

Run tests in headed mode and generate an HTML report
npx playwright test --headed --reporter=html

Open the last generated HTML report
npx playwright show-report

Show the trace file
npx playwright show-trace trace.zip

---
