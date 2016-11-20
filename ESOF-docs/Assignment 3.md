#Software Architecture and the 4+1 Architectural View Model

## Introduction 

Architectural design is concerned with understanding how a system should be organized and designing the overall structure of that system. It is the critical link between design and requirements engineering, as it identifies the main structural components in a system and the relationships between them. The output of the architectural design process is an architectural model that describes how the system is organized as a set of communicating components.
As Bosch said “ Software architecture is important because it affects the performance, robustness, distributability, and maintainability of a system ”.

The software architecture can serve firstly as a design plan for the negotiation of system requirements, and secondly as a means of structuring discussions with clients, developers, and managers.
Because of the close relationship between non-functional requirements and software architecture, the particular architectural style and structure that we choose for a system should depend on the non-functional system requirements

It is impossible to represent all relevant information about a system’s architecture in a single architectural model, as each model only shows one view or perspective of the system. There are different opinions as to what views are required. The well-known Krutchen’s 4+1 view model of software architecture, suggests that there should be four fundamental architectural views, which are related using use cases or scenarios. 
The views that he suggests are: Logical View, Development View, Deployment View and Process View.

The architecture of a software system may be based on a particular architectural pattern or style. An architectural pattern is a description of a system organization. Architectural patterns are a means of reusing knowledge about generic system architectures. They describe the architecture, explain when it may be used, and discuss its advantages and disadvantages.
Commonly used architectural patterns include: Model-View-Controller, Layered Architecture, Repository, Client–server, and Pipe and Filter.

We have found some architecture patterns on their code, such as Layered Architecture.The notions of separation and independence are fundamental to architectural design because they allow changes to be localized.The layered architecture pattern is a way of achieving separation and independence. They emulate the audio in one package and the video in other, which are the lower level layers. Then there is a package that uses those layers to ask services from the lower level layers.The system functionality is organized into separate layers, and each layer only relies on the facilities and services offered by the layer immediately beneath it.
This pattern has the advantage of allowing replacement of entire layers so long as the interface is maintained, but in practice providing a clean separation between layers is often difficult. 

They also have confirmed to be using an ARM CPU emulator (as a starter) and processes like hashing, memory management and IO from others open source projects. This parts of the code are easily adapted and can be reused for every kind of emulator since it is a recurring problem.Generic models of application systems architectures help us understand the operation of applications, compare applications of the same type, validate application system designs, and assess large-scale components for reuse.

//não sei se se pode considerar isto um padrão visto q nao foram eles a "inventar o codigo" nem q nome se daria a este suposto padrão. help!

Model–view–controller can be used too since rendering have to deal with user inputs .As with other software architectures, model view controller expresses the "core of the solution" to a problem while allowing it to be adapted for each system.It divides a given software application into three interconnected parts, so as to separate internal representations of information from the ways that information is presented to or accepted from the user.

//possivelmente o model view controller tbm é aplicado visto q tem q lidar com inputs de utilizadores e o render tem q se sujeitar a isso... fiquem livres de falar de outros padrões mesmo q nao sejam utilizados aqui e digam pq deveriam ser ou pq nao faz sentido serem usados

## Logical View - Rui Oliveira
>Grade: 4pts

## Development View

The development view (also known as implementation view) focuses on decomposing software into components (program libraries, or subsystems) that are then developed by a small number of developers. These components are split into a hierarchy of layers, with the higher layers depending from the lower layers. The following component diagram depicts Citra's layer hierarchy and dependencies:

![alt tag](https://s11.postimg.org/wghfquigz/development_view.png)

The game interacts with the emulator through an interface made available by the emulator. The emulator deals with everything else. The user, in the game settings, defines which modules they want to be loaded. After that, the emulator asks the module loader for those modules, using an interface made available by the module loader. Each of these modules contains a feature, meaning that any features that are added to the game do not put in danger the program functionality. The module loader then makes those modules available to the emulator.

During the game, the emulator communicates with its core to send to the game component the information regarding the world, entities, configurations, audio, etc.

In our opinion, this is an optimal approach since, as said, new modules can be added without compromising the entire system. This approach also allows each part of the system to be easily improved.

## Deployment View

The deployment view leans over the hardware requirements of the system. It maps artifacts to the hardware that uses them. It also models a system's logical elements, their physical location, and how they communicate. It is often used to create a rough sketch of the physical layout of a system early in the development lifecycle. The following diagram is what we consider it would be the development view for CITRA.

![alt tag](http://icecream.me/uploads/6ddb59eff0ed22cbfcf68e6af0be7841.png)

CITRA is an emulator and debugger for nintendo 3DS, therefore it is requires a PC to run it. The pc must be 64bits, windows 7 or higher, Linux or Mac OS X and must have Opengl 3.3 or higher. The other important thing one needs to use CITRA is a ROM file which contains a (non-multiplayer) game. This ROM file is used for playing or debugging purposes.

## Process View - Guilherme Amaro
>Grade: 4 pts


**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

-[Rui Miguel Oliveira](https://github.com/ruimoliveira)
