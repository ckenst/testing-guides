# Guideword Heuristics

- http://www.qualityperspectives.ca/resources_mnemonics.html
- Might need to break this apart and put into a directory for easier consumption

**FCC CUTS VIDS**

A test touring heuristic.

- Feature tour: Move through the application and get familiar with all the controls and features you come across.
- Complexity tour: Find the five most complex things about the application.
- Claims tour: Find all the information in the product that tells you what the product does.
- Configuration tour: Attempt to find all the ways you can change settings in the product in a way that the application retains those settings.
- User tour: Imagine five users for the product and the information they would want from the product or the major features they would be interested in.
- Testability tour: Find all the features you can use as testability features and/or identify tools you have available that you can use to help in your testing.
- Scenario tour: Imagine five realistic scenarios for how the users identified in the user tour would use this product.
- Variability tour: Look for things you can change in the application - and then you try to change them.
- Interoperability tour: What does this application interact with?
- Data tour: Identify the major data elements of the application.
- Structure tour: Find everything you can about what comprises the physical product (code, interfaces, hardware, files, etc…).

- http://michaeldkelly.com/blog/2005/9/20/touring-heuristic.html

**MCOASTER**

A test reporting heuristic.

- Mission
- Coverage
- Obstacles
- Audience
- Status
- Techniques
- Environment
- Risk

- http://michaeldkelly.com/blog/2005/8/19/coming-up-with-a-heuristic.html

**RCRCRC**

A regression testing heuristic.

- Recent: new features, new areas of code are more vulnerable
- Core: essential functions must continue to work
- Risk: some areas of an application pose more risk
- Configuration sensitive: code that’s dependent on environment settings can be vulnerable
- Repaired: bug fixes can introduce new issues
- Chronic: some areas in an application may be perpetually sensitive to breaking

- http://karennicolejohnson.com/2009/11/a-heuristic-for-regression-testing/

**REACT**

A bug reporting heuristic.

- Reproduce:
- Explore:
- Analyze:
- Communicate:
- Triage

- http://www.brendanconnolly.net/react-to-bugs/

**RIMGEN**

A bug reporting heuristic for Bug Advocacy.

- Replicate.
- Isolate.
- Maximize.
- Generalize.
- Externalize
- Neutral Tone. (Formerly 'And Say it Clearly and Dispassionately')


**SFDIPOT** (San Francisco Depot)

A test strategy heuristic.

- Structure
- Function
- Data
- Integrations
- Platform
- Operations
- Time

**STRIDE**

The STRIDE Threat Model for security testing.

- Spoofing identity. An example of identity spoofing is illegally accessing and then using another user's authentication information, such as username and password.
- Tampering with data. Data tampering involves the malicious modification of data. Examples include unauthorized changes made to persistent data, such as that held in a database, and the alteration of data as it flows between two computers over an open network, such as the Internet.
- Repudiation. Repudiation threats are associated with users who deny performing an action without other parties having any way to prove otherwise—for example, a user performs an illegal operation in a system that lacks the ability to trace the prohibited operations. Nonrepudiation refers to the ability of a system to counter repudiation threats. For example, a user who purchases an item might have to sign for the item upon receipt. The vendor can then use the signed receipt as evidence that the user did receive the package.
- Information disclosure. Information disclosure threats involve the exposure of information to individuals who are not supposed to have access to it—for example, the ability of users to read a file that they were not granted access to, or the ability of an intruder to read data in transit between two computers.
- Denial of service. Denial of service (DoS) attacks deny service to valid users—for example, by making a Web server temporarily unavailable or unusable. You must protect against certain types of DoS threats simply to improve system availability and reliability.
- Elevation of privilege. In this type of threat, an unprivileged user gains privileged access and thereby has sufficient access to compromise or destroy the entire system. Elevation of privilege threats include those situations in which an attacker has effectively penetrated all system defenses and become part of the trusted system itself, a dangerous situation indeed.

According to the website: When you are considering threats, it is useful to ask questions such as these:

- How can an attacker change the authentication data?
- What is the impact if an attacker can read the user profile data?
- What happens if access is denied to the user profile database?
- https://msdn.microsoft.com/en-US/library/ee823878.aspx

(Other Guidewords can be found in their respective directories)
