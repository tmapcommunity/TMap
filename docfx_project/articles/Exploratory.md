Exploratory testing

### What is Exploratory testing?

Exploratory testing is an experience based approach of testing. TMap distinguishes coverage based and experience based testing.  Others use terms like scripted testing and free-style testing, but TMap prefers the division in focus on either experience or coverage, with the advise to always combine both coverage based and experience based testing.
Of the three approaches of experience based testing, Exploratory testing is the most versatile. The other two approaches are checklists and error guessing.

Exploratory testing is the simultaneous designing, executing and result interpreting of tests, and learning. In other words every form of testing in which the tester designs his tests during test execution and the information obtained is reused to design new and improved test cases.

Testing is about creating and executing tests, but more important about covering risks and determining quality, all of that to ultimately gain confidence that an IT solution will bring the expected business value. Exploratory testing is very well suited to gain that confidence because of its interactive nature.

Exploratory testing has many flavors. In most flavors you will find the following characteristics:

- Focus on confidence (risk-based)
- Structured (charter, log, debriefing)
- Session-based & Timeboxed (not too short, not too long)
- Tandem-approach (two testers)
- Combine experience-based and coverage-based testing
- Simultaneous test design, test execution and learning
- Flexible (fit for Agile and DevOps)
- Prepared (test ideas, testing tours)
- Tools (heuristics, checklists, test design tooling, test recording tooling)
- Serious Fun !!

Exploratory testing is structured! It is planned by means of charters with test ideas. It is prepared with a start set of test data and/or test cases and/or testing tours. And for every test, before executing it, the tester(s) must think about the expected result. (the result may be described in a global way or very detailed depending on the goal of the test).
Finally it is logged to keep track of what was tested and what actual results occurred, how these compare to the expectation leading to the observations and anomalies if applicable.

##### Exploratory testing activities:

An exploratory test is structured in three phases:

1.  The preparation phase;

2.  The execution phase;

3.  The reporting phase;

##### Preparation phase

The preparation phase consists of the following actions:

*Determine the scope.*
The scope of the exploratory test can be the user stories agreed on  by the team at the start of the sprint. Sometimes a user story can be divided into (sub) stories. One (sub) story can be the scope of the exploratory test.

*Set a time-box.*
For every (sub) chapter the duration of the test is specified. An exploratory test is time boxed – this means that the execution of an exploratory test is limited by the time. When the time is up, the exploratory test ends.

*Determine the exploratory test team.*
Exploratory testing is mostly done in pairs. Ideally one of the pair is being a test engineer and the second member is a product expert, but that may differ.

*Create an exploratory test charter*

The test charter is a brief document that contains information to prepare for the test session.

##### Execution phase

At the execution phase the following will be done:

*Execute the exploratory test.*

Execute the exploratory test for the applicable (sub) chapter. The test engineer and the product expert are using one and the same terminal. During execution they switch position behind “the steering wheel”. The product expert executes the test while the test engineer logs the test execution to make it possible to repeat the test case. After which they switch roles within the same charter and time-box.

*Logging defects.*
When a defect is found, the defect is reported with reproducible steps and an indication of how often certain unwanted behavior has been observed.

##### Reporting phase

When the time specified in the time box is over, the execution of the exploratory test stops and the following actions take place:

