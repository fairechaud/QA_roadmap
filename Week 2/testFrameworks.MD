# Testing frameworks

Utilizing a framework for automated testing will increase a team’s test speed and efficiency, improve test accuracy, and will reduce test maintenance costs as well as lower risks. They are essential to an efficient automated testing process for a few key reasons:  

+ Improved test efficiency
+ Lower maintenance costs
+ Minimal manual intervention
+ Maximum test coverage
+ Reusability of code

## Types of frameworks

There are six common types of test automation frameworks, each with their own architecture and differing benefits and disadvantages. 

+ Linear Automation Framework
+ Modular Based Testing Framework
+ Library Architecture Testing Framework
+ Data-Driven Framework
+ Keyword-Driven Framework
+ Hybrid Testing Framework

### Linear Automation Framework

**This is actually what I used during my time as a Testing Engineer at Ford, testcase were designed in a sequential way, then they were performed by both manual and automated testing teams using in-house solutions and hardware**

With a linear test automation framework, AKA record-and-playback framework, testers don’t need to write code to create functions and the steps are written in a sequential order. In this process, the tester **records each step such as navigation, user input, or checkpoints, and then plays the script back automatically to conduct the test.**

**Advantages:**

+ There is no need to write custom code, so expertise in test automation is not necessary.
+ Fastest ways to generate test scripts since they can be easily recorded in a minimal amount of time.
+ The test workflow is easier to understand for any party involved in testing since the scripts are laid out in a sequential manner.
+ This is also the easiest way to get up and running with automated testing, especially with a new tool. Most automated testing tools today will provide record-and-playback features, so you also won’t need to plan extensively with this framework.

**Disadvantages:**

+ The scripts developed using this framework **aren’t reusable.** The data is hardcoded into the test script, meaning the test cases cannot be re-run with multiple sets and will need to be **modified if the data is altered.**
+ **Maintenance is considered a hassle** because any changes to the application will require a lot of rework. This model is not particularly scalable as the scope of testing expands.

### Modular based testing framework

Implementing a modular framework will require testers to divide the application under test into separate units, functions, or sections, each of which will be tested in isolation. After breaking down the application into individual modules, a test script is created for each part and then combined to build larger tests in a hierarchical fashion. These larger sets of tests will begin to represent various test cases.

*A key strategy in using the modular framework is to build an abstraction layer, so that any changes made in individual sections won’t affect the overarching module.*

**Advantages:**

+ If any changes are made to the application, only the module and it’s associated individual test script will needs to be fixed, meaning you won’t have to tinker with the rest of the application and can leave it untouched.
+ Creating test cases takes less effort because test scripts for different modules can be reused.

**Disadvantages:**

+ Data is still hard-coded into the test script since the tests are executed separately, so you can’t use multiple data sets.
+ Programming knowledge is required to set up the framework.
