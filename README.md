# Glossary of Object Capabilities (OCaps) Terms

## Amplification
The process of increasing the authority of a capability, often through composition with other capabilities.

## Attenuation
The process of limiting or reducing the authority of a capability when it's passed to another entity.

## Attenuator
An object that reduces or limits the capabilities of another object, often used to implement the principle of least privilege.

## Authority
The set of actions that an object is permitted to perform within a system.

## Brand
A marker used to differentiate or identify specific capabilities or objects, ensuring that only authorized entities can use them.

## Capability
A communicable, unforgeable token of authority that represents the right to perform specific actions or access specific resources.

## Capability Discipline
A practice or approach to designing systems that strictly adhere to the principles of capabilities, such as POLA (Principle of Least Authority).

## Caretaker
An object that manages access to another object, often used in revocation patterns.

## Confinement
The practice of restricting an object's access to only the capabilities it needs to perform its intended function.

## Designation
The ability to refer to or name an object within a capability system.

## Discretionary Access Control
A security model where an object can grant its capabilities to other objects at its own discretion.

## Encapsulation
The bundling of data and the methods that operate on that data within a single unit or object.

## Endowment
The initial set of capabilities that an object is given when it is created, which defines its authority.

## Facet
A limited view or interface of an object that exposes only a subset of its capabilities.

## Factory
An object or function responsible for creating instances of other objects, often used to control the distribution of capabilities.

## Forwarder
An object that passes along invocations to another object, often used in revocation patterns.

## Granting
The act of giving a capability to another entity.

## Immutability
The property of an object whose state cannot be changed after its creation, often used to enhance security and ensure predictable behavior.

## Invulnerability
The property of an object that cannot be compromised or manipulated by unauthorized entities, often achieved through strict encapsulation and unforgeable references.

## Least Privilege
The principle of giving an object only the minimum capabilities necessary to perform its function.

## Membrane
A boundary in a capability system that mediates and potentially transforms object references as they pass through it.

## Object
A self-contained entity that combines state and behavior, typically used as the basic unit of programming in object-oriented systems.

## Occlusion
The hiding or masking of certain capabilities when an object is passed to another context.

## Power Box
A user interface pattern in capability systems for securely granting capabilities to applications.

## Principle of Least Authority (POLA)
A security principle stating that every module must be able to access only the information and resources necessary for its legitimate purpose.

## Proxy
An object that stands in for another object, potentially adding behavior like revocation or attenuation.

## Revocable
A capability that can be invalidated or removed after it has been granted.

## Revocation
The act of removing or invalidating a previously granted capability.

## Rights Amplification
The process by which the combination of two or more capabilities results in greater authority than the sum of the individual capabilities.

## Sealer/Unsealer Pair
A mechanism for creating encrypted capabilities that can only be used by authorized parties.

## Transitivity
The property where if A can designate B, and B can designate C, then A can indirectly designate C through B.

## Unforgeable Reference
A reference or pointer to an object that cannot be guessed or fabricated, ensuring that possession of the reference implies the right to use it.

## Virtualization
The creation of a simulated environment within a capability system, often used for sandboxing or testing.

## Waiver
The voluntary relinquishment of a capability by an object.

## Wrapper
An object that encapsulates another object, potentially modifying its behavior or restricting its capabilities.
