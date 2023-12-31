# ISTQB Foundational level - Seven testing principles

## 1. Testing shows the presence of defects, not their absence

Testing can show that defects are present, but cannot prove that there are no defects. Testing reduces the probability of *undiscovered defects remaining in the software* but, even if no defects are found, **testing is not a proof of correctness**. Likewise, testing and solving defects is not guaranteed proof that the software is flawless.

## 2. Exhaustive testing is impossible

Testing everything (all combinations of inputs and preconditions) is **not feasible** except for trivial cases. Rather than attempting to test exhaustively, risk analysis, test techniques, and priorities should be used to focus test efforts.

## 3. Early testing saves time and money

To find defects early, both static and dynamic test activities should be started as early as possible in the software development lifecycle. Early testing is sometimes referred to as *shift left*. Testing early in the software development lifecycle helps reduce or eliminate costly changes.

## 4. Defects cluster together

A small number of modules usually contains most of the defects discovered during pre-release testing, or is responsible for most of the operational failures. Predicted defect clusters, and the actual observed defect clusters in test or operation, **are an important input into a risk analysis used to focus the test effort.**

## 5. The pesticide paradox

If the same tests are repeated over and over again, *eventually these tests no longer find any new defects*. To detect new defects, existing tests and test data **may need changing**, and new tests may need to be written. (Tests are no longer effective at finding defects, just as pesticides are no longer effective at killing insects after a while.) In some cases, *such as automated regression testing*, the pesticide paradox has a beneficial outcome, which is the relatively low number of regression defects.

## 6. Testing is context dependent

Testing is done differently in different contexts. For example, safety-critical industrial control software is tested differently from an e-commerce mobile app. As another example, testing in an Agile project is done differently than testing in a sequential software development lifecycle project (see section 2.1).

## 7. Absence-of-errors is a fallacy

Some organizations expect that testers can run all possible tests and find all possible defects, but principles 2 and 1, respectively, tell us that **this is impossible**. Further, it is a fallacy (i.e., a mistaken belief) to expect that just *finding and fixing a large number of defects will ensure the success of a system*. For example, thoroughly testing all specified requirements and fixing all defects found could still produce a system that is difficult to use, that does not fulfill the users’ needs and expectations, or that is inferior compared to other competing systems.