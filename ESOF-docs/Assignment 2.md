
**Requirements**

Before starting a project, it's essential that a team studies its costumers and user needs, so it can have a clear goal and understanding of a solution's required properties.
Software ystem requirements describe what a system should do, the services it provides and its operation constraints. Some of the problems that arise during the requirements engineering process are due to not separating these different description levels properly.

They are divided into two categories: user requirements and system requirements.
User requirements are statements of what the system's services are expected to provide it's users and the constraints under which it must operate.
System requirements are more detailed descriptions of the software system’s inner workings. In this project, the only system requirements are OpenGL 3.3 and a 64-bit operating system.

Software system requirements can also be classified as functional or non-functional requirements.
A system's functional requirements describe what the system should do.
Non-functional requirements constrict the workings of the system.

Requirement engineering processes may include four important high-level activities. assessment of utility to a specified business (feasibility study), discovering requirements (elicitation and analysis), standardization of the latter (specification), and verifying that these do indeed meet the customer's needs (validation).

For requirements elicitation, we interviewed the main Citra team developers, as well as obtained information from their website, https://citra-emu.org/. 
As said by one of the main developers, the requirements are mostly fixing bugs and implementing new features.
Since Citra is not supported by any company, they do not have a deadline to implement features. So how does the team decide on whether or not to implement a new feature? 

With an emulator, they already have a "spec" to follow - the original console that they're trying to emulate, so new "features" generally mean emulating part of that console that had not already been implemented (or at times, implemented partialy). User requests often do not relate to emulation, but rather usability features. For example, a user won't request to implement the 3DS's fragment lighting (they already know how to do that, it's part of the hardware), but they might request to implement cheat code support or changes to the user interface. These types of usability features tend to be in a lower priority (as they still don't have the most important thing, the fully functional emulation, completed), so they aren't a big driving factor in their current work. According to the main developer, this may change as the project matures. 
Lastly, they say optimization is another big area - a lot of effort is spent identifying bottlenecks and rewriting code to improve speed. Emulation of modern video game consoles requires both fast/efficient code and a high-end computer.

They implement features whenever desired, or when the contributors' meets their quality standard, in order to avoid bugs or setbacks. However, their main focus right now is having a fully functional emulation, to fix bugs that stop games from booting, or that crash the program. Issues about specific games not booting are valid bugs, but are not prioritized unless there are several games which suffer from the same issue. There are still too many non-working games to file individual issues for each one individualy.
In future they intend to implement multiple features, such as cheat code support, improved cut-scene emulation speed and mobile platform support.
Given the circumstances of this project (hobby, volunteers, low amount of time that developers have to work with and inconsistent frequency of commits, specific knowledge about console hardware, emulation, among other areas), the reality of adding new features sums to developers contributing to Citra on what they like, and not always in an ideal manner.

Citra works on all three major desktop operating systems and is actively tested and supported on multiple 64-bit versions of Windows (7 and above), Linux and Mac OS X. While other platforms may work, they aren't tested by developers. In a far future, mobile platforms may be targeted as well. They have no plans to support 32-bit operating system officially.
At this point, Citra cannot emulate most commercial games at full speed, even if your computer can run the most demanding of PC games just fine.
The only hard requirements for the official version of Citra is a graphics card that supports at least OpenGL 3.3 and a 64-bit operating system, but a processor with the highest possible performance per core is highly recommended.




**Specific Requirements and Features** 

As previously mentioned, software system requirements are often divided into functional and non-functional.
A system's functional requirements describe what the system should do. With Citra, they include having the emulator running smoothly, with no crashes, while performing as accurately as possible to the physical console. Another one is Hardware Specifics emulation - as the purpose of the emulator is to emulate the hardware's functionality.

Non-functional requirements constrict the workings of the system. In Citra's case, they manifest as code standards and matching a design process specified by the main development team (i.e.: avoiding "speedhacks", since these make the game faster at the cost of potential bugs, as many other emulators do).




**Use Cases**

An use case diagram represents the user's interactions with the system, identifying the different users of the system and different use cases. An use case lists the action(s) for a user to achieve a certain goal. This should be as simple as possible, capturing all requirements from a user's perspective in order to facilitate understanding.

These are the simplified uses cases for Citra Emulator:
![alt tag](http://i.imgur.com/deDgtE4.png)

| Actor(s) | Use Case(s) | Brief Explanation |
| --- | --- | --- | 
| Indie Developer & Gamer | Emulate Game | This is the core feature of an emulator. |
| Indie Developer | Debug | A developer should be able to debug his game on Citra. |
| Gamer | Save Game & Load Game | Although some (if not all) games already come with a save/load game feature, some emulators allow users to save the state of the emulation. |




**Domain Model**

Domain model is a conceptual model of the domain that incorporates both behavior and data. Its purpose is to connect the Use Case Model with the Software Design Model. Since this emulator is such a simple concept, and the problem domain is rather small, there is no need for real world classes. With this in mind, we decided that this would be the domain model for the project:

![alt tag](http://icecream.me/uploads/d3285a245af38b0a7e8def42c7fe5cb0.png)




**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

-[Rui Miguel Oliveira](https://github.com/ruimoliveira)
