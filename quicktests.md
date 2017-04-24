# Quicktests

> A quick-test is an inexpensive test, optimized for a common type of software error,
that requires little time or product-specific preparation or knowledge to perform. (Kaner, BBST Slides)

> A quick-test is a cheap test that has some value but requires little preparation, knowledge or time to perform. (RST slides, page 104)

In other words, quicktests are a great way to /start/ testing a product.

## From BBST Slides:

 - User interface design errors
 - Boundaries
 - Overflow
 - Calculations and operations
 - Initial states
 - Modified values
 - Control flow
 - Sequences
 - Messages
 - Timing and race conditions
 - Interface tests
 - Error handling
 - Failure handling
 - File system
 - Load and Stress
 - Configuration
 - Multivariable relationships

## From RST Slides:

 - Happy Path: Use the product in the most simple, expected, straightforward way, just as the most optimistic programmer might imagine users to behave. Perform a task, from start to finish, that an end-user might be expected to do. Look for anything that might confuse, delay, or irritate a reasonable person.
 - Documentation Tour: Look in the online help or user manual and find some instructions about how to perform some interesting activity. Do those actions. Improvise from them. If your product has a tutorial, follow it. You may expose a problem in the product or in the documentation; either way, you’ve found something useful. Even if you don’t expose a problem, you’ll still be learning about the product.
 - Sample Data Tour: Employ any sample data you can, and all that you can—the more complex or extreme the better. Use zeroes where large numbers are expected; use negative numbers where positive numbers are expected; use huge numbers where modestly-sized ones are expected; and use letters in every place that’s supposed to handle numbers. Change the units or formats in which data can be entered. Challenge the assumption that the programmers have thought to reject inappropriate data.
 - Variables Tour: Tour a product looking for anything that is variable and vary it. Vary it as far as possible, in every dimension possible. Identifying and exploring variations is part of the basic structure of my testing when I first encounter a product.
 - Complexity Tour: Tour a product looking for the most complex features and using challenging data sets. Look for nooks and crowds where bugs can hide.
 - File Tour: Have a look at the folder where the program's .EXE file is found. Check out the directory structure, including subs. Look for READMEs, help files, log files, installation scripts, .cfg, .ini, .rc files. Look at the names of .DLLs, and extrapolate on the functions that they might contain or the ways in which their absence might undermine the application.
 - Menus and Windows Tour: Tour a product looking for all the menus (main and context menus), menu items, windows, toolbars, icons, and other controls.
 - Keyboard and Mouse Tour: Tour a product looking for all the things you can do with a keyboard and mouse. Run through all of the keys on the keyboard. Hit all the F-keys. Hit Enter, Tab, Escape, Backspace. Run through the alphabet in order. Combine each key with Shift, Ctrl, and Alt. Also, click on everything.
 - Interruptions: Start activities and stop them in the middle. Stop them at awkward times. Perform stoppages using cancel buttons, O/S level interrupts (ctrl-alt-delete or task manager), arrange for other programs to interrupt (such as screensavers or virus checkers). Also try suspending an activity and returning later.
 - Undermining: Start using a function when the system is in an appropriate state, then change the state part way through (for instance, delete a file while it is being edited, eject a disk, pull net cables or power cords) to an inappropriate state. This is similar to interruption, except you are expecting the function to interrupt itself by detecting that it no longer can proceed safely.
 - Adjustments: Set some parameter to a certain value, then, at any later time, reset that value to something else without resetting or recreating the containing document or data structure.
 - Dog Piling: Get more processes going at once; more states existing concurrently. Nested dialog boxes and non-modal dialogs provide opportunities to do this.
 - Continuous Use: While testing, do not reset the system. Leave windows and files open. Let disk and memory usage mount. You're hoping that the system ties itself in knots over time.
 - Feature Interactions: Discover where individual functions interact or share data. Look for any interdependencies. Tour them. Stress them. I once crashed an app by loading up all the fields in a form to their maximums and then traversing to the report generator. Look for places where the program repeats itself or allows you to do the same thing in different places.
 - Click for Help: At some point, some users are going to try to bring up the context-sensitive help feature during some operation or activity. Does the product’s help file explain things in a useful way, or does it offend the user’s intelligence by simply restating what’s already on the screen? Is help even available at all?
 - Input Constraint Attack: Discover sources of input and attempt to violate constraints on that input. For instance, use a geometrically expanding string in a field. Keep doubling its length until the product crashes. Use special characters. Inject noise of any kind into a system and see what happens. Use Satisfice’s PerlClip utility to create strings of arbitrary length and content; use PerlClip’s counterstring feature to create a string that tells you its own length so that you can see where an application cuts off input.
 - Click Frenzy: Ever notice how a cat or a kid can crash a system with ease? Testing is more than "banging on the keyboard", but that phrase wasn't coined for nothing. Try banging on the keyboard. Try clicking everywhere. I broke into a touchscreen system once by poking every square centimeter of every screen until I found a secret button.
 - Shoe Test: This is any test consistent with placing a shoe on the keyboard. Basically, it means using auto-repeat on the keyboard for a very cheap stress test. Look for dialog boxes so constructed that pressing a key leads to, say, another dialog box (perhaps an error message) that also has a button connected to the same key that returns to the first dialog box. That way you can place a shoe (or Coke can, as I often do, but sweeping off a cowboy boot has a certain drama to it) on the keyboard and walk away. Let the test run for an hour. If there’s a resource or memory leak, this kind of test will expose it.
 - Blink Test: Find some aspect of the product that produces huge amounts of data or does some operation very quickly. For instance, look a long log file or browse database records very quickly. Let the data go by too quickly to see in detail, but notice trends in length or look or shape of the data. Some bugs are easy to see this way that are hard to see with detailed analysis. Use Excel’s conditional formatting feature to highlight interesting distinctions between cells of data.
 - Error Message Hangover: Make error messages happen and test hard after they are dismissed. Often developers handle errors poorly.
 Resource Starvation: Progressively lower memory, disk space, display resolution, and other resources until the product collapses, or gracefully (we hope) degrades.
 - Multiple Instances: Run a lot of instances of the app at the same time. Open the same files. Manipulate them from different windows.
 - Crazy Configs: Modify the operating system’s configuration in non-standard or non-default ways either before or after installing the product. Turn on “high contrast” accessibility mode, or change the localization defaults. Change the letter of the system hard drive. Consider that the product has configuration options, too—change them or corrupt them in a way that should trigger an error message or an appropriate default behavior.
 - Cheap Tools: Learn how to use InCtrl5, Filemon, Regmon, AppVerifier, Perfmon, and Process Explorer, and Task Manager (all of which are free). Have these tools on a thumb drive and carry it around. Also, carry a digital camera. I now carry a tiny 3 megapixel camera and a tiny video camera. Both fit into my coat pockets. I use them to record screen shots and product behaviors. While it’s not cheap, you can usually find Excel on most Windows systems; use it to create test matrices, tables of test data, charts that display performance results, and so on. Use the World-Wide Web Consortium’s HTML Validator at http://validator.w3c.org. Pay special attention to tools that hackers use; these tools can be used for good as well as for evil. Netcat, Burp Proxy, wget, and fuzzer are but a few examples.
