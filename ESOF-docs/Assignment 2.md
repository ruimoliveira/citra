
**Requirements**

Before we can start building a project it is essential that the team study the costumers and user needs so the team can have a clear statement and understanding of required properties of a solution to solve the problem.
The requirements for a system are the descriptions of what the system should do, the services that it provides and the constraints on its operation.Some of the problems that arise during the requirements engineering process are a result of failing to make a clear separation between these different levels of description.
We can divide them in two: user requirements and system requirements.

User requirements are statements of what services of the system is expected to provide to system users and the constraints under which it must operate.
System requirements are more detailed descriptions of the software system’s functions, services, and operational constraints.

Software system requirements are often classified as functional requirements or non-functional requirements.
The functional requirements for a system describe what the system should do. 
Non-functional requirements, as the name suggests, are requirements that are not directly concerned with the specific services delivered by the system to its users.

Requirement engineering processes may include four important high-level activities. These focus on assessing if the system is useful to the business (feasibility study), discovering requirements (elicitation and analysis), converting these requirements into some standard form (specification), and checking that the requirements actually define the system that the customer wants (validation).

For requirements elicitation we informal interviewed the open-source developers as we also discovered their requirements in their project site https://citra-emu.org/. 
As said by one of the main developers in our informal interview, requeriments are mostly fixing bugs and implementing new features.
Since Citra is not supported by any company they don't have a deadline to implement features, so how does the team decide on whether to implement a new feature or no? 

With an emulator, they already have a "spec" to follow - the original console that they're trying to emulate, so new "features" generally means emulating a part of that console that you do not already implement (or at times, implement incompletely). User requests commonly aren't related to emulation but rather usability features - For example, a user wouldn't request to implement 3DS fragment lighting (they already know how to do that, it's part of the hardware!), but they might request to implement cheat code support or changes to the UI.These types of usability features tend to be a lower priority(as they still don't have the most important thing, the fully working emulation completed), so they aren't a big driving factor in the work that they do currently. As said by the main developer,this may change as the project becomes more mature. 
Lastly, they say optimization is another big area - lots of effort is spent identifying bottlenecks and rewriting things to improve speed. Emulation of modern video game systems requires both fast/efficient code and a fast computer.

They implement features when they want or when the contributors have a feature that have the quality they require in order to avoid bugs or setbacks but their main focus right now is having a fully working emulation completed,to fix bugs that stop games from booting and bugs that crashes the program when running.Issues about specific games not booting are valid bugs but they are currently not interested in them unless there are several games which fail with the same or similar messages. There are too many non-working games right now to file individual issues for every one of them.
In future they intend to implement features like cheat code support, improve speed of cut scenes and support for mobile platforms.
Given the circumstances of this project (hobby, volunteers, low amount of time that developers have to work and inconsistent frequency of commits, specific knowledge about console hardware, emulation, among other areas) the reality of the new features is, contributors of Citra contribute what they like and not always what is ideal.

Citra works on all three major desktop OSes and is actively tested and supported on various 64-bit version of Windows (7 and up), Linux and Mac OS X. Other platforms may work, but aren't tested by developers. In far future, mobile platforms may be targeted as well. They have no plans to support 32-bit operating system officially.
At this point, Citra is simply not fast enough to run most commercial games at full speed, even if your computer can run the most demanding of PC games just fine.
The only hard requirements for the official version of Citra is a graphics chip that supports at least OpenGL 3.3 and a 64-bit OS, but you definitely want a processor with the highest possible performance per core.



** Specific Requirements and Features ** 

As we said in the introduction,software system requirements are often classified as functional requirements or non-functional requirements.
The functional requirements for a system describe what the system should do.In this case a functional requerimet is having the emulator running smoothly and with no crashes.It will also include emulating the hardware spec - as the purpose of the emulator is to 
to duplicate the functionality of hardware.

Non-functional requirements, as the name suggests, are requirements that are not directly concerned with the specific services delivered by the system to its users.Their non-functional requirement are adhering standarts to their code and following their design process.



Specific Requirements and Features (Functional and Non-Functional requirements)
>Grade: 5pts

**Use Cases**

These are the uses we could figure out for both the application.
![alt tag](http://i.imgur.com/deDgtE4.png)

Domain Model
>Grade: 6 pts

