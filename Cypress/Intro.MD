# Documentation

## Intro to Cypress

Starter project to test a React application using cypress (npm/node.js)

**https://docs.cypress.io/examples/tutorials**



### Setup
1. Downloaded nvm (node + npm)
2. cloned repo from: https://github.com/cypress-io/cypress-tutorial-build-todo/tree/01_setup
3. npm install (the packages.json includes all dependencies for the project)
4. changed Cypress version to 8.3.0 in the packages.json file (more stability)
5. Either add "cypress" : "open" to the packages.json command section or simply "npx cypress open" in bash

### Tutorials
- [x] Project setup
- [x] Text inputs
- [x] Form submission and XHRs
- [x] Loading data with fixtures
- [ ] Todo item behaviour
- [ ] Toggling and debugging
- [ ] Filters and data-driven tests
- [ ] Full end-to-end tests Pt. 1
- [ ] Full end-to-end tests Pt. 2

## Writing tests

There should be a 'cypress' folder included in the project. Inside it, organise tests into categories, test suites, etc.

*e.g. Cypress/integration/input-form.spec.js* Will include the test suite for tests related to texting the input form and text-based inputs for the To do list.

## List of commands

|Command| Description|
|------|------|
|Commands specific to testcase design|
|describe('Name of test suite', () => {})| describe and context('Name') are used to name and organize suites of tests|
|it('Name of testcase', () => {})    |  Each testcase include in the test suite|
|it.only('Name of testcase', () => {})  | Specifies a testcase to be run on its own, without reusing state or impacting other testcases |
|cy.vist('URL')| opens a URL|
|cy.get('.class-name')| Selects a class or component as the UUT |
|*.type('inputText')| Inputs text in the selected component |
|\*.should('have.*whatever*', 'value')| The UUT shall have whatever property equal to the specified value|
||Creating Cypress commands (for reusability)| --- ||
|----|----|
|Cypress.Commands.add('name of command', => {})| Creates a new command to be used globally|
|cy.name-of-command| Calls the predefined command, can be used for global setup, improves code reusability|

