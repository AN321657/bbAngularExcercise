# bbAngularExcercise

Please download the zip folder and unzip it.

# weather-report

This project is generated with yo angular generator for desired architechture. ( As per current trend we can opt angular cli )

Additional library is used with npm protractor for E2E testing. 
 

## Build & development

Run `grunt` for building and `grunt serve` for preview.

## Testing

Running `grunt test` will run the unit tests with karma.

Additional e2e test is will run with protractor.

I have configured test covrage for karma Unit test. 
1. Currently format is text which will reflect in terminal
2. To get html go to karma_congif.json and replace the below snippet

coverageReporter: {
      type: 'html',
      dir: 'coverage'
    },

Please make sure you should having jdk installed in your system, before starting the selenium server.

1. Start the Selenium server:
./node_modules/.bin/webdriver-manager start

2. Open a new terminal and run Protractor:
./node_modules/.bin/protractor protractor.conf.js

Steps to be followed:

npm install 

grunt serve

grunt test ( for all test together)

grunt runOnlyKarmaTest

grunt runOnlyProtractorTest 

grunt build

As per the time constraint, I have prototype of the architecture. 
1. Moduler code for controller, services, views, and constants, while using different environment like DEV, QE, and PROD
2. Build version will be available in "dist" folder and the command needs to be is "grunt build", which covers all the operation like minification, uglyfication, concatination.
3. All environment varibles will be available in appConstant.js file. (In this project, I have kept the App Key and API URL)
4. Angular $q Promises are implemented while calling the API. As per standards extra handling like interceptors and web sockets can be implemented for the secure and dynamic live data streaming, for which I having the hands on experience.
5. For the current implementation of the testing framework which I have shared has the sample test coverage, which can be further enhanced by adding the more test scenarios. Adding the test scenarios will also improve the code coverage report.

