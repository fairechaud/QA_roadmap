# Software Testing Life Cycle

<img src="../img/stlc-phases.webp">


|-----|---------|------------|---------|---------|----------|
|Requirement Analysis| Requirements Document available (both functional and non functional) 
 Acceptance criteria defined.
 Application architectural document available.
|  Analyse business functionality to know the business modules and module specific functionalities.
 Identify all transactions in the modules.
 Identify all the user profiles.
 Gather user interface/ authentication, geographic spread requirements.
 Identify types of tests to be performed.
 Gather details about testing priorities and focus.
 Prepare Requirement Traceability Matrix (RTM).
 Identify test environment details where testing is supposed to be carried out.
 Automation feasibility analysis (if required).| 
 Signed off RTM
 Test automation feasibility report signed off by the client |
 RTM
 Automation feasibility report (if applicable)|
| Test Planning	|
 Requirements Documents
 Requirement Traceability matrix.
 Test automation feasibility document.|
 Analyze various testing approaches available
 Finalize on the best-suited approach
 Preparation of test plan/strategy document for various types of testing
 Test tool selection
 Test effort estimation
 Resource planning and determining roles and responsibilities.|
 Approved test plan/strategy document.
 Effort estimation document signed off.|
 Test plan/strategy document.
 Effort estimation document.|
|Test case development	|
 Requirements Documents
 RTM and test plan
 Automation analysis report|
 Create test cases, test design, automation scripts (where applicable)
 Review and baseline test cases and scripts
 Create test data|
 Reviewed and signed test Cases/scripts
 Reviewed and signed test data|
 Test cases/scripts
 Test data|
|Test Environment setup	|
 System Design and architecture documents are available
 Environment set-up plan is available|
 Understand the required architecture, environment set-up
 Prepare hardware and software development requirement list
 Finalize connectivity requirements
 Prepare environment setup checklist
 Setup test Environment and test data
 Perform smoke test on the build
 Accept/reject the build depending on smoke test result|
 Environment setup is working as per the plan and checklist
 Test data setup is complete
 Smoke test is successful|
 Environment ready with test data set up
 Smoke Test Results.|
| Test Execution	|
 Baselined RTM, Test Plan , Test case/scripts are available
 Test environment is ready
 Test data set up is done
 Unit/Integration test report for the build to be tested is available|
 Execute tests as per plan
 Document test results, and log defects for failed cases
 Update test plans/test cases, if necessary
 Map defects to test cases in RTM
 Retest the defect fixes
 Regression Testing of application
 Track the defects to closure|
 All tests planned are executed
 Defects logged and tracked to closure|
 Completed RTM with execution status
 Test cases updated with results
 Defect reports|
|Test Cycle closure	|
 Testing has been completed
 Test results are available
 Defect logs are available|
 Evaluate cycle completion criteria based on – Time, Test coverage, Cost, Software Quality, 
 Critical Business Objectives
 Prepare test metrics based on the above parameters.
 Document the learning out of the project
 Prepare Test closure report
 Qualitative and quantitative reporting of quality of the work product to the customer.
 Test result analysis to find out the defect distribution by type and severity|
 Test Closure report signed off by client|
 Test Closure report
 Test metrics