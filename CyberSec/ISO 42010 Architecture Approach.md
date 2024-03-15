Architecture is defined as the “fundamental concepts or properties related to an entity in its environment and governing principles for the realization and evolution of this entity and its related life cycle processes”

The ultimate goal of this approach to develop an architecture is to use an **ordered process** that is able to **classify information in a structured manner** about a complex project(like an application, enterprises or even city planning) to help us **identify and prioritize the goals and objectives that this project needs them to be solved, and thus GUIDE and know which solution to implement to the project**

A summarized exemplification of all these concepts brought to the real world in a scenario of a software engineering application would be this:
- **Stakeholder Concerns**: Identify key stakeholder concerns such as usability, performance, and security, which will help in defining the **goals and objectives, as well as knowing which architecture views and viewpoints to define**.
- **Architecture Views**: The views relates to the information that addresses the stakeholders concerns **in different domains**, for instance, a **usability view** might include user interface mockups, while a **security view** could detail encryption methods
	These are the basis for the architecture descriptions, which is the information to be classified and segmented.
	- **Architecture Viewpoints**: The viewpoints are the set of rules and conventions that state how views are built, interpreted and analyzed, with the purpose of **making easier the process of creating and understanding the views** us(like the *syntactic rules* of languages, which define how a language is built and understood, making this useful to break down very complex topics)
		An example could be that "As a security analyst, I need the system to be tolerant to failures", where the viewpoint 
- **Aspects and Perspectives**: *Aspects* refer to **objective type information** that **characterizes** the features of the entity of interest, letting us decompose a complex entity into smaller and more manageable parts, this covers the data of the entity, the activities it involves, and even location and people related to it, where in the context of a software application a **data aspect** could relate to the data model we have, and detailing how that data is **structured and interacted with**, like usage of relational databases in the application, there can also be **activity aspects**, which cover things like all the processes performed in the entity of interest, like in a web app this includes forms, user authentication, etc,. But the aspects could also cover wider things like location aspects, to cover infrastructure or people aspects, involving the interactions and hierarchy of the team 
	While the *Perspective* take an *aspect* of the entity and we **expand the aspect from different angles, in order to identify more concerns**, like viewing an application feature from the *perspective* of a developer or a stakeholder, where the developer has more technical concerns, while the stakeholder has more cost concerns
	These aspects can be then associated with different modes of perception such as **structural, behavioral, taxonomic, and connectivity**
	Examples of perspective include things such as: viability, cost, risk, usability, operability, legal compliance, ease of maintenance, market acceptability and share, ease of implementation.
- **Viewpoints and Models**: Utilize viewpoints to frame concerns and guide the creation of models that form the architecture views.

![[LayersOfTheConcepts.png]]

This approach helps in organizing the architecture description and ensures that the software application is designed to meet the stakeholders’ needs effectively.



The architecture is composed out of:
- **Entity of Interest**: This is a concept that covers a broad set of things like the systems in the architecture, and also things outside the boundaries of those systems such as the enterprises, and more.
- **Stakeholder Concerns**: Central to shaping the architecture.
- **Architecture Views**: Created based on stakeholders’ perspectives and concerns
- **Aspects and Perspectives**: New concepts introduced to align with modern practices.
- **Architecture Description**: This concepts is not the same as architecture, because this rather is the **representation or expression** of the architecture, which is a collection of artifacts like diagrams, tables, documents, etc. This architecture description helps communicate the design and characteristics of the entity of interest and the entity's properties(which the architecture is defined upon, which can be a system or enterprise)

![[ArchitectureComponentDiagram.png]]



# TODO
- Read the TFIA from Alejandro and the [Constructing an architecture-based cybersecurity solutionArchivo](https://mv1.mediacionvirtual.ucr.ac.cr/mod/resource/view.php?id=1967943)
