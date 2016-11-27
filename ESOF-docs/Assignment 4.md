
The goal of this fourth assignment is to document the project according to the current state with respect to verification and validation. This assignment requires you to carefully and thoroughly inspect the source code. You're also free to choose (static/dynamic) testing tools to help you test and debug and project. 

In particular, this report should discuss the following

Discuss Software Testability and Reviews: controllability, observability, isolateability, separation of concerns, understandability, heterogeneity.  
>Grade: 6pts

**Controllability**

Before starting to test, developers usually ask the question "How hard it is to to test this component?". Controllability determines the work it takes to test the CUT (component under test) to an extent of which function will be called in the test cases. The more dependencies it has with other components, the harder it is to test, because we need to find simulations of those interactions that the CUT can have.

//In CITRA, ...

**Observability**

Now that we know the controllability of a component, what do we need to do so the test cases pass? Observability measures the dificulty of caputring component's output and determines if this output is correct. It is a simple thing if a component only does simple functions, but if it has accumulated some inputs it can be quite tricky to confirm that the current input is related to the output.

//In CITRA, ...

**Isolateability**

Isolateability decides whether it is possible to test each function output isolated or if we have to process a number of functions before we can evaluate the output. The first case is the optimal choice but it may not be possible. The latter will increase the time of solution in case of error because there is a lot of code to go through.

//In CITRA, ...

**Separation of concerns**

Separation of concerns is the name of a design which means that a project should be separated into different sections, in order for each section to deal with a determined concern (data that changes the code). The main use of this design is to be able to reuse certain some sections and it is easier to develop each section independently from others.

//In CITRA, ...

**Understandability**

Evalutes whether the CUT is well documented and if a person reading it would be able to comprehend it easily.

//In CITRA, ...

**Heterogeneity**

Heterogeneity determines if the use of external technologies like libraries require some tests too. Normally, projects tend to use libraries that are already tested. However, when there is a need to use a library that isn't fully tested, developers need to add some test cases to verify the output of the functions that will be used.

//In CITRA, ...

Report Test Statistics and analytics:  e.g., number of test cases, percentage of coverage, number of flaky tests, etc. (see links of projects in moodle for inspiration)

>Grade: 8pts

Identify a new bug and/or correct a bug
>Grade: 6pts (identification: 4 points; correction: 2 points)

You think your project has no bugs?! Then, you do need to have a compelling story for us to credit you 6pts! 
