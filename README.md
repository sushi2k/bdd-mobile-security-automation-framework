# BDD security tests for Android and iOS application

ING provides a set of BDD security tests with Calabash,Cucumber and Ruby, following the OWASP Mobile Security Testing Guide and the OWASP Mobile Top 10 2016, that can be easily customized and implemented through the entire CI/CD pipeline. 

The tests use the power of [calabash.io](https://calabash.io) to automate the UI, [Cucumber](https://cucumber.io/) and Gherkin for its simple language and the Android tools to check for security issues.

### Prerequisites

* Docker
* Genymotion or real devices 

### Docker container 

The docker container can be used to spin up Calabash and the Android tools. Follow the README in the docker folder.

__At the moment the docker container can only be used to test Android applications. If you want to run iOS tests you need to install Calabash native on macOS__


## First Test

The repo contains a simple test that can be used as a sample to check that everything works. 


## OWASP MASVS and MSTG
The repo's structure is based on the [OWASP Mobile Application Security Verification Standard](https://github.com/OWASP/owasp-masvs) and the corresponding tests from the [OWASP Mobile Security Testing Guide](https://github.com/OWASP/owasp-mstg). For each test many features are defined with corresponding steps. 


### Work in progress

**iOS (only native on macOS)**:

* V2 - Data Storage and Privacy
	* Testing For Sensitive Data in Logs 	* Testing for Sensitive Data in the Clipboard 
	* Testing for Sensitive Data in the Keyboard Cache (To Be Completed)
	* Testing for Sensitive Data in Backups (To Be Completed)


**Android**:

* V2 - Data Storage and Privacy
    * Testing For Sensitive Data in Logs 
    * Testing for Sensitive Data in the Clipboard 
    * Testing for Sensitive Data in the Keyboard Cache 
    * Testing for Sensitive Data in Backups (To Be Completed)

* V6 - Platform Interaction 
	* Testing for XSS in WebView (Done)

