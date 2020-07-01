# Test Techniques

Most of this information is from BBST Test Design, BBST Exploratory test slides and from Lessons Learned in Software Testing. Also from Kaner & Fiedler's Test Techniques Mind map. 

This isn't meant to be a complete taxonomy but a partial listing. 

A test technique is a method of designing, running and interpreting the results of tests.

## Testers

People-Based Testing; Who does the testing?

Tester-based techniques focus on who does the testing which might have little to do with what you imagine will happen.

### User testing

- Testing with the types of people who typically use the product. - Kaner, Bach, Pettichord (2002)

### Alpha testing

- In-house testing performed by the test team. - Kaner, Bach, Pettichord (2002)

### Beta testing

- A type of user testing that uses testers who aren't part of the organization and who are members of your products target market. - Kaner, Bach, Pettichord (2002)

### Bug bashes

- In-house testing using anyone who is available. - Kaner, Bach, Pettichord (2002)

### Subject-matter expert testing

- Give the product to an expert on some issues addressed by the software and request feedback (bugs, criticisms, and compliments). - Kaner, Bach, Pettichord (2002)

### Paired testing

- Two testers work together to find bugs.

### Eat your own dog food

- Your company uses and relies on prerelease versions of its own software.

### Localization testing

## Coverage

Coverage-Based Testing is what gets tested.

In principle, coverage-based techniques direct you to run every test of a given type. In practice, you probably won't but you might measure your coverage of that type of testing

### Function testing

- Test every function, one by one. Test the function thoroughly, to the extent you can say with confidence that the function works.
- Create a Function List
- Glass box function testing is usually called unit testing
- Sometimes called feature testing

### Function integration testing

- Test several functions or features together, to see how they work together.
- Sometimes called feature integration testing

### Menu tour

- Walk through all of the menus and dialogs in a GUI product, taking every choice available. - Kaner, Bach, Pettichord (2002)

### Domain testing

- A domain is a (mathematical) set that includes all possible values of a variable of a function. The variables might be input or output variables. For each variable, you partition its set of possible values into equivalence classes and pick a small number of representatives from each class. - Kaner, Bach, Pettichord (2002)
- Use domain testing when you are just learning the program; working through the program with the goal of finding every variable and testing it is a good way to find bugs.

### Equivalence class analysis

- An equivalence class is a set of values for a variable that you consider equivalent. Tests are equivalent if you believe that they all do the same thing. Once you've found an equivalence class, test only one or two of its members.
- Part of domain testing

### Boundary testing

- An equivalence class is a set of values. If you map them onto a number line, the boundary values are the smallest and largest members of the class. In boundary testing you test these and you also test the boundary values of nearby classes that are just smaller than the smallest member of the class you're testing and just larger than the largest member of the class you're testing.
- Part of domain testing

### Best representative testing

- A best representative of an equivalence class is a value that is at least as likely as any other value in the class to expose an error in the software.

### Test Idea Catalogs

- For each type of input field, you can develop a fairly standard set of tests and reuse it for similar fields in this product and later products. - Kaner, Bach, Pettichord (2002)
- Also called input field test catalogs or matrices

### Map and test all the ways to edit a field

- You can often change the value of a field in several ways. - Kaner, Bach, Pettichord (2002)

### Logic testing

- Variables have relationships in the program. Logic testing attempts to check every logical relationship in the program. Cause-effect graphing works here.

### State-based testing

- A program moves from state to state. In a given state, some inputs are valid and others are ignored or rejected. In state-based testing, you walk the program through a large set of state transitions (state changes) and check the results carefully, every time.
- Sometimes called State Transitions

### Path testing

- A path includes all of the steps that you took or all of the statements that the program passed through in order to get to your current state. Path testing involves many paths through the program. - Kaner, Bach, Pettichord (2002)

### Statement and branch coverage

- You achieve 100 percent statement coverage when your tests execute every statement (or line of code) in the program. You achieve 100 percent statement and branch coverage if you execute every statement and every branch from one statement to another.

### Configuration coverage

- Configuration coverage measures the percentage of configuration tests that you have run (and the program has passed), compared to the total number of configuration tests that you plan to run.

### Specification-based testing

- Testing focused on verifying every factual claim (shown to be true or false) that is made about the product in the specification. - Kaner, Bach, Pettichord (2002)

### Requirements-based testing

- Testing focused on proving that the program satisfies every requirement in a requirements document. - Kaner, Bach, Pettichord (2002)

### Combination testing

- Testing two or more variables in combination with each other. - Kaner, Bach, Pettichord (2002)

### Localization testing

- Testing focused on verifying that the program conforms to a particular locale or culture.

### Compliance-driven testing

### User Interface testing

### Tours

I've listed all of the tours from the BBST Test Design class but that's it. There are  many more tours available. 

- Function or feature tour

	- Menu's and Windows tour
	- Mouse and Keyboard tour

- Transaction tour
- Error message tour
- Variables tour
- Data tour
- Sample Data tour
- Structure tour

	- Code
	- Data
	- Interfaces

- Operational modes tour
- Sequence tour
- Claims tour
- Benefits tour
- Market Context tour
- User tour
- Life History tour

	- Lead into Scenario Testing

- Configuration tour
- Interoperability tour
- Compatibility tour
- Testability tour
- Specified-risk tour

	- Leads to Risk Catalog

- Extreme Value tour
- Complexity tour

## Risks

Risk-based testing or Potential problems. Why you are testing (the risks you are testing for). 

### Boundary testing

### Quicktests

- A quicktest is an inexpensive test, optimized for a common type of software error, that requires little time or product-specific preparation or knowledge to perform. They are a great way to start testing a product. - BBST Foundations

