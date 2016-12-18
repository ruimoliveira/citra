<h1 align="center">Assignment 5</h1>
<h1 align="center">Software Maintenance/Evolution</h1>
[![BCH compliance](https://bettercodehub.com/edge/badge/ruimoliveira/citra)](https://bettercodehub.com)

In Software Engineering, software maintenance and evolution is discribred as an optimization process of an already developed software project. In which there should be some feature improvement, error correction/prevention, adaptation to any change in system requirements and new features. For some projects, these changes can be expensive, but since Citra is an open source project, the only currency is time.

##Software Maintainability
Students should contact the recitations professor in order to be added to the ESOF organization to be able to automatically compute the metrics of interest using the service https://bettercodehub.com/. 
See the pdf with an example of a report of the interesting metrics and a description of what they represent. 

**Write Short Units of Code**
![alt tag](http://icecream.me/uploads/2439771fc8bbb7c4ee0e624c6de49379.png)
**Write Simple Units of Code**
![alt tag](http://icecream.me/uploads/dee6c584c04681b7430ce5e2ebfed6af.png)
**Write Code Once**
![alt tag](http://icecream.me/uploads/d6adb4c813d0fb5804b34616c0405c2e.png)

There are functions that do exactly the same thing or use a considerable amount of code that has already been used somewhere else. But most of the cases the functions are in different components or the objects are not exactly the same. So it becomes hard to reuse that code and the solution to be applied in case of bug is to correct it in the different files. Therefore, we don't agree with the result of this measure.

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

A large system takes more effort to analyze, test and modify. Therefore changing a part of a system or a functionality of one is more costly the bigger the system is. So its better to keep the system as small as possible. Citra has a medium-sized system, evaluated in 5 man-years which is way below the 20 man-year mark. We agree with this test result because Citra is not a big project, but rather a medium-sized one.

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
