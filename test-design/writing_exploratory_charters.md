# Writing Exploratory Charters

What is exploratory testing?

> Simultaneous learning, test design and test execution. \(Bach\)
>
> A style \(approach\) of software testing that emphasizes the personal freedom and responsibility of the individual tester to continually optimize the value of her work by treating test-related learning, test design, test execution and test result interpretation as mutually supportive activities that run in parallel throughout the project. \(Kaner\)

## How to Write Exploratory Charters

This is based on "A simple charter template" from Elisabeth Hendrickson's awesome book Explore It!, Chapter 2, page 67 of 502 \(ebook\).

Explore \(target\) With \(resources\) To discover \(information\)

* Target: What are you exploring? It could be a feature, a requirement, or a module.
* Resources: What resources will you bring with you? Resources can be anything: a tool, a data set, a technique, a configuration, or perhaps an interdependent feature.
* Information: What kind of information are you hoping to find? Are you characterizing the security, performance, reliability, capability, usability or some other aspect of the system? Are you looking for consistency of design or violations of a standard?

## Examples of Charters

Some of these follow the above format, some don't. As we learn to write charters, the format can differ. Many thanks to Bach's Rapid Software Testing Appendices.

* Explore editing profiles with injection attacks to discover security vulnerabilities
* Explore editing profiles with various login methods to discover surprises
* Explore input fields with JavaScript and SQL injection attacks to discover security vulnerabilities
* Explore catalog features with 10x \# products to discover problems with browsing and searching
* Explore and analyze the product elements of . Produce a test coverage outline.
* Explore large pools of executors running at the same time to discover bad behavior related to race conditions or flaws in claiming runs of reasonably large values.
* Identify and test all claims in the  manual. \(either use checkmark/X/? notation on the printed manual, or list each tested claim in your notes\)
* Define work flows through DecideRight and try each one. The flows should represent realistic scenarios of use, and they should collectively encompass each primary function of the product.
* We need to understand the performance and reliability characteristics of DecideRight as decision complexity increased. Start with a nominal scenario and scale it up in terms of number of options and factors until the application appears to hang, crash, or gracefully prevent user from enlarging any further.
* Test all fields that allow data entry \(you know the drill: function, stress, and limits, please\)
* Analyze the file format of a DecideRight scenario and determine the behavior of the application when its elements are programmatically manipulated. Test for error handling and performance when coping with pathological scenario files.
* Check UI against Windows interface standards.
* Is there any way to corrupt a scenario file? How would we know it’s corrupted? Investigate the feasibility of writing an automatic file checker. Find out if the developers have already done so.
* Test integration with external applications, especially Microsoft Word.
* Determine the decision analysis algorithm by experimentation and reproduce it in Excel. Then, use that spreadsheet to test DecideRight with complex decision scenarios.
* Run DecideRight under AppVerifier and report any errors.

## Time-Box Sessions

Exploring can be an open-ended endeavor. To help guide those explorations you can use time boxed sessions for structuring and organizing your effort.

Refer to session-based test management \(SBTM\).

