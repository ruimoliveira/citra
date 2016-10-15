
**Brief description of the project**

As described in the README.md file, Citra is an open-source, passion-driven Nintendo 3DS emulator/debugger written in C++ is written so builds can be actively maintained for Windows, Linux and OS X. At this time, Citra is able to boot many commercial games, most of which do not run to a playable state yet, but are being worked on every day to advance the project forward.


**Development Process**

>Citra is being developed as a hobby for several programmers and their work schedule on this Open Source Software Project is not very consistent. They are not supported by any company, therefore they don't have a deadline to implement features. Citra has a team of experiences developers that help (begginer/intermediate level) new contributors with the standard level of code that is to be commited. They take a while to accept pull requests, so that they are certain that the pull has the quality they require, in order to avoid bugs or setbacks.
  >Since the contribution frequency is inconsistent, they can't use any industrial-standard engineering process. They "are constantly working on new features" (as said by one of the project leaders) so it would be considered an Incremental development process. However, as they don´t have any kind of deadlines and they only merge when they are sure the feature is operating correctly, we think they are also using a Slow programming process.


**Opinions, Critics and Alternatives**

- Due to how they work, the Incremental Development and Deployment process is the most reliable, if not the only plausible, development process.
- Test-driven development is an alternative to the above. However, this is ill-advised. As with an emulator's nature, it's required to work with multiple games, each with it's own code quirks, while optimizing for playable perfomance. This would mean an excessive amount of tests, and very slow progress towards an acceptable result.

- Being a hobby project, there's no fixed planning in development. Most releases tend to be random bug fixes, small new features, etc.
- There is a guideline on code style. This improves feature recognition by other developers and smoothens development times.
- Since it's an open project, it's bound to have disparities in coding methodology. This issue has been actively tackled, just as explained above.
- Having a stricter group of developers would potentialy hurt development times, and not necessarily improve code quality, since pull requests are already verified individually before merge.

- As a result of its early development stage, the interface is not very user-friendly and there's a large ammount of bugs.
- Part of this project requires specific knowledge about console hardware, emulation, among other areas. This significantly decreases the quantity of code submissions.
