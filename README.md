# vfdademo
Demo app for testing cool new technologies using NodeJS, Express, Angurlar and other ...

pre:
nodejs
npm
bower

npm init
npm install --save express
npm install --save-dev  grunt
npm install --save request


Grunt Scripts :</br>
Grunt Scripts support the continuous integration, multiple tasks were designed and made available to Jenkins.
The implementation of tasks relies on a number of dependencies that can be loaded and installed using the following commands :
 <code>npm install grunt-contrib-copy --save-dev</code>        // install contrib-copy </br>
 <code>npm install grunt-contrib-clean --save-dev </code>      // install contrib-clean </br>
 <code>npm install grunt-contrib-compress --save-dev </code>   // install contrib-compress </br>
 <code>npm install grunt-mocha-test --save-dev </code>          //install contrib-test  </br> 
 <code>npm install grunt-zip --save-dev </code>                // //install contrib-zip  </br>
 <code>npm install grunt-properties-reader --save-dev </code>    // install properties-reader </br>
 <code>npm install grunt-protractor-runner --save-dev </code>    // install protractor-runner </br>
 
There are three main tasks that are exposed to Jenkins: </br>
1-	buildTask </br>
This task makes the necessary directory clean up  and start the build , the archive file will be created and placed in the dist folder </br>
<code> grunt buildTask</code> </br>

2-	unitTest </br>
the task will run the unit test , please note that  the unit test is implemented by using Mocha Framework </br>
<code> grunt unitTest </code> </br>


3-	intergationTest </br>
the task will run the integration test which is implemented by using Protractor Framework ,  a Framework that internally uses Selenium Server  v
<code> grunt intergationTest </code> </br>

For API documentation generation we us http://apidocjs.com/.

<code>npm install apidoc -g</code>

<code>grunt apidoc</code>

Need Devops working
