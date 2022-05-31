<p align='center'>
 <img src='Assets/banners/banner-bhai-branko.png' />
</p>

------------------------------------------------------------------------------------------------
### Introduction

Testing is part of the Quality Assurance (QA) and Quality Control (QC) processes. It the narrow 
sense it is a validation of the software during the software development process.

------------------------------------------------------------------------------------------------
### Test types

![Test types](Assets/images/test-types.png)

------------------------------------------------------------------------------------------------
### Tester Activities

- Review software documentation
- Design and document test scenarios
- Design and document test plans
- Design or develop automated testing tools.
- Document and report software defects using a bug tracking system
- Provide feedback and recommendations to developers on software usability and functionality.
- Create or maintain databases of known test defects.

------------------------------------------------------------------------------------------------
### Test scenario design

- The test case **MUST** follow a name convetion
- The test case **MUST** have an unique ID
- The test case **MUST** have a short descrition
- The test case **MUST** have a short algorithm with easy to follow steps
- The test case **MUST** be atomic and test only single features
- The test case **SHOULD** be reusable 
- The test case **SHOULD** return PASSED, FAILED or SKIPPED
- The test case **SHOULD** describe all prerequirements

------------------------------------------------------------------------------------------------
### Example

#### ID
OMB_API_01_01_01

#### Description
The DUT MUST use port 502 when the port is set to 0 in the configuration packet.

#### Results
PASSED, FAILED

#### Algorithm

1. Configure the DUT in message mode, the default number of server ports, and tcpPort set to 0
2. Create a simulated client and connect to port 502 (default Modbus port)
3. Send data to the server
4. Wait for an indication packet from the stack
5. Send a response to the indication packet
6. Validate the response sent by the stack on the bus
7. If all steps succeeded then the test has passed


------------------------------------------------------------------------------------------------
### Selected references
- [ISO 25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010)
- https://www.triad.co.uk/news/testing-vs-qa/#:~:text=QA%20and%20Testing%20are%20not,quality%20within%20a%20technical%20arena.
- https://www.bmc.com/blogs/how-to-write-test-cases-for-software/
- https://www.javatpoint.com/software-engineering-sdlc-models
- https://www.scnsoft.com/blog/software-development-models
- https://echoua.com/sdlc-models-full-guide/
- https://www.sketchbubble.com/en/presentation-spiral-model-in-sdlc.html

------------------------------------------------------------------------------------------------
### Credits
 - [Branimir Georgiev](https://github.com/braboj)


