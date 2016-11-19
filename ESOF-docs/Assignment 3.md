**Introduction to Software Architecture and the 4+1 Architectural View Model;**

Architectural design is concerned with understanding how a system should be organized and designing the overall structure of that system. It is the critical link between design and requirements engineering, as it identifies the main structural components in a system and the relationships between them. The output of the architectural design process is an architectural model that describes how the system is organized as a set of communicating components.
As Bosch said “ Software architecture is important because it affects the performance, robustness, distributability, and maintainability of a system ”.  ( daqui a pouco já completo a introdução )

**Architectural patterns** - todos

An architectural pattern is a good reusable solution to a regular problem within a specific context.

We have found that the existence of some architecture patterns on their code, such as Layered Architecture. They emulate the audio in one package and the video in other, which are the lower level layers. Then there is a package that uses those layers, asking services from the lower level layers.

They also have confirmed to be using an ARM CPU emulator (as a starter) and things like IO, hashing, memory management from others open source projects. This parts of the code are easily adapted and can be reused for every kind of emulator, since it is a recurring problem. //não sei se se pode considerar isto um padrão visto q nao foram eles a "inventar o codigo" nem q nome se daria a este suposto padrão. help!

//possivelmente o model view controller tbm é aplicado visto q tem q lidar com inputs de utilizadores e o render tem q se sujeitar a isso... fiquem livres de falar de outros padrões mesmo q nao sejam utilizados aqui e digam pq deveriam ser ou pq nao faz sentido serem usados



**Logical View** - Rui Oliveira
>Grade: 4pts

Development View
>Grade: 4pts

**Deployment View**

The deployment view leans over the hardware requirements of the system. It maps artifacts to the hardware that uses them. It also models a system's logical elements, their physical location, and how they communicate. It is often used to create a rough sketch of the physical layout of a system early in the development lifecycle. The following diagram is what we consider it would be the development view for CITRA.

![alt tag](http://icecream.me/uploads/6ddb59eff0ed22cbfcf68e6af0be7841.png)

CITRA is an emulator and debugger for nintendo 3DS, therefore it is requires a PC to run it. The pc must be 64bits, windows 7 or higher, Linux or Mac OS X and must have Opengl 3.3 or higher. The other important thing one needs to use CITRA is a ROM file which contains a (non-multiplayer) game. This ROM file is used for playing or debugging purposes.

**Process View** - Guilherme Amaro
>Grade: 4 pts

**Group:**

 -[Guilherme Amaro](https://github.com/PORShoterxx)

 -[José Francisco Gomes](https://github.com/teresa-Guilherme/)

 -[Pedro Ferreira](https://github.com/pedrof81)

-[Rui Miguel Oliveira](https://github.com/ruimoliveira)