### Constraints

- Input constraints

	- A constraint is a limit on what the program can handle. - Kaner, Bach, Pettichord (2002)

- Output constraints

	- The inputs were legal, but they led to output values that the program could not handle. - Kaner, Bach, Pettichord (2002)

- Computation constraints

	- The inputs and outputs are fine but in the course of calculating a value (that will lead to an output), the program fails. - Kaner, Bach, Pettichord (2002)

- Storage (or data) constraints

	- Inputs, outputs, and calculations are legal, but the operations run the program out of memory or yield data files that are too enormous to process.

### Local expressions

### Stress testing

### Load testing

### Performance testing

### History-based testing

### Risk-based multivariable testing

### Usability testing

### Configuration/compatibility testing

### Interoperability testing

### Long-sequence regression

### Additional tips

- If you do risk-based testing, also do comparable non-risk based testing to test for the risk you missed.
- Test for timing issues.
- When you create a test, always create a test procedure that will force the program to use the test data that you have entered, allowing you to determine whether it's using that data incorrectly. - Whittaker (2002)

## Activities

Activity-Based Testing; How you test.

These techniques focus on "how to" test and might most closely match the classical notion of a "technique."

### Guerilla testing

- A fast and vicious attack on the program. A form of exploratory testing that is usually time-boxed and done by an experienced exploratory tester. - Kaner, Bach, Pettichord (2002)

### All-Pairs testing

### Random testing

### Use cases

- Tests derived from use cases. Also called use case flow tests or scenario tests.

### Scenario testing

- A scenario test normally involves four attributes: 1 The test must be realistic and it should reflect something that customers must do; 2 the test should be complex, involving several features, in a way that should be challenging to the program; 3 It should be easy and quick to tell whether the program passed or failed the test; 4 A stakeholder is likely to argue vigorously that the program should be fixed if it fails this test. - Kaner, Bach, Pettichord (2002)

### Installation testing

- Install the software in the various ways and on the various types of systems that it can be installed. Check which files are added or changed on disk. Does the installed software work? What happens when you uninstall? - Kaner, Bach, Pettichord (2002)

### Regression testing

- Regression testing involves reuse of the same tests, so you can retest after change. - Kaner, Bach, Pettichord (2002)
- Bug fix regression

	- After reporting a bug and hearing later on that it's fixed. Prove the fix was no good.

- Old bugs regression

	- Prove that a change to the software has caused an old bug fix to become unfixed.

- Side-effect regression (stability)

	- The goal is to prove that the change has caused something that used to work to now be broken.

### Load testing

- The program or system under test is attacked, by being run on a system that is facing many demands for resources. Under a high load, the system will probably fail, but the pattern of events lading to the failure will point to vulnerabilities in the software or system under test that might be exploited under more normal use of the software under test.

### Long-sequence testing

- Testing done overnight or for days or weeks. The goal is to discover errors that short sequence tests will miss. Examples of errors include wild pointers, memory leaks, stack overflows, etc. - Kaner, Bach, Pettichord (2002)

### Performance testing

- These tests are usually run to determine how quickly the program runs, in order to decide whether optimization is needed. But the tests can expose many other bugs.

### High Volume Automated Testing

- http://kaner.com/?p=278

- A general concept with multiple techniques

## Evaluation / Oracle

Evaluation-Based Testing.

How to tell whether the test passed or failed. Build a set of tests around a well-specified oracle

An oracle is an evaluation tool that will tell you whether the program has passed or failed a test. In HiVAT the oracle is probably another program that generates results or checks the software under test's results. The oracle is generally more trusted than the software under test, so a concern flagged by the oracle is worth spending time and effort to check.

### Function equivalent testing

### Mathematical oracle

### Constraint checks

### Self-verifying data

- The data files you use in testing carry information that lets you determine whether the output data is corrupt.

### Comparison with saved results

- Regression testing (typically, but not always automated) in which pass or fail is determined by comparing the results you got today with the results from last week. If the result was correct last week, and it's different now, the difference might reflect a new defect.

### Comparison with a specification or other authoritative document

- A mismatch with the specification could be an error.

### Heuristic consistency

- Consistency is an important criterion for evaluating a program. Inconsistency may be a reason to report a bug, or it may reflect intentional design variation. 
- We work with 7 main consistency heuristics

### Diagnostics-based testing

### Verifiable state models

## Desired Result

Document focused testing runs a set of tests primarily to collect data needed to fill out a form or create a clearly-structured report

### Smoke testing

- Same thing as build verification?
- This type of side-effect regression testing is done with the goal of proving that a new build is not worth testing.

### Confirmation testing

### User acceptance testing

### Certification testing

## Glass box techniques

### Unit tests

### Functional tests below the UI level

### Boundary testing

### State transitions

### Risk-based

### Dataflows

### Program slicing

### Protocol testing

### Diagnostics-driven testing

### Performance testing

### Compliance-focused testing

### Glass-box regression testing

### Glass-box decision coverage

### Glass-box path coverage

## Testing Approaches

Testing approaches are different than techniques. Include the BBST definitions. 

You can use any techniques across any approach. Approaches just like techniques can overlap. 

### Exploratory testing

- We expect the tester to learn, throughout the project, about the project, its market, its risk, and the ways in which it has failed previous tests. New tests are constantly created and used. They're more powerful than older tests because they're based on the tester's continuously increasing knowledge.

### Scripted testing

- Manual testing, typically done by a junior tester who follows a step-by-step procedure written by a more senior tester.
- Automated test execution or comparison by a machine

### Glass box testing

### Black box testing

