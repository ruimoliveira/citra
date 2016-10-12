-Brief description of the project 

  Grade: 3pts
  
  Note: This could be in the top-level README.md, which will then include links to all the assigments

-Development Process

  Briefly describe the development process
  
  Grade: 7pts
  
  Opinions, Critics and Alternatives 
  
  Grade: 10pts


>What was the software process you chose at the start of the project (test-driven, The waterfall model, Incremental development and delivery, Boehm's spiral model, Reuse-oriented software engineering, Software prototyping) and why did you choose it?

>While some of us do have professional backgrounds in software, for us Citra is a hobby project. With these types of OSS projects (no real organization backing us, no revenue/money), it's hard to enforce industry-standard engineering practices, we we often attract beginner/intermediate programmers (and a lot of students), and folks often have very inconsistent schedules as far as how frequently they contribute/how big of contributions they make. So what this kind of comes down to is it's difficult to force the project into any of the above molds - We're often happy just to get [quality] contributions. We place much higher importance on changes that are well-written, make tangible benefits to the project, and adhere to our coding guidelines/standards than actually meeting any sort of product-oriented deadlines. I guess you could say this falls under the "incremental development and delivery" model, as we are constantly working on new features, and when these features are ready, they are merged and become immediately available to users in the form of our nightly builds. Something like waterfall would not work at all for this type of project, and is really only viable for [commercial] products with well-defined requirements. Test-driven development is good for certain parts of emulators - for example CPU emulation. It's easy to write fuzz tests that test every valid permutation of each CPU instruction on real HW, and then verify that our software implementation behaves in the same way (and we do stuff like this). But for reasons that I described above (lack of professional/experienced developers, lack of time/consistent schedule of developers, etc.) it's not always a good return-on-investment to enforce up-front unit tests for every line of code (as classic test driven development advocates for). Often, if something clearly works well and is a tangible improvement to the project, we'd rather get it merged (and move the project forward) rather than enforcing so much coding bureaucracy that we scare folks away and lose the work. Furthermore, TDD has a lot of value in massive software projects with huge feature sets/user bases and minimizing regressions is critical - For us if something breaks, we can simply just revert the change. There are minimal stakeholders that we need to worry about. I would say we've basically landed with our own model of OSS development that works well for our specific situation, and luckily we have a core set of really talented developers that mentor newcomers and ensure that only quality changes get merged without much real regression. We also rely a lot on automated systems for building cross-platform, verifying/fixing code style, etc. to ensure junk doesn't get merged. I would guess our system is pretty similar to other hobby OSS projects of similar size, although we do have a reputation among our community for having a very quality, well-written source base with good procedures, often at the expense of having changes take a bit longer to get accepted.

>Did you (the developers) regretted or had any second thoughts about the software process you chose? If yes, why?

>I think this is mostly answered above -- In the sense that we have the ability to have a very organic/flexible development process, we adapt as we find improvements, so there is no reason to regret earlier decisions. On the contrary, I would say we felt "overly disciplined" with our development process early on (when the project was much less significant), with regards to a very high bar for contributions/strict process -- But this has actually paid off hugely. By having most of our core codebase done "correctly" the first time around, we've avoided issues that plague other similar projects (hacks that are critical for the emulator to work, prioritizing hacks that improve speed instead of accuracy, introducing hard to find bugs by prioritizing fast but untested progress over accurate tested code, etc.

>Hope that helps... Let me know if you have any other questions.

>bunnei
