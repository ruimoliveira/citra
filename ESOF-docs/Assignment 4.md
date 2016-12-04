##**Software Testability and Reviews**

In the following topics Citra's marks of testability will be discussed, focusing mainly on verification (which consists in ensuring that the product is being well built with the requirements obtained in mind) and validation (which consists in ensuring that the product will meet the intended purpose and the needs of its stakeholers).

Testability, a property applying to empirical hypothesis, involves two components. The effort and effectiveness of software tests depends on numerous factors including properties of the software requirements,properties of the software itself (such as size, complexity and testability),properties of the test methods used,properties of the development- and testing processes and qualification and motivation of the persons involved in the test process.
The testability of software components (modules, classes) is determined by factors such as:

##**Controllability**

Before starting to test, developers usually ask the question "How hard it is to to test this component?". Controllability determines the work it takes to test the CUT (component under test) to an extent of which function will be called in the test cases. The more dependencies it has with other components, the harder it is to test, because we need to find simulations of those interactions that the CUT can have.

In Citra, most of the components have a good controllability since they don't have many dependencies and can be tested fairly easy. However, there are some modules that depends on many other modules input to correctly work. In this case it can become very hard to test the output from this component, which means the controllability is low.

##**Observability**

Now that we know the controllability of a component, what do we need to do so the test cases pass? Observability measures the dificulty of caputring component's output and determines if this output is correct,its the degree to which it is possible to observe (intermediate and final) test results.It is a simple thing if a component only does simple functions, but if it has accumulated some inputs it can be quite tricky to confirm that the current input is related to the output.

Citra's components are divided into small functions but since the project is an emulator, it accumulates large quantities of data. This makes it difficult to test if the output obtained is correct, which makes observability low.

##**Isolateability**

Isolateability decides whether it is possible to test each function output isolated or if we have to process a number of functions before we can evaluate the output. The first case is the optimal choice but it may not be possible. The latter will increase the time to find a solution in case of error because there is a lot of code to go through.

We think that Citra has good isolateability since they divide every component into small functions which makes it easier to find a mistake.

##**Separation of concerns**

Separation of concerns is the name of a design which means that a project should be separated into different sections, in order for each section to deal with a determined concern (data that changes the code). The main use of this design is to be able to reuse certain some sections and it is easier to develop each section independently from others.

Citra does use this design, for example: everything related to audio is emulated in a component, evertything related to video is emulated in another components. And in each there are sub-components that deal with small aspects of the emulation. So we think this approach is quite good.

##**Understandability**

Evalutes whether the CUT is well documented and if a person reading it would be able to comprehend it easily.

In this project, we think documentation of the code is average (at least for a person which is viweing the source code for the first times). The function's names are usually self explanatory. Inside the functions there are examples where it is explained in detail what is happening and examples where that isn't verified. This probably occurs because contributors are not the same and documentation isn't demanded on pull request (it is advised). This later case makes people lose more time than what is supposed to understand what is happening in detail.

##**Heterogeneity**

Heterogeneity determines if the use of external technologies like libraries require some tests too. Normally, projects tend to use libraries that are already tested. However, when there is a need to use a library that isn't fully tested, developers need to add some test cases to verify the output of the functions that will be used.

Citra is using a component which belongs to another OSP. Tests of that component don't cover half of the code, so to be certain that this component properly works, it is necessary to add a lot more tests. In conclusion, Heterogeneity in Citra is below the intended level.

#**Test Statistics and Analysis**

Citra is using [Catch](https://github.com/philsquared/Catch/)-based tests, but currently almost nothing in the Citra Repository is being tested. In the [Dynarmic Repository](https://github.com/MerryMage/dynarmic) (another open source project that is used by Citra to emulate Nintendo's 3DS CPU - ARM11 architecture) has a lot more coverage (40%).

From what we could perceive, the lack of test implementation is due to multiple reasons:

- priorities other than unit testing;
- less contributors willing to do tests, requiring all contributors to do write tests for their code could result in loss of interested contributors;
- since Citra is a reverse engineering project, it is not always clear if testing is being done correctly, that is, if tests results are false positives, if something is working for a particular game, it does not mean it will work on all games.

This means that code quality is garanteed the good old fashion way. The code is working until proved otherwise. This is by all means not the best way to assure code quality in software development, but considering nature of the project at hand, it certainly is the most adequate.

#**Identify a new bug and/or correct a bug**

Acredito em ti Guilherme.

**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

 -[Rui Miguel Oliveira](https://github.com/ruimoliveira)
