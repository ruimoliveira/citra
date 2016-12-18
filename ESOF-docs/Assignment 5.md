<h1 align="center">Assignment 5</h1>
<h1 align="center">Software Maintenance/Evolution</h1>
[![BCH compliance](https://bettercodehub.com/edge/badge/ruimoliveira/citra)](https://bettercodehub.com)

In Software Engineering, software maintenance and evolution is discribred as an optimization process of an already developed software project. In which there should be some feature improvement, error correction/prevention, adaptation to any change in system requirements and new features. For some projects, these changes can be expensive, but since Citra is an open source project, the only currency is time.

##Software Maintainability

**Write Short Units of Code**
![alt tag](http://icecream.me/uploads/2439771fc8bbb7c4ee0e624c6de49379.png)

Citra does have functions that are big and probably could be made into smaller functions. But the 15 line rule is a little incomprehensive. The bigger the function is, the harder is it to comprhend it, but there may be cases that it may not make sense to take a part of a function out just because it hit the limit of 15 lines. Also in this results there are examples of it counting defines and some big switch cases where it doesn't make sense counting those.

**Write Simple Units of Code**
![alt tag](http://icecream.me/uploads/dee6c584c04681b7430ce5e2ebfed6af.png)

This project consists in emulating software and reverse engineering which makes it really hard to contain the number of branch points lower. There is a considerable amount of cases that may occur in different situations

**Write Code Once**
![alt tag](http://icecream.me/uploads/d6adb4c813d0fb5804b34616c0405c2e.png)

There are functions that do exactly the same thing or use a considerable amount of code that has already been used somewhere else. But most of the cases the functions are in different components or the objects are not exactly the same. So it becomes hard to reuse that code and the solution to be applied in case of bug is to correct it in the different files. Therefore, we don't agree with the result of this measure.

**Keep Unit Interfaces Small**
![alt tag](http://icecream.me/uploads/d8e1c1837eac716afed48c715fbcf22c.png)

Citra tends to use functions with many parameters (more than 4) and we think it could probably be easy to group similar parameters into objects, reducing then the number of arguments, thus turning the code easiert to read.

**Separate Concerns in Modules**
![alt tag](http://icecream.me/uploads/b638bf71ef433547c98189d286bf70a4.png)

Citra tries to separate most of the data they receive properly but the vast majority of it goes to emulating the CPU which makes calls to other classes thus making the CPU handler harder to understand and analyze. Hence the result of this test.

**Couple Architecture Components Loosely**
![alt tag](http://icecream.me/uploads/9cad7ee9cc1f7c48e0588e5be9ed9a93.png)

Citra does have a good separate concerns in components as said in the previous assignment, and we agree with the result of this test.

**Keep Architecture Components Balanced**
![alt tag](http://icecream.me/uploads/6be4a21baf42cbe198e878a61bdd251b.png)

We agree with this result because the way the code is distributed in the source folder makes it fairly easy to locate whatever it is that we are trying find in order to change/implement. It has a structure of packages and sub-packages with very straight forward names. There is on component that has a lot more code than others (3x more) but the component size uniformity is rather good.

**Keep Your Codebase Small**
![alt tag](http://icecream.me/uploads/dcf687344483c3f60981ac2f802d32cf.png)

A large system takes more effort to analyze, test and modify. Therefore changing a part of a system or a functionality of one is more costly the bigger the system is. So its better to keep the system as small as possible. Citra has a medium-sized system, evaluated in 5 man-years which is way below the 20 man-year mark. We agree with this test result because Citra is not a big project, but rather a medium-sized one.

**Automate Tests**
![alt tag](http://icecream.me/uploads/73f2cc85840f5ade5f5da84688cab1b6.png)

Since there isn't a directory called "/test/", this tool will assume there aren't any tests made, unless we include them in the configuration file. Citra has currently 0 tests as said in previous assignments so there aren't any files to be included.

**Write Clean Code**
![alt tag](http://icecream.me/uploads/89f79fc483a9a9b3c3b1de7fc46d409e.png)

We do agree with this guideline result but there are certain aspects of it wihich we don't understand. For example, how does and algorithm determines if a variable name is appropriate or not or how does it determine if a comment is useless or not. Some of the marked lines where comments with "//TODO" statements. We disagree with this measure because it gives an idea of what is still there to be done and (sometimes) who is gonna do it. Of course when it is done, the comment will be removed, so we dont think it should be considered a useless comment.


In conclusion, as explained above there are a few points which we don't agree, especially the useless comments part which doesn't make much sense to us. Some of the points above may not be optional at certain circunstances but overall this tool does the job its supposed to do.


##**Report evolution process (change impact analysis and implementation)**
Citra is an in-development open-source project. Not long ago, it would barely be considered playable, let alone boot commercial games. However, this has changed for the better, and many games run OK on most computers, but that varies per game and per user. In order to run them on lower-end machines, some options need to be configured. There's also a need to configure multiple entries for controls, most of which are not clear, or even debug settings which have almost no explanation. 

For a project that is now starting to reach a wider userbase, this is becoming an issue, with people not knowing what to do. In light of that, we decided that a setup wizard would be a great addition to Citra. It's a rather "simple" implementation, as it does not affect the internal structure of the emulator, and only needs a few modifications to the QT UI, which is located in the citra_qt package.

The idea behind it is straight-forward. On its first run, Citra opens a window with the setup wizard, asking whether you wish to proceed with the guided setup, or just jump straight to the game with default settings. If the user accepts its aid, it goes through the various categories and settings, explaining what to enable and disable based on what the user expects from his situation.


##**Link to pull request**
Sadly, due to time constraints, this segment of the assignment was deliberatly skipped. While the implementation is indeed "simple", it requires knowledge on how to use the QT interface creator. With more pressing subjects at hand, this was deemed lower priority, and thus was not completed in time.


**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

 -[Rui Miguel Oliveira](https://github.com/ruimoliveira)
