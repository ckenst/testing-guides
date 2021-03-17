# Unit Testing

A small test that makes sure a certain unit of your codebase works as intended. They have the smallest and narrowest scope of all your tests which result in very quick run times. What is a unit? It depends on your context. 

Here's an example from Martin Fowler: 
"If you're working in a functional language a unit will most likely be a single function. Your unit tests will call a function with different parameters and ensure that it returns the expected values. In an object-oriented language a unit can range from a single method to an entire class." [Martin Fowler](https://martinfowler.com/articles/practical-test-pyramid.html)


## Test Doubles

Test Doubles replace a real thing with a fake thing, returning a canned response instead (that you specify ahead of time in your test). 

- Dummies: objects are passed around but never actually used. Usually they are just used to fill parameter lists.
- Fakes: objects actually have working implementations, but usually take some shortcut which makes them not suitable for production (an InMemoryTestDatabase is a good example).
- Mocks: are pre-programmed with expectations which form a specification of the calls they are expected to receive. They can throw an exception if they receive a call they don't expect and are checked during verification to ensure they got all the calls they were expecting.
- Spies: are stubs that also record some information based on how they were called. One form of this might be an email service that records how many messages it was sent.
- Stubs: provide canned answers to calls made during the test, usually not responding at all to anything outside what's programmed in for the test.

Definitions from [Martin Fowler](https://martinfowler.com/bliki/TestDouble.html)