*Evaluate*
When the exploratory test is finished an evaluation of the exploratory test is planned. In this evaluation the behavior of the product and the defects will be discussed with other exploratory test teams, product experts or at least shared within the development team. Maybe multiple sightings of the same or similar behavior have been found. Defects(can be combined) are submitted to the [defect management](http://www.tmap.net/building-blocks/defect-management) system.

*End evaluation*
After all the exploratory tests of (sub) stories have been executed, there will be an final evaluation on the product, to get a good overall feeling of the status.

*Regression test*
If the right logging is used, out of the logged test steps the test engineer can make test cases that can be used in the (automated) regression test. This can be an expanding set for example to be run after every sprint or before an integration milestone takes place.

Based on the knowledge gained during testing, new and better tests are devised to discover information about quality and risks and thus build towards confidence in the business value of the test object.

##### Combining experience based and coverage based testing

Experience based testing and coverage based testing should always be combined. Exploratory Testing will largely benefit from test design techniques to find good ideas for testing, either by applying test design techniques during the test session (for example when you come across a boundary you apply boundary value analysis) or separately (for example to create a specific set of test cases that covers all possible paths of a process flow). This especially is applicable in the common situation where testers are involved in the team already before the software is delivered, so they can use the test basis (e.g. documentation) to make a starting-set of tests within the scope of a specific test charter. During the test session they will then perform the prepared tests, learn from that and devise new tests to execute right away.

To give an example: The charter could be: Testing input fields of a screen. One of the test ideas might be applying equivalence class partitioning and/or boundary value analysis. And then you are free to give some more detail, like ‘age’ less or equal to 18 years. When leaving these charters and test ideas and expected outputs out, it would not be exploratory testing but only be the approach called error guessing.

### People involved

Since Exploratory Testing largely depends on experience it needs people with good testing skills. But also people that know about the subject matter at hand. Often there is not one single person that has all knowledge and skills. Therefore Exploratory Testing is typically done in tandems. One of the two people focuses on the test object and executes the tests, the other focuses on the charter and the documentation of tests in a log and writing anomalies/defect reports.

Preferably a third person assists the team in the debriefing by asking critical questions about the experiences they had during the test-session.

Typically Exploratory Testing is very well suited for people that don’t consider themselves as professional testers. People with a background as end-user, developer, requirements-engineer or operations-specialist find great value in this approach to testing because it leaves them freedom to devise additional tests during the test session so that they don’t have to create all test cases up front when they don’t have a clear idea of the system under test yet.
However, to be able to do proper exploratory testing the people involved do need some training, guidance and coaching because good testing actually is hard work.

Exploratory Testing through its flexible nature aligns very well with the activities of Agile and DevOps teams.

### Artifacts

Charter: A brief document that contains information to prepare for the test session, for example the timebox available, the purpose of the test, the scope (what to test and what not to test), some test ideas and possible test data.

Test log: A list of the inputs and actions used, the expected results and the actual results. Also the observations are listed including references to the anomalies / defect reports.

Anomaly/Defect reports: If any differences between expected and actual results are observed this is logged in an anomaly report (also called defect report). Often a defect management system is used to support this.

Test report: This may be written or just in a debriefing meeting.

Tools: For example for recording the test session to minimize the need for manual logging. But also tools for generating test cases as a start set. And tools for test execution, for example of a regression test (although mostly the regression tests are run separately of the exploratory sessions).

A specific aid for testers are heuristics. A Heuristic is any approach to problem solving, learning, or discovery that employs a practical method not guaranteed to be optimal or perfect, but sufficient for the immediate goals. Examples of heuristics are checklists with common defects or common approaches to defining tests. Even test design techniques may be applied as heuristics.

### Success factors

As described in the TMap HD book, the success of testing heavily depends on the people involved. These people need a wide range of skills, or example (but not limited to) testing skills, domain knowledge, IT-development skills etcetera.

Exploratory testing needs structure. The first important artifact is the charter. A large test object can easily be covered by making a bunch of charters that together cover all relevant features, aspects and attributes. Different teams of testers can execute these charters. The results of the test sessions, as determined during the debriefings, are brought together to establish the overall confidence that was gained about the business value that the test object will deliver.

During drawing up a charter the testers write down test ideas. These are general thoughts about what can be done during the test session. For example specific uses of the test object, application of one or more coverage based test design techniques, and the use of testing tours to structure the test session.

### References

In the book “Neil’s quest for quality”, the musing of Niki van Dreumel of ASR insurances concludes:

In the hands of experts, Exploratory Testing is a structured way to measure the quality of the information system in a relatively short time and to reach an objective view on the risks involved.

Explore It! by Elisabeth Hendrickson

Exploratory Software Testing by James A. Whittaker.