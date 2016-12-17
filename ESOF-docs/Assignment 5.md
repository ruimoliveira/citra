#**Assignment 5: Software Maintenance/Evolution**

[![BCH compliance](https://bettercodehub.com/edge/badge/ruimoliveira/citra)](https://bettercodehub.com)

The goal of this last assignment is to evolve a feature in the selected project and document how the process taken to evolve the feature (that is, document the change impact analysis and feature evolution)

In particular, this report should discuss the following

##**Discuss Software Maintainability using the SIG metrics (plus add the badge to your .md file).**
Students should contact the recitations professor in order to be added to the ESOF organization to be able to automatically compute the metrics of interest using the service https://bettercodehub.com/. 
See the pdf with an example of a report of the interesting metrics and a description of what they represent. 

**Write Short Units of Code**
![alt tag](http://icecream.me/uploads/2439771fc8bbb7c4ee0e624c6de49379.png)
**Write Simple Units of Code**
![alt tag](http://icecream.me/uploads/dee6c584c04681b7430ce5e2ebfed6af.png)
**Write Code Once**
![alt tag](http://icecream.me/uploads/d6adb4c813d0fb5804b34616c0405c2e.png)

There are some sections of the code that define the same object in different places. We dont know the reason as why this happened, probably different people doing this functions which resulted in writing the same thing twice. This also happens with functions that do exactly the same thing or use a considerable amount of code that has already been used somewhere else. It probably has the same reason behind this issue. So we can conclude that this tool was effective in finding repeated code and Citra has a considerable amount of it.

**Keep Unit Interfaces Small**
![alt tag](http://icecream.me/uploads/d8e1c1837eac716afed48c715fbcf22c.png)

Citra tends to use functions with many parameters (more than 4) and we think it could probably be easy to group similar parameters into objects, reducing then the number of arguments, thus turning the code easiert to read.

**Separate Concerns in Modules**
![alt tag](http://icecream.me/uploads/b638bf71ef433547c98189d286bf70a4.png)
**Couple Architecture Components Loosely**
![alt tag](http://icecream.me/uploads/9cad7ee9cc1f7c48e0588e5be9ed9a93.png)

**Keep Architecture Components Balanced**
![alt tag](http://icecream.me/uploads/6be4a21baf42cbe198e878a61bdd251b.png)

We agree with this result because the way the code is distributed in the source folder makes it fairly easy to locate whatever it is that we are trying find in order to change/implement. It has a structure of packages and sub-packages with very straight forward names. There is on component that has a lot more code than others (3x more) but the component size uniformity is rather good.

**Keep Your Codebase Small**
![alt tag](http://icecream.me/uploads/dcf687344483c3f60981ac2f802d32cf.png)

**Automate Tests**
![alt tag](http://icecream.me/uploads/73f2cc85840f5ade5f5da84688cab1b6.png)

Since there isn't a directory called "/test/", this tool will assume there aren't any tests made, unless we include them in the configuration file. Citra has currently 0 tests as said in previous assignments so there aren't any files to be included.

**Write Clean Code**
![alt tag](http://icecream.me/uploads/89f79fc483a9a9b3c3b1de7fc46d409e.png)

We do agree with this guideline result but there are certain aspects of it wihich we don't understand. For example, how does and algorithm determines if a variable name is appropriate or not or how does it determine if a comment is useless or not. Some of the marked lines where comments with "//TODO" statements. We disagree with this measure because it gives an idea of what is still there to be done and (sometimes) who is gonna do it. Of course when it is done, the comment will be removed, so we dont think it should be considered a useless comment.

Grade: 4pts

##**Report evolution process (change impact analysis and implementation)**
Briefly describe how the feature you decided to evolve was identified; why you decide to evolve that particular feature? How did you locate the parts in the source code that needed to be modified; etc.  

Grade: 12pts

##**Link to pull request**

Grade: 4pts

Submission date (i.e., last commit to the repository): 23:59, 18-12-2016.

**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

 -[Rui Miguel Oliveira](https://github.com/ruimoliveira)
