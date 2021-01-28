# Architecture principles

* Clean code
    * Be consistent
    * Prefer meaningful names oer comments
    * Indentation and style
    * Keep method, classes, files small
    * Pure functions 
    * Refactor switch statements to classes
    * Don't pass booleans 
    * Don't pass null
    * Use the correct constructs
    * Command Query separation
    * Organize code by the actor it belongs to
    * Keep framework code distant
    * Tests should be fast, independent and repeatable
    * Refactor often
    * Use meaningful names
* Design principles
    * SOLID (**single responsibility, open–closed, Liskov substitution, interface segregation и dependency inversion**)
    * YAGNI (**You aren't gonna need it** с англ. — «Вам это не понадобится»)
    * KISS (**Keep It Simple, Silly** с англ. — «Держать его просто глупо»)
    * DRY (**Don't Repeat Yourself**)
    * Composition over inheritance
    * Program to interfaces, not to implementations
    * Design by Contract (DBC)
    * Separation of Concerns
    * Principle of Least Surprise
    * Law of Demeter
    * The Four Primary Object-Oriented Design Principles
    * Encapsulate what varies
    * The Hollywood Principle
    * All software is composition
    * Design patterns are complexity
    * Cross-cutting concerns
    * Principle of Least Resistance
    * Strive for loose coupling between objects that interact
* Design pattern 
    * Creation
    * Structural
    * Behavioural
* Architectural principles
    * **[Architecture characteristics](characteristics/description.md)**
        * Operational
            * **Availability** - how long a system will need to be available (if24/7, steps need to be in place to allow the 
            system to be up and running quickly in case of any failure)
            * **Continuity** - Disaster recovery capability
            * **Reliability/safety** - assess if the system needs to be failsafe, or if it is mission critical
            in a way that affects lives. If it fails, will it cost the company large sums of money?
            * **Robustness** - Ability to handle error and boundary conditions while running if the internet connection goes
            down or if there is a power outage or hardware failure.
            * **Scalability** - Ability for the system to perform and operate as the number of users or requests increases.
            * **Recoverability** - business continuity requirements (e.g., in case of a disaster, how quickly is the system 
            required to be on-line again?). This will affect the backup strategy and requirements for duplicated hardware.
            * **Performance** - include stress testing,peak analysis, analysis of the frequency of functions used,
            capacity required, and response times. Performance acceptance sometime requires an exercise of its own,
            taking months to complete.  
        * Structural
            * **Configurability** - ability for the end users to easily change aspects of the software is configuration
             (through usable interfaces)
            * **Extensibility** - how important it is to plug new pieces of functionality in
            * **Installability** - ease of system installation on all necessary platforms
            * **Leveragability/reuse** - ability to leverage common components across multiple products
            * **Localization** - Support for multiple languages on entry/query screens in data fields; 
            on reports; multibyte character requirements and units of measure or currencies
            * **Maintainability** - How easy it is to apply changes and enhance system?
            * **Portability** - does the system need to run on more that one platform?
            (For example, does the frontend need to run against Oracle as well as SAP DB?)
            * **Supportability** - what level of technical support is needed by the application? What level of logging
            and other facilities are required to debug errors in the system?
            * **Upgradeability** - ability to easily/quickly upgrade from a previous version of this
            application/solution to a newer version on servers and clients
        * Cross-Cutting
            * **Accessibility** - access to all your users, including those with disabilities like
            colorblindness or hearing loss
            * **Archivability** - will the data nees to be archived or deleted after a period of time? (For example, 
            customer accounts are to be deleted after three months or marked as obsolete and archived
            to a secondary database for future access)
            * **Authentication** - security requirements to ensure users are who they say they are
            * **Authorization** - security requirements to ensure users can access only certain functions within the
            application (by use case, system, webpage, business rule, field level, etc.)
            * **Legal** - what legislative constraints is the system operating in 
            (data protection, Sarbanes Oxley, GDPR, etc.)? What reservation rights does the company require?
            Any regulations regarding the way the application is to be build or deployed?
            * **Privacy** - ability to hide transactions from internal company employees (encrypted transactions
            so even DBAs and network architects cannot see them)
            * **Security** - does the data need to be encrypted in the database? Encrypted for network
            communication between internal systems? What type of authentication needs to be in place for remote user access? 
            * **Usability/achievability** - level of training requred for users to achieve their goals with
            the application/solution. Usability requirements need to be treated as seriously as 
            any other architectural issue.
        * Other
            * **Testability**
            * **Agility**
            * **Fault Tolerance**
            * **Elasticity**
            * **Deployability**
            * **Learnability**
            * [Modularity](characteristics/modularity.md) 
    * **Architecture decisions** (**the rules** for how a system should be constructed)
    * **Design principles** (**the guideline** rather than a hard-and-fast rule. Example: 
    leverage async messaging between services to increase performance)
* [CAP theorem](cap-theorem.md)

## Links

* [more links](links.md)
