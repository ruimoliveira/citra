
**Brief description of the project**

  As described in the README.md file, Citra is an open-source, passion-driven Nintendo 3DS emulator/debugger written in C++ is written so builds can be actively maintained for Windows, Linux and OS X. At this time, Citra is able to boot many commercial games, most of which do not run to a playable state yet, but are being worked on every day to advance the project forward.


**Development Process**

  Citra is being developed as a hobby for several programmers and their work schedule on this Open Source Software Project is not very consistent. They are not supported by any company, therefore they don't have a deadline to implement features. Citra has a team of experiences developers that help (begginer/intermediate level) new contributors with the standard level of code that is to be commited. They take a while to accept pull requests, so that they are certain that the pull has the quality they require, in order to avoid bugs or setbacks.
  Since the contribution frequency is inconsistent, they can't use any industrial-standard engineering process. They "are constantly working on new features" (as said by one of the project leaders) so it would be considered an Incremental development process. However, as they don´t have any kind of deadlines and they only merge when they are sure the feature is operating correctly, we think they are also using a Slow programming process.
  They also use test driven development for certain parts of the emulator, but they fear that making the project only based on test driven, would scare the contributtors with the amounts of bureaucracy needed to implemented.

**Opinions, Critics and Alternatives**

  The use of incremental development and delivery as an engineer process, has its advantages, such as:
    * more interaction between the users/client and developers and consequently, early and requent feedback from the client;
    * low chance of project failure;
    * the most important requirement is tested thoroughly;
    
  This process provides a more closely and frequently interaction to meet the client's needs. On the other hand the main disadvantage, and the one we consider that might eventually occurr is code degradation. Using this process may degrade the quality of the code, as it is harder to refractor as more features are implemented.
  Given the circunstances of this project (hobby, volunteers, low amount of time that developers have to work and inconsistent frequency of commits,specific knowledge about console hardware, emulation, among other areas), we would say that Incremental Development and Deployment process is the most reliable, if not the only plausible development process.
  Test-driven development is an alternative to the above. However, this is ill-advised. As with an emulator's nature, it's required to work with multiple games, each with it's own code quirks, while optimizing for playable perfomance. This would mean an excessive amount of tests, and very slow progress towards an acceptable result.
  Since it's an open project, it's bound to have disparities in coding methodology. However, there is a guideline on code style. This improves feature recognition by other developers and smoothens development times.
  There is a guideline on code style. This improves feature recognition by other developers and smoothens development times. Having a stricter group of developers would potentialy hurt development times, and not necessarily improve code quality, since pull requests are already verified individually before merge.
