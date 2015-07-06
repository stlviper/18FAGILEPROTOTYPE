### Demo Application 


Instruction to install and run application on other machine

Pre-Requisites is to install [NodeJS](https://nodejs.org/) (min version 0.10.18) and [NPM](https://docs.npmjs.com/getting-started/installing-node)

```
git clone https://github.com/vencoreinc/18FAGILEPROTOTYPE.git vencoredemo
cd vencoredemo/development/src
 // default port is 80
node app.js
// To run the application on a different port
PORT="8080" node app.js // to run on port 8080
```

### Docker Install

Additional details how to deploy the application using docker are in dist directory in [Github](https://github.com/vencoreinc/18FAGILEPROTOTYPE/tree/master/dist)

### Grunt tasks 

To run the following grunt tasks from the command line you need to install gurnt-cli globally

`
npm install -g grunt-cli
`

These are the main tasks that are exposed to Jenkins: </br>
* buildTask : <code> grunt buildTask</code> </br>
This task does the clean up, creates the necessary directories and starts the build ,then once the archive file is created it will be placed in the dist folder </br>
 
* unitTest : <code> grunt unitTest </code> </br>
the task will run the unit test , please note that  the unit test is implemented by using [Mocha Framework](http://mochajs.org/) </br>

* integrationTest: <code> grunt integrationTest </code> </br>
the task will run the integration test which is implemented by using [Protractor Framework](https://angular.github.io/protractor/#/) ,  and internally uses [Selenium](http://www.seleniumhq.org/) Server.
* Following URL has the instructions to setup [selenium server](https://github.com/angular/protractor/blob/master/docs/server-setup.md) 
* Setup headless browswer testing on linux [Github](https://github.com/vencoreinc/18FAGILEPROTOTYPE/tree/master/development/src/test)
 

For API documentation generation we used [apidocjs](http://apidocjs.com/)
Install apidoc globally and run the grunt task as shown below. 

<code>npm install apidoc -g</code>

<code>grunt apidoc</code>


