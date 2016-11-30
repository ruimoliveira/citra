
The goal of this fourth assignment is to document the project according to the current state with respect to verification and validation. This assignment requires you to carefully and thoroughly inspect the source code. You're also free to choose (static/dynamic) testing tools to help you test and debug and project. 

In particular, this report should discuss the following

Discuss Software Testability and Reviews: controllability, observability, isolateability, separation of concerns, understandability, heterogeneity.  
>Grade: 6pts

**Controllability**

Before starting to test, developers usually ask the question "How hard it is to to test this component?". Controllability determines the work it takes to test the CUT (component under test) to an extent of which function will be called in the test cases. The more dependencies it has with other components, the harder it is to test, because we need to find simulations of those interactions that the CUT can have.

In Citra, most of the components have a good controllability since they don't have many dependencies and can be tested fairly easy. However, there are some modules that depends on many other modules input to correctly work. In this case it can become very hard to test the output from this component, which means the controllability is low.

**Observability**

Now that we know the controllability of a component, what do we need to do so the test cases pass? Observability measures the dificulty of caputring component's output and determines if this output is correct. It is a simple thing if a component only does simple functions, but if it has accumulated some inputs it can be quite tricky to confirm that the current input is related to the output.

Citra's components are divided into small functions but since the project is an emulator, it accumulates large quantities of data. This makes it difficult to test if the output obtained is correct, which makes observability low.

**Isolateability**

Isolateability decides whether it is possible to test each function output isolated or if we have to process a number of functions before we can evaluate the output. The first case is the optimal choice but it may not be possible. The latter will increase the time to find a solution in case of error because there is a lot of code to go through.

We think that Citra has good isolateability since they divide every component into small functions which makes it easier to find a mistake.

**Separation of concerns**

Separation of concerns is the name of a design which means that a project should be separated into different sections, in order for each section to deal with a determined concern (data that changes the code). The main use of this design is to be able to reuse certain some sections and it is easier to develop each section independently from others.

Citra does use this design, for example: everything related to audio is emulated in a component, evertything related to video is emulated in another components. And in each there are sub-components that deal with small aspects of the emulation. So we think this approach is quite good.

**Understandability**

Evalutes whether the CUT is well documented and if a person reading it would be able to comprehend it easily.

In this project, we think documentation of the code is average (at least for a person which is viweing the source code for the first times). The function's names are usually self explanatory. Inside the functions there are examples where it is explained in detail what is happening and examples where that isn't verified. This probably occurs because contributors are not the same and documentation isn't demanded on pull request (it is advised). This later case makes people lose more time than what is supposed to understand what is happening in detail.

**Heterogeneity**

Heterogeneity determines if the use of external technologies like libraries require some tests too. Normally, projects tend to use libraries that are already tested. However, when there is a need to use a library that isn't fully tested, developers need to add some test cases to verify the output of the functions that will be used.

//In CITRA, ...

**Report Test Statistics and analytics:  e.g., number of test cases, percentage of coverage, number of flaky tests, etc. (see links of projects in moodle for inspiration)**

>Grade: 8pts

Citra is using [Catch](https://github.com/philsquared/Catch/)-based tests, currently almost nothing in the Citra Repository is being tested, but the [Dynarmic Repository](https://github.com/MerryMage/dynarmic) (another open source project that is used by Citra to emulate Nintendo's 3DS CPU - ARM11 architecture) has a lot more coverage.
From what we could perceive, no tests were implemented yet mainly due to many reasons.

priority definitions, sometimes it's more important to efficient to focus on coding something and after everything is done code the tests
reverse engineering project (REP), since this is a REP, it is not always clear if testing is being done correctly, that is, if tests results are false positives, so it is best to move 
less contributors willing to do tests, some of the times humans are lazy, and we all fall guilty with that one

so code quality is garanteed the good old fashion way, while(!working) recode();

Identify a new bug and/or correct a bug
>Grade: 6pts (identification: 4 points; correction: 2 points)

You think your project has no bugs?! Then, you do need to have a compelling story for us to credit you 6pts! 
