This security framework aims to represent the systems in IT with an architectural base, this is also based on 3 concepts, 
- **Isolation**: This concept involves creating secure environments where system components are separated to prevent unauthorized access or interference
- **Interaction**: This refers to the way system components communicate and work together, ensuring that these interactions are secure
- **Representation**: This is about how security relationships between system components are defined and represented to maintain a secure system
It focuses on viewpoints, which are:
- **System Viewpoint**: Describes the system of interest, i.e., the target of the security.
- **Security Viewpoint**: Describes the security goals and related aspects
- **Process Viewpoint**: Establishes a clear methodology to define the security of the system
This also remarks the structure to 

# Steps to model systems
The ordered process of modeling the system/entity of interest is to first ensure we follow an architecture based approach with the 3 mentioned viewpoints  
By doing that and following those viewpoints we are going to be able to **provide a systemic, comprehensive and potentially automated way to manage our target system**, while also being able to support scalability and modularity, to integrate newer technologies with ease and not be coupled to a specific implementation

## 1. Collect the information and requirements
This involves the process of getting all the data possible from **all the aspects(objective data of the system), perspectives(the data from aspects but in multiple different angles) AND with their respective priority according to our concerns**, the data must also focus on **objectives and policies**
Organization policies establish the main guidelines of the resulting security. If there are no available business policies, security objectives could be defined based on a rationale, but hopefully related to the business activity

## 2. Defining the system representation
> Cohesion and Coupling are **key concepts** when **designing the components and also analyzing them**

This is creating the **views** from which we are going to be able to express the system and understand it, these representations can be from any kind of modeling like UML, SysML, whole-parts tree, interaction diagrams or other things while we ensure it fits with out methodology
	The *whole-parts tree* is particularly useful and applicable for the majority of systems, this tree can be done using a bottom-up or top-down approach, going from general to specific or vice versa, and the things to consider when doing it is to prevent putting components **external to the boundaries of the system**, this also requires a good delimiter of the system, in this example the Cup-Package System is **focusing** on the cups and the elements that are **inherent and internal** to the cups and the objectives to be accomplished according to those concerns  
		This could be interpreted as the process of **lexers and parsers**, where we define the rules that will **give sense** to an entity, and with the Parse Tree we are able to **identify all the components segmented and divided with clear boundaries between the rules and their domain**, and at the bottom the details of the components
- It is also useful to try to place all the details at **the leaf nodes of the tree or lower nodes**, while having the upper nodes being more straight-forward, simpler and free from coupling matters with the implementation details, like implementing some sort of **abstraction to the upper nodes**, making these upper nodes just guides that describe the characteristics of the implementation details, but this should be done carefully and depending if the current system allows it
- IT ALSO is useful, **when creating and designing the representation of the system as a whole-parts tree**, to be able to be constructing the tree **progressively** AND when there are new things added to the tree(because we WON'T know all the components at start), then **MERGE  or SEPARATE** components to be able to ensure **cohesion and coupling**
	Like a **B+ Tree in data structures**
![[WholePartsTreeAndInteractionDiagrams.png]]
Once we have a system representation, we need one or more (direct) security objectives to reflect our concerns about the security of the system components. A direct objective is basically a way for specifying what we want about security in the system. Then, we define the following security objective: We want to prevent the cups from being broken or lost while transported to their destination  


> This way we are starting to **structure and order** the system to be developed and thus when we are making this ease of development, we acquire **benefits naturally** that lets us work with the components much more easily because we are essentially working with a good base, whereas if we skipped this approach we could run into **a lot of extra steps just to achieve the same result**, and we still would end up doing the same thing  
> With this division, we are able to then **associate the objectives and concerns to the individual components**, and we acquire also a clear boundary between the components linked with their **objectives and concerns** AND also other external systems interacted with 

## 3. Define High-level, Propagated Direct and Indirect Objectives
All these objectives are meant to address the concerns of the project while also fitting into each component of the project
- **High-Level Security Objectives**: These are initially derived from organizational policies and goals, and they guide the security for the entire system throughout its lifecycle
- **Propagated Direct Objectives**: These are more specific objectives that stem from the high-level ones, applied to particular components of the system that are relevant to the security goals.
	They are like getting the declared objectives giving focus to specific parts of the project  
The actual purpose of this is to, based on the **whole-parts tree** AND the **interaction diagrams**, then link to **each component with each objective**, and thus be able to justify and reason **with much more confidence and clarity**
- **Indirect Security Objectives**: These are the objectives that must be addressed also when we want to meet the declared objectives, like implicit objectives, by securing other components that indirectly affect the main security goals, often identified through security relationships like isolation, interaction, and representation
	Examples of these indirect objectives are:
	- A box protecting (isolating) the physical integrity of a hard disk may need additional protection for its own integrity
	- A software handling (interacting) a confidential piece of information may need additional integrity controls for its own code, to avoid a misbehaviour that would reveal the information. 
	- A digital ID (representing) for a user authenticated into a system may need additional integrity controls for itself to avoid an unwanted modification


## 4. Defining Security Representation 
Propagating the initial security objectives to all related components of the system to support an integral and comprehensive security process.
## 5. Identifying and Assessing Risks
Using the security representation to guide a risk assessment process, identifying potential risks to the system.
## 6. Establishing Security Requirements
Deriving security requirements from the risk assessment to mitigate selected risks.
## 7. Defining and Implementing Security Controls
Implementing security controls to enforce the established security requirements and achieve the security objectives.

This methodology is supported by an architecture-based approach with three viewpoints: system, security goals, and security process, aiming to provide a systemic, comprehensive, and potentially automated way to manage the security life cycle of IT systems and cybersecurity. The process supports scalability and modularity, allowing for integration with existing security solutions and standards.






