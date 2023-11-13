# Integers

> What are the interesting input tests for a simple integer field?

## Integers

* Nothing
* Empty field \(clear the default value\)
* Whitespace only \(tab, space\)
* 0
* Valid value
* At lower bound \(LB\) of range
* At lower bound \(LB\) of range − 1
* At upper bound \(UB\) of range
* At upper bound \(UB\) of range + 1
* Far below the LB of range
* Far above the UB of range
* At LB number of digits or characters
* At LB − 1 number of digits or characters
* At UB number of digits or characters
* At UB + 1 number of digits or characters
* Far more than UB number of digits or characters
* Negative Nondigits, especially / \(ASCII character 47\) and : \(ASCII character 58\)
* Wrong data type \(e. g., decimal into integer\)
* Expressions Leading space
* Many leading spaces Leading zero
* Many leading zeros Leading + sign
* Many leading + signs
* Nonprinting character \(e. g., Ctrl+char\)
* Operating system filename reserved characters \(e. g., “ \* . :”\)
* Language reserved characters
* Upper ASCII \(128-254\) \(a.k.a. ANSI\) characters
* ASCII 255 \(often interpreted as end of file\)
* Uppercase characters Lowercase characters
* Modifiers \(e. g., Ctrl, Alt, Shift-Ctrl, and so on\)
* Function key \(F2, F3, F4, and so on\)
* Enter nothing but wait for a long time before pressing the
* Enter or Tab key, clicking OK, or doing something equivalent that takes you out of the field. Is there a time-out? What is the effect?
* Enter one digit but wait for a long time before entering another digit or digits and then press the Enter key. How long do you have to wait before the system times you out, if it does? What happens to the data you entered? What happens to other data you previously entered?
* Enter digits and edit them using the backspace key, and delete them, and use arrow keys \(or the mouse\) to move you into the digits you’ve already entered so that you can insert or overtype new digits.
* Enter digits while the system is reacting to interrupts of different kinds \(such as printer activity, clock events, mouse movement and clicks, files going to disk, and so on\).
* Enter a digit, shift focus to another application, return to this application. Where is the focus?

