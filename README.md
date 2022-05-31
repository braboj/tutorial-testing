<p align='center'>
 <img src='Assets/banners/banner-bhai-branko.png' />
</p>

------------------------------------------------------------------------------------------------
### Introduction

Testing is part of the Quality Assurance (QA) and Quality Control (QC) processes. It the narrow 
sense it is the verification and validation of the software during the software development
process. In practice the testers usually do not have any knowledge about the internals of the
product and procede using the black box testing methodology.  In this case the tester is required
to identify the required function, supply input and compare it with the expected output. 

------------------------------------------------------------------------------------------------
### Testing concepts

![Test types](Assets/images/test-types.png)

The black box testing is usually divided in two parts. First the functional testing is
used to verify that the software is working correctly.

- When a tested element has a valid input X do I see a correct output Y?
- When a tested element has an invalid input X do I see the error Y?

After the development of the product and no further bugs are discovered the non-functional
testing is used to validate the software.

- Is the product API covering the requirements by the client?
- Is the product more performant than previous releases or competiors?
- Is the software secure to be used in trusted enviromnents?
- Is the software robus enough to handle large amount of data?

------------------------------------------------------------------------------------------------
### Testing techniques

- Boundary value
- Equivalence partitioning
- Decision tables
- Ad-hoc testing

------------------------------------------------------------------------------------------------
### Tester activities

- Review software documentation
- Design and document test scenarios
- Design and document test plans
- Design or develop automated testing tools.
- Document and report software defects using a bug tracking system
- Provide feedback and recommendations to developers on software usability and functionality.
- Create or maintain databases of known test defects.

------------------------------------------------------------------------------------------------
### Minimal requirements for the test case design

- Each test suit **MUST** have a name convention allowing grouping in categories
- Each test case **MUST** follow the test suite name convention
- Each test case **MUST** have an unique ID
- Each test case **MUST** be atomic and test only single features
- Each test case **MUST** have a short description
- Each test case **MUST** have a short algorithm with easy to follow steps
- Each test case **SHOULD** return PASSED, FAILED or SKIPPED for better coverage analysis
- Each test case **SHOULD** be able to be reused in different test groups

------------------------------------------------------------------------------------------------
### Example

#### ID
OMB_API_01_01_01

#### Description
The DUT MUST use port 502 when the port is set to 0 in the configuration packet.

#### Results
PASSED, FAILED

#### Algorithm

1. Configure the DUT as a server in message mode and tcpPort set to 0
2. Create a simulated modbus client and connect to port 502 (default Modbus port)
3. Send data to the server
4. Wait for an indication packet from the stack
5. Send a response to the indication packet
6. Validate the response sent by the stack on the bus
7. If all steps succeeded then the test has passed

------------------------------------------------------------------------------------------------
### Glossary

#### Verification
The process of monitoring whether the software runs correctly.

#### Validation
The process of monitoring whether the software confomrs to the customers needs.

------------------------------------------------------------------------------------------------
### Selected references
- [ISO 25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010)
- https://www.triad.co.uk/news/testing-vs-qa/#:~:text=QA%20and%20Testing%20are%20not,quality%20within%20a%20technical%20arena.
- https://www.bmc.com/blogs/how-to-write-test-cases-for-software/
- https://www.javatpoint.com/software-engineering-sdlc-models
- https://www.scnsoft.com/blog/software-development-models
- https://echoua.com/sdlc-models-full-guide/
- https://www.sketchbubble.com/en/presentation-spiral-model-in-sdlc.html
- https://www.geeksforgeeks.org/software-testing-techniques/
- https://www.guru99.com/software-testing-techniques.html
- https://www.swtestacademy.com/software-testing-techniques/
- https://www.softwaretestinghelp.com/guide-to-functional-testing/

------------------------------------------------------------------------------------------------
### Credits
 - [Branimir Georgiev](https://github.com/braboj)


