### Demo Application 


Instruction to install and run application on other machine

Prerequisites is to install NodeJS (min version 0.10.18) on operation system. 

<code>
git clone https https://github.com/vencoreinc/18FAGILEPROTOTYPE.git vencoredemo
cd vencoredemo/development/src
node app.js // default port is 80
// To run the application on a different port
PORT="8080" node app.js // to run on port 8080
</code>

### Following Grunt tasks are available and can be run from the command line
  
These are the main tasks that are exposed to Jenkins: </br>
* buildTask : <code> grunt buildTask</code> </br>
This task does the clean up, creates the necessary directories and starts the build ,then once the archive file is created it will be placed in the dist folder </br>
 
* unitTest : <code> grunt unitTest </code> </br>
the task will run the unit test , please note that  the unit test is implemented by using [Mocha Framework](http://mochajs.org/) </br>

* integrationTest: <code> grunt integrationTest </code> </br>
the task will run the integration test which is implemented by using [Protractor Framework](https://angular.github.io/protractor/#/) ,  a Framework that internally uses [Selenium](http://www.seleniumhq.org/) Server</br>
 

For API documentation generation we used [apidocjs](http://apidocjs.com/)
Install apidoc globally and run the grunt task as shown below. 

<code>npm install apidoc -g</code>

<code>grunt apidoc</code>


