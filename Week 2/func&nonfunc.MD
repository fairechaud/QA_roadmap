# Software Testing methodologies 

The goal of mixing numerous types of testing methodologies together is to ensure 
that our piece of software can successfully operate in multiple environments and across
a multitude of platforms.

These methodologies are often broken down between functional and non-functional testing.

## Functional testing

+ **Definition:** involves testing the software product against the *business requirements*. It is meant to guarantee that each piece of the software **behaves as expected by the use cases formulated by the design team/business analyst**

Functional testing methodologies include the following, the order is important:

+ Unit testing
+ Integration testing
+ System testing
+ Acceptance testing

## Non-functional testing

+ **Definition:** it primarily focuses on the *operational aspects* of a piece of software. Not so much the behavior or what the output is, rather **how the process is performed and how the output is delivered**

+ Performance testing
+ Security testing
+ Usability testing
+ Compatibility testing

## Full breakdown of each methodology

### Unit testing

Unit testing is the first level of testing and is often *performed by the developers themselves*. It is the process of ensuring individual components of a piece of software at the code level are functional and work as they were designed to. 

Developers in a test-driven environment will typically write and run the tests prior to the software or feature being passed over to the test team. Unit testing can be conducted manually, but **automating the process will speed up delivery cycles and expand test coverage.** Unit testing will also make debugging easier because finding issues earlier means they take less time to fix than if they were discovered later in the testing process. **TestLeft** is a tool that allows advanced testers and developers to shift left with the fastest test automation tool embedded in any IDE.

**When I worked as an Embedded Software Developer at Ford, working on features to deploy road car infotainment systems, I carried out TDD where I was testing every piece of code I was in charge of developing. Similarly, when there was a tool that needed to be made, unit testing was a big part of the way I approached projects.**

+ Keywords: *units, individual components, functions, early debugging, modules, shift left*

### Integration testing

After each unit is thoroughly tested, it is integrated with other units to create modules or components that are designed to perform specific tasks or activities. These are then tested as group through integration testing to ensure whole segments of an application behave as expected (i.e, the interactions between units are seamless). **These tests are often framed by user scenarios, such as logging into an application or opening files**. Integrated tests can be conducted by either *developers or independent testers* and are usually comprised of a combination of **automated functional and manual tests.**

**As part of the development team at Ford, we had an in-house system-building tool that took care of compiling, building and ensuring software packages worked well with each other. Our CI/CD pipeline had multiple checks in place. When I worked on bug fixes, instead of the CI/CD pipeline, I was compiling full system images on my own environment and ensuring individual components were interfacing well.**

+ Keywords: *user scenarios, tasks, group of tests, unit interaction, use cases, automated and manual tests*

### System testing

System testing is a black-box testing method used to evaluate the completed and integrated system, as a whole, to ensure it meets specified requirements. The functionality of the software is tested from end-to-end and is typically conducted by a separate testing team than the development team before the product is pushed into production.

**As part of the dedicated North-American testing team at Ford, we were often tasked with performing spec-based, black-box testing on every single new system version or build before it was greenlit for production. We would break down big updates into suites of different features and tackle them in parallel.**

**Similarly, in my first position as a software developer, we would run multiple use cases everytime a new build was completed. We focused on predefined usecases and targetting how the system was going to be used in the real-world to ensure proper behavior and we combined a few stress testing techniques to reveal corner case or obscure vulnerabilities.**

+ Keywords: *black-box, spec-based, end-to-end, preproduction*

### Acceptance testing 

Acceptance testing is the last phase of functional testing and is used to assess whether or not the final piece of software is ready for delivery. It involves ensuring that the product is in compliance with all of the original business criteria and that it meets the end user’s needs. This requires the product be tested both internally and externally, meaning you’ll need to get it into the hands of your end users for beta testing along with those of your QA team. Beta testing is key to getting real feedback from potential customers and can address any final usability concerns.

### Performance testing

**Performance testing** is a non-functional testing technique used to determine how an application will behave under various conditions. The goal is to test its responsiveness and stability in real user situations. Performance testing can be broken down into four types:

+ *Load testing* is the process of putting **increasing amounts of simulated** demand on your software, application, or website to verify whether or not it can handle what it’s designed to handle.
+ *Stress testing* takes this a step further and is used to gauge how your software will respond **at or beyond its peak load**. The goal of stress testing is to *overload* the application on purpose *until it breaks by applying both realistic and unrealistic load scenarios.* With stress testing, you’ll be able to find the failure point of your piece of software.
+ *Endurance testing* also known as soak testing, is used to analyze the behavior of an application under a specific amount of simulated load over longer amounts of time. The goal is to understand *how your system will behave under sustained use*, making it a longer process than load or stress testing (which are designed to end after a few hours). A critical piece of endurance testing is that **it helps uncover memory leaks.**
+ *Spike testing* is a type of load test used to determine how your software will respond to **substantially larger bursts** of concurrent user or system activity over varying amounts of time. Ideally, this will help you understand *what will happen when the load is suddenly and drastically increased.*
