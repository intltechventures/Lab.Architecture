
# Testing Resources

## Background Reading
- [The Way of Testivus: Less Unit Testing Dogma, More Unit Testing Karma](http://www.agitar.com/downloads/TheWayOfTestivus.pdf)


## Testing: Associations/Organizations
- https://www.associationforsoftwaretesting.org/


## Testing: Useful Groups/Meetups
- https://www.meetup.com/Software-Testers-of-Seattle/


## Testing Tutorial Resources 
- http://toolsqa.com/


## Testing Related Blogs, New Resources 
- https://www.deagiletesters.nl/en/blog/



## Ideas for Test Types/Categories: (TO-DO, organize and order these better...)
- Unit  
  + Boundary Value 
  + Equivalance Class 
  + Decision Table 
  + Path
  + Data Flow 
- Configuration 
- Installation
- Deployment
- Compatibility 
- Black Box
- Grey Box
- White Box 
- UI
- String
- Integration
  * Class
  * Subsystem
  * System 
- Interface
- System 
  * Data
  * Actions
  * Devices
  * Events
  * Threads
- All Pairs 
- Smoke
  * aka build verification test
- Sanity 
- Acceptance 
- Regression
- Compatibility
  * OS
  * Browser
- Usability 
  * Localization / Internationalization 
  * Compliance
    * ADA / Accessiblity 
- Exploratory 
- Stress
- Performance
- Load
- Stability 
- Volume
- Stability/Long Running 
- Security
  * Penetration
  * Vulnerability 


## Cloud Based Testing Platforms
- https://www.perfecto.io/
  * "3,000+ Devices available 24/7 in the Cloud"
  * "Test Web, Mobile & IoT devices using a single script"
  * https://www.perfecto.io/platform/test-automation/

- https://www.blazemeter.com/
  * "Test your API | Website | App leveraging open source tools JMeter, Gatling, Selenium & Taurus"
  * https://www.blazemeter.com/pricing
    * "50 concurrent users, free"

- https://saucelabs.com/
  * "Sauce Labs ensures your favorite mobile apps and websites work flawlessly on every browser, operating system, and device."
  * https://saucelabs.com/pricing
  * Frameworks Supported:
    * https://saucelabs.com/products/open-source-frameworks/selenium
    * https://saucelabs.com/products/open-source-frameworks/appium
    * https://saucelabs.com/products/open-source-frameworks/espresso
    * https://saucelabs.com/products/open-source-frameworks/xcuitest 


## Testing Tooling: General 
- http://robotframework.org/ 
  * https://github.com/robotframework/robotframework
  * https://twitter.com/robotframework


- Cucumber
  * https://en.wikipedia.org/wiki/Cucumber_(software)
  * https://cucumber.io/
    * "open source tool tests business-readable specifications against your code on any modern development stack."
  * https://docs.cucumber.io/
  * https://docs.cucumber.io/guides/10-minute-tutorial/
  * https://docs.cucumber.io/guides/
  * https://docs.cucumber.io/gherkin/
  * https://docs.cucumber.io/cucumber/
  * https://docs.cucumber.io/tools/related-tools/
  * cukes-rest: Cucumber DSL for testing RESTful Web Services 
    * https://github.com/ctco/cukes
      * "cukes-rest takes simplicity of Cucumber and provides bindings for HTTP specification. As a sugar on top, cukes-rest adds steps for storing and using request/response content from a file system, variable support in .features, context inflation in all steps and a custom plug-in system to allow users to add additional project specific content."
  * https://support.smartbear.com/articles/testcomplete/bdd-cucumber-and-testcomplete/


- http://watir.com/
  - Language: Ruby


- https://www.testcontainers.org/
  + Testcontainers is a Java library that supports JUnit tests, providing lightweight, throwaway instances of common databases, Selenium web browsers, or anything else that can run in a Docker container.
  + https://github.com/testcontainers/testcontainers-java/
    * License: MIT


## User Interface Scripting/Testing Resoruces

- Playwright
  + https://playwright.dev/
    * Playwright is a Node.js library to automate Chromium, Firefox and WebKit with a single API. 
    * Playwright is built to enable cross-browser web automation that is ever-green, capable, reliable and fast.
  * https://github.com/microsoft/playwright
  + https://twitter.com/playwrightweb


- Puppeteer
  + https://pptr.dev/
    * "Puppeteer is a Node library which provides a high-level API to control
    Chrome or Chromium over the DevTools Protocol. Puppeteer runs headless by
    default, but can be configured to run full (non-headless) Chrome or
    Chromium."
  + https://github.com/puppeteer/puppeteer
  +  https://try-puppeteer.appspot.com/



## Testing Tooling, Language Specific: Java
- Junit
  * https://junit.org/junit5/
  * https://en.wikipedia.org/wiki/JUnit

- Mockito
  * https://site.mockito.org/
  * https://en.wikipedia.org/wiki/Mockito
    * "Mockito is an open source testing framework for Java released under the MIT License. The framework allows the creation of test double objects in automated unit tests for the purpose of test-driven development or behavior-driven development"

- Spock Framework 
  * http://spockframework.org/
  * https://en.wikipedia.org/wiki/Spock_(testing_framework)
    * "Spock is a Java testing framework capable of handling the full life cycle of a computer program. It was initially created in 2008 by Peter Niederwieser, a software engineer with GradleWare. A second Spock committer is Luke Daley who is also the creator of the popular Geb functional testing framework."


## Testing Tooling: API focused
- Dredd - HTTP API Testing Framework
  * https://dredd.org/en/latest/
    * Languages supported:
      * Go
      * Node.js (JavaScript)
      * Perl
      * PHP
      * Python
      * Ruby
      * Rust
  * "Language-agnostic HTTP API Testing Tool"
  * https://github.com/apiaryio/dredd



## Testing Tooling: Mobile Apps
- Appium
  * http://appium.io/
    * "Appium is an open source test automation framework for use with native, hybrid and mobile web apps. It drives iOS, Android, and Windows apps using the WebDriver protocol."
- Espresso (Android)
  * https://developer.android.com/training/testing/espresso/
    * https://developer.android.com/studio/test/espresso-test-recorder
- XCUITest (iOS)
  * ...to be added...


## Testing Tooling, Language Specific: JavaScript
- ...to be added...


## Testing Tooling, Language Specific: .NET 
- NUnit
  * https://nunit.org/
    * "NUnit is a unit-testing framework for all .Net languages. Initially ported from JUnit, the current production release, version 3, has been completely rewritten with many new features and support for a wide range of .NET platforms."


## Testing Tooling, Language Specific: Python
- pytest
  * https://docs.pytest.org/en/latest/
  * https://github.com/pytest-dev/pytest


## Testing Tooling: Load/Performance
- http://www.opensourcetesting.org/category/performance/
  * several interesting articles...most recent posting appears to have been Dec 26, 2017, as of Nov 11, 2018...

- https://artillery.io/
  * https://github.com/Nordstrom/serverless-artillery

- JMeter
  + https://jmeter.apache.org/
    + "Apache JMeter may be used to test performance both on static and dynamic resources, Web dynamic applications."
    + "It can be used to simulate a heavy load on a server, group of servers, network or object to test its strength or to analyze overall performance under different load types."
    + Ability to load and performance test many different applications/server/protocol types:
      * Web - HTTP, HTTPS (Java, NodeJS, PHP, ASP.NET, …)
      * SOAP / REST Webservices
      * FTP
      * Database via JDBC
      * LDAP
      * Message-oriented middleware (MOM) via JMS
      * Mail - SMTP(S), POP3(S) and IMAP(S)
      * Native commands or shell scripts
      * TCP
      * Java Objects
    * Full featured Test IDE that allows fast Test Plan recording (from Browsers or native applications), building and debugging.

- cucumber-perf (Cucumber Performance)
  * https://github.com/mpinardi/cucumber-performance

- Cucumber
  * http://blog.mattwynne.net/2012/03/13/using-cucumber-for-load-testing/
  * https://stackoverflow.com/questions/26585142/load-testing-with-cucumber-and-java
  * [Cucumber: Using cucumber as the basis for a load testing application., Google Groups, Cukes, 2010-08-26](https://groups.google.com/forum/#!topic/cukes/4ZGkf3a234Y) 

- FunkLoad (no longer maintained...?)
  * https://github.com/nuxeo/FunkLoad

- Selenium
  * http://toolsqa.com/performance-testing-tools/performance-testing-selenium/

- Tsung
  * https://github.com/processone/tsung
  * http://tsung.erlang-projects.org/
  * "Tsung is an open-source multi-protocol distributed load testing tool"
  * "It can be used to stress HTTP, WebDAV, SOAP, PostgreSQL, MySQL, LDAP, MQTT and Jabber/XMPP servers. Tsung is a free software released under the GPLv2 license."
  * "The purpose of Tsung is to simulate users in order to test the scalability and performance of IP based client/server applications. You can use it to do load and stress testing of your servers. Many protocols have been implemented and tested, and it can be easily extended."
  * "It can be distributed on several client machines and is able to simulate hundreds of thousands of virtual users concurrently (or even millions if you have enough hardware …)."
  * "Tsung is developed in Erlang, an open-source language made by Ericsson for building robust fault-tolerant distributed applications."
  * "Several IP addresses can be used on a single machine using the underlying OS IP Aliasing"
  * "XML configuration system; several sessions can be used to simulate different type of users. Dynamic sessions can be easily described in XML (this can be used to retrieve at runtime an ID from the server output and use it later in the session)."
  * "In order to generate a realistic traffic, user think-times and the arrival rate can be randomize using a probability distribution"

- Nodeload (no longer being actively developed...)
  * https://github.com/benschmaus/nodeload
    * "HTTP load/traffic generator and benchmark tool built on Node.js "

- WebLoad
  * https://www.radview.com/
  * https://www.radview.com/about-webload/features/test-creation/
  * https://www.radview.com/webload-licensing/


## Testing Strategies/Concepts:
- Conext-Driven Testing
  * http://context-driven-testing.com/
- Test-Driven Development (TDD)
  * https://en.wikipedia.org/wiki/Test-driven_development
  * https://martinfowler.com/bliki/TestDrivenDevelopment.html
  * http://agiledata.org/essays/tdd.html
  * http://www.drdobbs.com/architecture-and-design/test-driven-design/240168102
  * https://medium.com/@DakshHub/a-hitchhiker-guide-to-test-driven-development-tdd-e1ef11dbc832
  * https://news.codecademy.com/test-driven-development/
- Behavior-Driven Development (BDD)
  * https://en.wikipedia.org/wiki/Behavior-driven_development
  * Dan North:
    * https://dannorth.net/introducing-bdd/
    * https://www.infoq.com/news/2015/04/dan-north-bdd-examples
    * https://dannorth.net/2012/05/31/bdd-is-like-tdd-if/
    * https://www.infoq.com/interviews/dan-north-bdd
    * https://dannorth.net/category/bdd/
    * [Interview with Dan North on Behavior-Driven Development, OOPSLA 2007](https://www.youtube.com/watch?v=qWsnmx45734)
  * https://www.agilealliance.org/glossary/bdd/
  * https://medium.com/@TechMagic/get-started-with-behavior-driven-development-ecdca40e827b



## Testing: TDD
- Test Driven Development: By Example 1st Edition (2002) 
  * https://www.amazon.com/Test-Driven-Development-Kent-Beck/dp/0321146530/



## Testing: Misc. Idea Resources
- http://commonsensetesting.org/
  * "The Seven Basic Principles of the Context-Driven School"
    * "The value of any practice depends on its context."
    * "There are good practices in context, but there are no best practices."
    * "People, working together, are the most important part of any project’s context."
    * "Projects unfold over time in ways that are often not predictable."
    * "The product is a solution. If the problem isn’t solved, the product doesn’t work."
    * "Good software testing is a challenging intellectual process."
    * "Only through judgment and skill, exercised cooperatively throughout the entire project, are we able to do the right things at the right times to effectively test our products."




NOTE: Those books I have personally read, and recommend - will be denoted with a "RECOOMEND" prefix to the title

## Suggested Books: General Testing Topics
- A Practical Guide to Testing in DevOps
  * https://leanpub.com/testingindevops
- Beautiful Testing: Leading Professionals Reveal How They Improve Software (Theory in Practice) 1st Edition (2009)
  * https://www.amazon.com/Beautiful-Testing-Professionals-Software-Practice/dp/0596159811
- Perfect Software: And Other Illusions about Testing
  * https://www.amazon.com/Perfect-Software-Other-Illusions-Testing/dp/0932633692
- Developer Testing: Building Quality into Software, 1st Edition (2016) 
  * https://www.amazon.com/Developer-Testing-Building-Addison-Wesley-Signature/dp/0134291069/
- How Google Tests Software 1st Edition (2012) 
  * https://www.amazon.com/Google-Tests-Software-James-Whittaker/dp/0321803027/
- Agile Testing: A Practical Guide for Testers and Agile Teams (2009) 
  * https://www.amazon.com/Agile-Testing-Practical-Guide-Testers/dp/0321534468
- More Agile Testing: Learning Journeys for the Whole Team (2014) 
  * https://www.amazon.com/More-Agile-Testing-Addison-Wesley-Signature/dp/0321967054/
- ```Lessons Learned in Software Testing: A Context-Driven Approach```
  * https://www.amazon.com/Lessons-Learned-Software-Testing-Context-Driven/dp/0471081124/
- ```Complete Guide to Test Automation: Techniques, Practices, and Patterns for Building and Maintaining Effective Software Projects (2018)```
  * https://www.amazon.com/Complete-Guide-Test-Automation-Maintaining/dp/1484238311/
- The Way of the Web Tester: A Beginner's Guide to Automating Tests (2016) 
  * https://www.amazon.com/Way-Web-Tester-Beginners-Automating/dp/1680501836/ 
- ```Friendly Introduction to Software Testing (2016)```
  * https://www.amazon.com/Friendly-Introduction-Software-Testing/dp/1523477377/
- ```Software Testing: A Craftsman’s Approach, Fourth Edition```
  * https://www.amazon.com/Software-Testing-Craftsmans-Approach-Fourth/dp/1466560681/
- Experiences of Test Automation: Case Studies of Software Test Automation 1st Edition (2012) 
  * https://www.amazon.com/Experiences-Test-Automation-Studies-Software/dp/0321754069/ 
- Testing in Scrum: A Guide for Software Quality Assurance in the Agile World (Rocky Nook Computing) 1st Edition
  * https://www.amazon.com/Testing-Scrum-Software-Assurance-Computing/dp/1937538397/



## Suggested Books: Testing, Technology Specific Topics
- Angular
  * Angular Test-Driven Development - Second Edition (2017) 
    * https://www.amazon.com/dp/1786465477/

- Appium
  * Appium Essentials (2015) 
    * https://www.amazon.com/Appium-Essentials-Manoj-Hans/dp/1784392480
  * Appium Recipes 1st ed. Edition (2016) 
    * https://www.amazon.com/Appium-Recipes-Shankar-Garg/dp/1484224175/
  * Mobile Test Automation with Appium: Mobile application testing made easy (2017) 
    * https://www.amazon.com/Mobile-Test-Automation-Appium-application/dp/1787280160/

- Selenium
  * ```Mastering Selenium WebDriver 3.0: Boost the performance and reliability of your automated checks by mastering Selenium WebDriver, 2nd Edition```
    * https://www.amazon.com/Mastering-Selenium-WebDriver-3-0-performance/dp/1788299671
  * Selenium WebDriver 3 Practical Guide: End-to-end automation testing for web and mobile browsers with Selenium WebDriver, 2nd Edition
    * https://www.amazon.com/dp/1788999762/ 
  * ```Selenium Framework Design in Data-Driven Testing: Build data-driven test frameworks using Selenium WebDriver, AppiumDriver, Java, and TestNG (2018)```
    * https://www.amazon.com/Selenium-Framework-Design-Data-Driven-Testing/dp/1788473574/
      * Selenium Grid Architecture 
      * Selenium Page Object Design Patterns 
      * Users will learn how to design and build a Selenium Grid from scratch to allow the framework to scale and support different browsers, mobile devices, versions, and platforms, and how they can leverage third party grids in the Cloud like SauceLabs.
      * Use third party tools and services like ExtentReports for results processing, reporting, and SauceLabs for cloud-based test services
  * Selenium Testing Tools Cookbook - Second Edition
    * https://www.amazon.com/Selenium-Testing-Tools-Cookbook-Second/dp/1784392510/
  * Test Automation using Selenium WebDriver with Java: Step by Step Guide
    * https://www.amazon.com/Test-Automation-using-Selenium-WebDriver/dp/0992293510/
  * Selenium Design Patterns and Best Practices
    * https://www.amazon.com/Selenium-Design-Patterns-Best-Practices/dp/1783982705/
  * Selenium WebDriver Practical Guide
    * https://www.amazon.com/Selenium-WebDriver-Practical-Guide-Avasarala/dp/1782168850/
  * Learning Selenium Testing Tools - Third Edition 3rd Revised ed. Edition (2015)
    * https://www.amazon.com/Learning-Selenium-Testing-Tools-Third/dp/1784396494/
  * Learning Selenium Testing Tools with Python (2014) 
    * https://www.amazon.com/Learning-Selenium-Testing-Tools-Python/dp/1783983507/
  * Zhimin Zhan
    * Practical Web Test Automation: Automated test web applications wisely with Selenium WebDriver (2014) 
      * https://www.amazon.com/Practical-Web-Test-Automation-applications/dp/1505882893/
    * Selenium WebDriver Recipes in C#: Second Edition (2015) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-C-Second/dp/1484217411/
    * Selenium WebDriver Recipes in Ruby: The problem solving guide to Selenium WebDriver in Ruby (Test Automation Recipes Series) (Volume 2) (2015) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-Ruby-Automation/dp/1505885329/
    * Selenium WebDriver Recipes in Java: The problem solving guide to Selenium WebDriver in Java (Web Test Automation Recipes Series) (Volume 3) (2015) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-Java-Automation/dp/1505895936/
    * Selenium WebDriver Recipes in C#: The problem solving guide to Selenium WebDriver in C# (Web Test Automation Recipes Series) (Volume 4) (2015) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-problem-Automation/dp/1505895863/
    * Selenium WebDriver Recipes in Python: The problem solving guide to Selenium WebDriver in Python (Test Recipes Series Book 5) (2018) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-Python-problem-ebook/dp/B07K6RJLRP
    * Selenium WebDriver Recipes in Node.js: The problem solving guide to Selenium WebDriver in JavaScript (Test Recipes Series) (Volume 6) (2016) 
      * https://www.amazon.com/Selenium-WebDriver-Recipes-Node-js-JavaScript/dp/1537328255/

- C#
  * The Art of Unit Testing: with examples in C# Second Edition (2013)
    * https://www.amazon.com/Art-Unit-Testing-examples/dp/1617290890/

- Cucumber
  * The Cucumber Book: Behaviour-Driven Development for Testers and Developers 2nd Edition (2017) 
    * https://www.amazon.com/dp/1680502387/
  * The Cucumber for Java Book: Behaviour-Driven Development for Testers and Developers
    * https://www.amazon.com/Cucumber-Java-Book-Behaviour-Driven-Development/dp/1941222293/
  * Cucumber Recipes: Automate Anything with BDD Tools and Techniques (2013) 
    * https://www.amazon.com/Cucumber-Recipes-Techniques-Pragmatic-Programmers/dp/1937785017/
  * Cucumber Cookbook (2015)
    * https://www.amazon.com/dp/1785286005/

- Gherkin Language
  * ...

- JMeter
  * Performance Testing with jMeter 3 - Third Edition (2017) 
    * https://www.amazon.com/Performance-Testing-jMeter-3-Third/dp/1787285774
  * Pro Apache JMeter: Web Application Performance Testing (2017) 
    * https://www.amazon.com/Pro-Apache-JMeter-Application-Performance/dp/1484229606/
  * Performance Testing with Jmeter - Second Edition (2015) 
    * https://www.amazon.com/Performance-Testing-Jmeter-Bayo-Erinle/dp/1784394815/
  * JMeter Cookbook (2014) 
    * https://www.amazon.com/JMeter-Cookbook-Bayo-Erinle/dp/1783988282/

- JUnit
  * Pragmatic Unit Testing in Java 8 with JUnit 1st Edition (2015) 
    * https://www.amazon.com/Testing-Junit-Frank-Appel/dp/1782166602/
  * Testing with Junit (2015) 
    * https://www.amazon.com/Testing-Junit-Frank-Appel/dp/1782166602/
  * Mastering Unit Testing Using Mockito and JUnit (2014) 
    * https://www.amazon.com/dp/1783982500/

- Mockito
  * Mockito for Spring (2015) 
    * https://www.amazon.com/dp/1783983787
   
- TestNG 
  * ...
   
- Watir
  * http://watir.com/
  * Watir Recipes: The problem solving guide to Watir (Web Test Automation Recipes Series) (Volume 1) (2014) 
    * https://www.amazon.com/Watir-Recipes-problem-solving-Automation/dp/1505883954/

- Python
  * Test-Driven Development with Python: Obey the Testing Goat: Using Django, Selenium, and JavaScript 2nd Edition (2017)
    * https://www.amazon.com/Test-Driven-Development-Python-Selenium-JavaScript/dp/1491958707
  * Python Testing with pytest: Simple, Rapid, Effective, and Scalable 1st Edition (2017) 
  * https://www.amazon.com/dp/1680502409/
- API Testing
  * Automating and Testing a REST API: A Case Study in API testing using: Java, REST Assured, Postman, Tracks, cURL and HTTP Proxies (2017) 
    * https://www.amazon.com/Automating-Testing-REST-API-testing/dp/0956733298




## Suggested Books: Performance Testing
- The Art of Application Performance Testing: From Strategy to Tools 2nd Edition (2014) 
  * https://www.amazon.com/Art-Application-Performance-Testing-Strategy/dp/1491900547


## Suggested Books: Test Certifications
- ISTQB
  * Sample Exam Questions- ISTQB Foundation Level-Agile Tester Extension Exam 1st Edition (2016) 
    * https://www.amazon.com/Sample-Questions-Foundation-Level-Agile-Extension/dp/1533567425/
  * Foundations of Software Testing ISTQB Certification (2015) 
    * https://www.amazon.com/Foundations-Software-Testing-ISTQB-Certification/dp/8131526364
  * Software Testing 3rd Edition (2015) 
    * https://www.amazon.com/Software-Hambling-Angelina-Thompson-Williams/dp/1780172990/
  * Software Testing Foundations, 4th Edition: A Study Guide for the Certified Tester Exam (2014)
    * https://www.amazon.com/Software-Testing-Foundations-4th-Certified/dp/1937538427/
  * Rex Black, et al
    * Advanced Software Testing - Vol. 1, 2nd Edition: Guide to the ISTQB Advanced Certification as an Advanced Test Analyst 2nd Edition (2015)
      * https://www.amazon.com/Advanced-Software-Testing-Certification-Analyst/dp/1937538680/
    * Advanced Software Testing - Vol. 2, 2nd Edition: Guide to the ISTQB Advanced Certification as an Advanced Test Manager Second Edition (2014) 
      * https://www.amazon.com/Advanced-Software-Testing-Certification-Manager/dp/1937538508/
    * Advanced Software Testing - Vol. 3, 2nd Edition: Guide to the ISTQB Advanced Certification as an Advanced Technical Test Analyst 2nd Edition (2015) 
      * https://www.amazon.com/Advanced-Software-Testing-Certification-Technical/dp/1937538648/
  * The Expert Test Manager: Guide to the ISTQB Expert Level Certification 1st Edition (2017) 
    * https://www.amazon.com/Expert-Test-Manager-Guide-Certification/dp/1933952946/



## Interesting Articles:

### 2021 


### 2020 


### 2019 


### 2018
- https://www.infoq.com/articles/james-bach-testing-career


### 2017  
- https://www.testingexcellence.com/selenium-and-cucumber-ui-automation-challenges/
  * "When we get to System Integration Testing or UI Testing, it is best to use Selenium without the underlying Cucumber framework as trying to write Cucumber feature files for user journeys, can get very cumbersome and would not serve the purpose the tool is built for."

- https://forums.meteor.com/t/acceptance-and-load-testing/34164/8


### 2016
- [BDD Tutorial - How to Use Cucumber and Watir Webdriver for Automated Testing, 2016-01-27](https://www.youtube.com/watch?v=Ql9-EmXJdS4) 

