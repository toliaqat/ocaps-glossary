# Glossary of Object Capabilities (OCaps) Terms

## Amplification
Amplification in the context of object capabilities refers to the process of increasing or enhancing the authority of a capability. This often involves composing multiple capabilities to enable broader access or more powerful operations. For example, a basic capability might allow read access to a file, but amplification might combine it with another capability to enable editing. This process must be managed carefully to avoid inadvertently granting excessive privileges that could compromise security.

## Attenuation
Attenuation is the practice of deliberately limiting the authority of a capability before passing it to another entity. It is a crucial concept for enforcing security principles such as the Principle of Least Authority (POLA), which mandates that entities should only have the minimum necessary access to perform their functions. Attenuation helps in creating safer interfaces by reducing the risk of misuse or unintended actions by the recipient of a capability.

## Attenuator
An attenuator is an object or mechanism that reduces the capabilities of another object, often by acting as a filter that restricts what the original capability can do. This is typically employed to enforce security policies like least privilege, ensuring that an entity can only perform actions explicitly permitted by the attenuated capability. An attenuator can transform a full access capability into a more limited one, such as converting a read-write capability to a read-only one.

## Authority
Authority in object capability systems refers to the set of actions that an object is permitted to perform within a system. This concept is central to managing access and permissions, as each object operates within the boundaries of its granted authority. Authority defines the scope of what an object can do, such as reading or modifying data, and is a key consideration in designing secure systems.

## Brand
A brand is a marker or tag used in object capability systems to differentiate or identify specific capabilities or objects. It ensures that only authorized entities can utilize these capabilities, acting as a form of access control. Brands help prevent unauthorized access by serving as a unique identifier that entities must recognize and validate before using a capability.

## Capability
A capability is a communicable and unforgeable token of authority that represents the right to perform specific actions or access particular resources within a system. Unlike traditional access control mechanisms, capabilities are directly associated with objects and are granted to entities as tokens, enabling more flexible and fine-grained access control. The unforgeability ensures that capabilities cannot be duplicated or tampered with, maintaining the integrity of access rights.

## Caretaker
A caretaker is an object that manages access to another object, often used in revocation patterns. It acts as a mediator or guard, controlling which entities can interact with the protected object and under what conditions. Caretakers play a vital role in dynamic access control scenarios, allowing for the adjustment or revocation of access rights as needed, without directly exposing the target object.

## Confinement
Confinement is the practice of restricting an object's access to only the capabilities it needs to perform its intended function. By limiting access to unnecessary capabilities, confinement helps prevent security vulnerabilities and reduces the potential impact of a security breach. This principle aligns with the broader concept of least privilege, where the objective is to minimize the attack surface by only granting essential permissions.

## Designation
Designation refers to the ability to refer to or name an object within a capability system. It involves specifying which objects are subject to particular capabilities, effectively determining the scope and target of those capabilities. Designation is a fundamental part of capability-based access control, as it defines the relationship between capabilities and the objects they govern.

## Discretionary Access Control
Discretionary Access Control (DAC) is a security model where an object can grant its capabilities to other objects at its discretion. This model contrasts with mandatory access control, where permissions are centrally enforced. In DAC, individual objects have the authority to delegate capabilities, allowing for flexible and decentralized access management. However, this flexibility can also introduce security challenges if not managed properly.

## Endowment
Endowment refers to the initial set of capabilities that an object is given when it is created, which defines its authority within a system. These initial capabilities determine what actions the object can perform and what resources it can access. Carefully designing endowments is crucial for maintaining security and ensuring that objects only possess the necessary capabilities to fulfill their roles.

## Facet
A facet is a limited view or interface of an object that exposes only a subset of its capabilities. By providing a restricted interface, a facet allows specific interactions with an object while concealing other capabilities. This approach is useful for adhering to the principle of least privilege, as it ensures that clients only have access to the capabilities they require.

## Forwarder
A forwarder is an object that passes along invocations to another object, often used in revocation patterns. Forwarders act as intermediaries, relaying messages or actions from one object to another while maintaining control over the interaction. This design pattern is useful for managing access and revoking capabilities, as forwarders can be adjusted or disabled without affecting the original objects.

## Granting
Granting is the act of giving a capability to another entity, effectively delegating authority to perform certain actions or access specific resources. This process is central to capability-based security, enabling flexible and decentralized access control. When granting capabilities, careful consideration must be given to the potential implications and security risks associated with delegating authority.

## Immutability
Immutability is the property of an object whose state cannot be changed after its creation. This characteristic is often used to enhance security and ensure predictable behavior, as immutable objects are resistant to unintended modifications. By designing objects to be immutable, developers can reduce the complexity of managing state changes and improve the reliability of their systems.

## Invulnerability
Invulnerability is the property of an object that cannot be compromised or manipulated by unauthorized entities. This is often achieved through strict encapsulation, unforgeable references, and robust access controls. Invulnerable objects are designed to resist attacks and unauthorized access, contributing to the overall security and integrity of the system.

