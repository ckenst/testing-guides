# Domain Testing 

Domain Testing is our fields most widely taught technique. You might know it by another name, equivalence class analysis or boundary testing. Together these are described as Domain Testing where a domain is a set of set of values.

- Equivalence class is about finding similarity. Two values are in the same class if they are so similar the program would treat them the same way. Testing with one or two best representatives from each class allows us to substantially reduce the number of required tests.

- Boundary testing is about selecting and using a boundary value in an attempt to show the program in-appropriately accepts a value instead of rejecting it.

It should be possible to automate domain tests. 


## Domain Testing Schema Overview

- What are the potentially interesting variables? 
- Which variable are you analyzing?
- What is the primary dimension of this variable?
- What is the type and scale of the primary dimension?
- Can you order the variable?
- Is this variable an input or result?  Why?
- How does the program use this variable?
- What other variables are related to this one?
- How would you partition the variable?
- Lay out the analysis in a classical boundary/equivalence table, including best representatives.
- What tests would you create for the consequences? 
- What are some of the secondary dimensions that apply to this variable? 
- Summarize your analysis with a risk/equivalence table.
- Analyze independent variables that should be tested together
- Analyze variables that hold results
- Analyze non-independent variables. Deal with relationships and constraints
- Identify and list unanalyzed variables. Gather information for later analysis
- Imagine and document risks that don't necessarily map to obvious dimension