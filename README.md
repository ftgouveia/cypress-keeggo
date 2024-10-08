# Introduction

## Cypress + Cucumber

Cypress.io is an end-to-end automated testing framework using JavaScript. Cypress aims to perform e2e accessibility testing.

# Prerequisites

- Language: NodeJs > 16 and Npm > 8
- Installation of Cypress 12.16.0
- IDE: recommended Visual Code

## IMPORTANT
If you have not made the necessary settings to run Cypress on your machine (first run and such), follow the procedure described below.

After carrying out these installation processes, simply continue running the plugin.

## Installation

Navigate to the application's root folder, where the `package.json` file is located.

If it's a new project and doesn't yet have the `package.json` file, no problem, just make sure it's in the root folder where your application will be located.


```bash
cd <application root folder path>
```

Apply the plugin according to the command 'npm install'


## Operation
Dependencies such as devDependencies `cypress` will be added, `@badeball/cypress-cucumber-preprocessor` , `@bahmutov/cypress-esbuild-preprocessor` and `multiple-cucumber-html-reporter` and the solution installation process will begin.

The plugin will make the following changes:
- Creation of the `package.json` file if it does not exist.
- Addition of execution scripts.
- Creation of the `cypress` folder with configurations for e2e tests, in addition to e2e example tests already configured in `cypress/e2e/integration`
- Creation of the `cypress.config.js` file containing the tool settings.
- The `.gitignore` file will be changed or included by adding the `cypress/reports/*` and `cypress/results/*` folders.

All right, your plugin will be ready to use!

## Run

Run the command 'npx cypress open' or execute scripts from package.json to run in background.
