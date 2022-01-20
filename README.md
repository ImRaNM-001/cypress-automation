set up a new project in your GitHub account and clone it locally.



Open a terminal and navigate to the root directory of the project.

Run npm init -y to create your package.json file.



If you wish, you can set up shortcuts for Cypress commands by installing the Cypress Snippets extension in VSCode. You can also set up linting with the Cypress plugin for ESLint:

https://github.com/cypress-io/eslint-plugin-cypress

Cypress uses Mocha for its test framework and for its assertions, so it may well be worth installing the ES6 Mocha Snippets extension and the Mocha plugin for ESLint:

https://www.npmjs.com/package/eslint-plugin-mocha

For now, we’ll skip that and get started installing our software. You only need two dependencies for Cypress, one for the Cypress application and one for mochawesome which will be our reporting module.



In your new project, open up the Terminal in VSCode.

Type the following command to install Cypress and the mochawesome reporter.

Terminal
 npm install cypress mochawesome mocha@5.2.0 --save-dev
In your package.json file, change the test script to the following:

package.json
"test": "cypress open"


That’s everything. Let’s open the Cypress runner and start creating a specification.


The folder structure now looks like this:

 ![image](https://user-images.githubusercontent.com/59203975/150313010-c58decab-fd50-4fe1-ac83-7400c3e3e615.png)
