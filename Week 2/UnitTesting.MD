# Unit Testing-related

## How we test a piece of software

We test a piece of software by comparing the result of executing it against *some defined criteria.* We usually name this piece of software the subject under test or SUT.

These pieces of software can be one of these two types, **but not both:**

+ A **query** retrieves some information about the system's state but doesn’t produce any side effects.

+ A **command** produces a change in the state of the system but doesn’t return a response.

## What are test doubles?

When you have to test an object that relies on "collaborators" and you want to be absolutely sure that the tested behavior is provided **ONLY** by the code in the object, you'll most likely need *test doubles*.

## Why test doubles?

Using a test double, you can suppress or keep collaborators under control. This way you can isolate the actual **object under test** from outside influence. Furthermore, you can avoid costly dependencies that can be out of scope or may introduce some sort of penalty.


## Types of test doubles

1. Fakes
2. Stubs
3. Mocks


### Testing queries

Queries are pretty easy to test because we only need to get the response and compare it with the expected outcome.

When testing queries we could use test doubles to replace expensive dependencies and to define their behaviors for the different scenarios. Usually, we will be using *stubs* or *fakes* for that.

### Testing commands

Commands, instead, are a bit trickier to test. We need to verify that we get the expected outcome by looking for their effect on the system. Nevertheless, sometimes we don’t have the possibility to do that because **we can’t use the real dependency and we use a test double.**

We will need doubles to define the collaborators' behavior and verify that we produce the desired effect, expecting that we send the proper messages to them. These kinds of doubles are called spies or *mocks.*


## Testing strategy considerations

When designing the testing strategy for an element or system, there are three related testing aspects:

+ **Scope:** How much of the code does the test touch? Tests can verify a single method, the entire application, or somewhere in between. The tested scope is under test and commonly refer to it as the Subject Under Test, though also the System Under Test or the Unit Under Test.
+ **Speed:** How fast does the test run? Test speeds can vary from milli-seconds to several minutes.
+ **Fidelity:** How "real-world" is the test? For example, if part of the code you're testing needs to make a network request, does the test code actually make this network request, or does it fake the result? If the test actually talks with the network, this means it has higher fidelity. The trade-off is that the test could take longer to run, could result in errors if the network is down, *or could be costly to use.*

See examples: https://developer.android.com/training/testing/fundamentals/test-doubles