
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

  Since Citra is not supported by any company they don't have a deadline to implement features, so how does the team decide on whether to implement a new feature or no? 

  For requirements elicitation we informal interviewed the developers as we also discovered their requirements in their project site https://citra-emu.org/. 
  As said by one of the developers in our informal interview, requeriments are mostly fixing bugs and implementing new features.With an emulator, you already have a "spec" to follow - the original console that you're trying to emulate, so new "features" generally means emulating a part of that console that you do not already implement (or at times, implement incompletely). User requests commonly aren't related to emulation but rather usability features - For example, a user wouldn't request to implement 3DS fragment lighting (we already know to do that, it's part of the hardware!), but they might request to implement cheat code support or changes to the UI.These types of usability features tend to be a lower priority(as we still don't have the most important thing, the fully working emulation completed), so they aren't a big driving factor in the work that we do currently. This may change as the project becomes more mature. 
Lastly, they say optimization is another big area - lots of effort is spent identifying bottlenecks and rewriting things to improve speed. Emulation of modern video game systems requires both fast/efficient code and a fast computer.

  They implement features when they want or when the contributors have a feature that have the quality they require in order to avoid bugs or setbacks but their main focus right now is to fix bugs that stop games from booting and bugs that crashes the program when running,having a fully working emulation completed.Issues about specific games not booting are valid bugs, they are currently not interested in them unless there are several games which fail with the same or similar messages. There are too many non-working games right now to file individual issues for every one of them.
In future they intend to implement features like cheat code support, improve speed of cut scenes and support for smartphones.
Given the circumstances of this project (hobby, volunteers, low amount of time that developers have to work and inconsistent frequency of commits, specific knowledge about console hardware, emulation, among other areas) the reality of the new features is contributors of Citra contribute what they like and not always what is ideal.

** Specific Requirements and Features ** 

  As stated above, a functional requirement specifies something the system should do (describes how a function should behave). For example: the box of a game must be able to contain the pieces of the game without losing them.
  On the other hand, a non-functional requirement describes how the system behaves (a constraint on the system behaviour).
For example: the box of a game must be made of leather.

//to be completed

**Use Cases**

These are the uses we could figure out for both the application.
![alt tag](http://i.imgur.com/deDgtE4.png)

**Domain Model**

  Domain model is a conceptual model of the domain that incorporates both behavior and data. Its purpose is to connect Use Case Model with Software Design Model. Since this emulator is such a simple concept, and the problem domain is rather small, there really isn't the need for real world classes. With this in mind we decided, that this would be the domain model for the project:
![alt tag](http://icecream.me/uploads/d3285a245af38b0a7e8def42c7fe5cb0.png)