## Least Privilege
The principle of least privilege dictates that an object should only be given the minimum capabilities necessary to perform its function. This security principle minimizes the risk of abuse or accidental misuse by limiting the potential impact of a security breach. Implementing least privilege requires careful analysis of each object's requirements and the diligent management of capabilities to ensure compliance.

## Membrane
A membrane is a boundary in a capability system that mediates and potentially transforms object references as they pass through it. Membranes can intercept, modify, or restrict interactions between objects, providing an additional layer of security and control. This design pattern is useful for enforcing access policies, monitoring communications, and ensuring that objects adhere to predefined constraints.

## Object
An object is a self-contained entity that combines state and behavior, typically used as the basic unit of programming in object-oriented systems. Objects encapsulate data and provide methods for interacting with that data, promoting modularity, and reuse. In capability-based systems, objects are often associated with specific capabilities, defining what actions they can perform and what resources they can access.

## Occlusion
Occlusion is the hiding or masking of certain capabilities when an object is passed to another context. This practice is used to prevent unauthorized access or manipulation of sensitive capabilities, ensuring that only intended interactions occur. Occlusion can be implemented through techniques such as wrapping or attenuation, providing a controlled interface for external interactions.

## Power Box
A power box is a user interface pattern in capability systems for securely granting capabilities to applications. It acts as an intermediary between users and applications, allowing users to review and approve capability requests before they are granted. Power boxes enhance security by providing transparency and control over the distribution of capabilities, ensuring that users are aware of the permissions they are granting.

## Principle of Least Authority (POLA)
The Principle of Least Authority (POLA) is a security principle stating that every module must be able to access only the information and resources necessary for its legitimate purpose. POLA minimizes security risks by reducing the potential impact of a breach, limiting the access and authority granted to each component. This principle guides the design of capability-based systems, promoting the careful management and delegation of capabilities.

## Proxy
A proxy is an object that stands in for another object, potentially adding behavior like revocation or attenuation. Proxies can intercept and modify interactions between clients and the target object, providing an additional layer of control and security. This design pattern is useful for implementing access controls, monitoring interactions, and managing capabilities dynamically.

## Revocable
A capability is considered revocable if it can be invalidated or removed after it has been granted. Revocable capabilities provide flexibility in managing access, allowing for the adjustment or termination of permissions as needed. This property is essential for maintaining security in dynamic environments, where access requirements may change over time.

## Revocation
Revocation is the act of removing or invalidating a previously granted capability. This process is crucial for maintaining security, as it allows for the termination of access when it is no longer needed or when a security risk is identified. Revocation can be implemented through various mechanisms, such as revocation lists, forwarders, or caretakers, depending on the system's requirements.

## Rights Amplification
Rights amplification is the process by which the combination of two or more capabilities results in greater authority than the sum of the individual capabilities. This concept allows for the dynamic creation of new capabilities by composing existing ones, enabling more complex interactions and access patterns. Rights amplification must be carefully managed to avoid unintentional privilege escalation or security breaches.

## Sealer/Unsealer Pair
A sealer/unsealer pair is a mechanism for creating encrypted capabilities that can only be used by authorized parties. Sealers encrypt capabilities, while unsealers decrypt them, ensuring that only entities with the appropriate unsealer can access the protected capabilities. This approach enhances security by controlling access to sensitive capabilities and preventing unauthorized use.

## Transitivity
Transitivity is the property where if A can designate B, and B can designate C, then A can indirectly designate C through B. This property allows for the delegation of capabilities and access rights across multiple entities, enabling more flexible and dynamic interactions. Transitivity must be carefully managed to prevent unauthorized access or privilege escalation, as it can introduce complex access patterns and dependencies.

## Unforgeable Reference
An unforgeable reference is a reference or pointer to an object that cannot be guessed or fabricated. This ensures that possession of the reference implies the right to use it, providing a secure means of granting access to capabilities. Unforgeable references are a cornerstone of capability-based security, as they prevent unauthorized entities from accessing protected objects.

## Virtualization
Virtualization is the creation of a simulated environment within a capability system, often used for sandboxing or testing. Virtualized environments provide isolated execution spaces where capabilities and interactions can be controlled and monitored, enhancing security and allowing for safe experimentation. This approach is useful for developing, testing, and deploying applications in a controlled manner, minimizing the risk of unintended side effects or security breaches.

## Waiver
A waiver is the voluntary relinquishment of a capability by an object. This action can be used to reduce an object's authority or to comply with security policies that require the limitation of access rights. Waivers provide a mechanism for dynamically adjusting capabilities, allowing objects to relinquish unnecessary or potentially risky permissions as needed.

## Wrapper
A wrapper is an object that encapsulates another object, potentially modifying its behavior or restricting its capabilities. Wrappers can provide additional functionality, enforce access controls, or transform interactions with the underlying object. This design pattern is useful for implementing security policies, managing capabilities, and creating flexible interfaces that adapt to changing requirements.
