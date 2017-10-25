# Lesson 1 - Introduction to Object Oriented Design

## Learning Objectives
- The student will be able to describe the importance of the DRY principle 
- The student will be able to demonstrate coding using the DRY principle
- The student will be able to describe why the DRY principle is required to implement the single responsibility principle
- The student will be able to describe why DRY is required to implement the open Open/closed principle


## Don't Repeat Yourself

The Don’t Repeat Yourself (DRY) principle states that duplication in logic should be eliminated via abstraction; duplication in process should be eliminated via automation.  The DRY princilple is the cornerstone of object oriented design and faciltates the implementation other principles of good object oriented design namely the [SOLID](https://en.wikipedia.org/wiki/SOLID_(object-oriented_design)) principle.  The SOLID principle is a mneumonic that helps people remember the five basic principles of object oriented design.   The first two principles of SOLID require that DRY principle be obeyed.

## SOLID
- [Single Responsibility](https://en.wikipedia.org/wiki/Single_responsibility_principle)
- [Open/closed](https://en.wikipedia.org/wiki/Open/closed_principle)
- [Liskov substitution principle](https://en.wikipedia.org/wiki/Liskov_substitution_principle)
- [Interface segregation principle](https://en.wikipedia.org/wiki/Interface_segregation_principle)
- [Dependency inversion principle](https://en.wikipedia.org/wiki/Dependency_inversion_principle)


## Why is DRY Important - Single Point of Control
Duplicate code adds to [technical debt]()https://en.wikipedia.org/wiki/Technical_debt.  Whether the duplication stems from Copy Paste Programming or poor understanding of how to apply abstraction, it decreases the quality of the code.  Duplication makes maintaining code more difficult because it makes finding bugs more difficult due to the fact there will be more than one place in your code that has the same bug.  It also makes adding features to your program more difficult because duplication introduces more than one place that controls a process within your program.  For these reasons the [Single Responsibility](https://en.wikipedia.org/wiki/Single_responsibility_principle) of SOLID requires that you not repeat yourself when writing code.  Violating DRY / Single Responsibility will make it difficult for you to fix or extend your code in the future.  You will evevitably have to fix your code, or extend it to add more features.  Modern software relies on libraries created by other programmers like you.  Sometimes your program will break because a programer "upstream" from you i.e. someone that created a library that you use has decides to change a library used by your program.  When this happens it can introduce a new bug in your program and if you don't have a single point of control for all aspects of your program, it will make fixing your program more difficult.

