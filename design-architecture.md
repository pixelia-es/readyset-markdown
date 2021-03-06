[Design](design) &gt; Architecture {#design-architecture}
---------------------------------------

### Release Information {#release-information}

Project:
:   PROJECTNAME

Internal Release Number:
:   X.Y.Z

Related Documents:
:   [Software Requirements Specification](srs)
:   [Design](design) &gt; [Security Worksheet](design-security)
:   [Glossary](glossary)
:   LINKS TO RELEVANT STANDARDS
:   LINKS TO OTHER DOCUMENTS

TODO: Answer the questions below to help you define your system
architecture. Some example text is provided.

### Overview {#overview}

What are the most important facts that a developer should know about this system architecture?
:   PARAGRAPH OR BULLETS

What software architecture style is being used?
:   Single-process desktop application (with plug-in extension modules).
:   Client-server with a custom thick-clients and server.
:   2-tier web application: webserver/app-server, database.
:   3-tier web application: webserver, app-server, database.
:   Single web service: app-server, database.
:   Network of web services.
:   Peer-to-peer with/without central server.
:   Pipe-and-filter.
:   Computing grid / distributed servers.

What are the ranked goals of this architecture?

:   1.  [Ease of integration](glossary-std#dg_easy_integration){.def}
    2.  [Extensibility](glossary-std#dg_extensibility){.def}
    3.  [Capacity matching](glossary-std#dg_cap_match){.def}

### Components {#components}

What are the components of this system?
:   The components of this system are clearly defined in this [UML Model
    with Component Diagram](LINK-TO-MODEL).
:   The components of this system are listed below by type:

:   - Presentation/UI Components
        -  [C-00: COMPONENTNAME](design-components#C-00)
    -  Application Logic Components
        -  [C-10: COMPONENTNAME](design-components#C-10)
    -  Data Storage Components
        -   [C-20: COMPONENTNAME](design-components#C-20)

### Deployment {#deployment}

How will the components be deployed to processes and machines?
:   The deployment of components to processes and machines is clearly
    defined in this [UML Model with Deployment Diagram](LINK-TO-MODEL).
:   The deployment of components to processes and machines is clearly
    defined below:

:   -   All-in-one server
        -   Tomcat process
            -   [C-00: Tomcat web server](design-components#C-00)
            -   [C-10: PROJECTNAME
                application](design-components#C-10)
        -   Database process
            -   [C-20: COMPONENTNAME](design-components#C-30)

:   The deployment of components to processes and machines is clearly
    defined below:

:   -   Load-balanced front-end servers
        -   [C-01: COMPONENTNAME](design-components#C-00)
    -   Back-end server
        -   JVM process
            -   [C-00: COMPONENTNAME](design-components#C-00)
            -   [C-10: COMPONENTNAME](design-components#C-10)
            -   [C-11: PLUG-IN COMPONENTNAME](design-components#C-11)
            -   [C-12: PLUG-IN COMPONENTNAME](design-components#C-12)
        -   Database process
            -   [C-20: COMPONENTNAME](design-components#C-30)

What aspects/resources of their environment are shared?
:   Everything is on one server so all machine resources are shared by
    all components.
:   All machines share the same bandwidth to the Internet. All machines
    access the same file server. So, if one component uses the resources
    heavily, other components may have to wait.

How are requests allocated to redundant or load-balanced servers?
:   We are not doing any load-balancing or redundancy for fail-over.
:   Load-balancing among front-end servers is handled by a load
    balancing device that we can make very few assumptions about.
    However, once a user session is established, the same front-end
    server will be used for all requests during that session.

What alternative deployment configurations are possible?
:   This is the only possible deployment.
:   The database could be moved to a different machine with a fairly
    simple change to a configuration file. Otherwise, nothing can be
    changed about the deployment.
:   We have the ability to move the database process to a
    separate machine. We have the ability to add more front-end servers.
    The application logic running on the application server cannot be
    split or load-balanced.

### Integration {#integration}

How will components be integrated? Specifically, how will they communicate?
:   All of our code uses direct procedure calls. The database is
    accessed through a driver.
:   Components within the same process use direct procedure call or
    standard Java events. Plug-ins are also accessed through a API of
    direct procedure calls and standard events. Communication with the
    database uses a JDBC driver. Communication between the front end-and
    back-end servers uses XML-RPC.

What architectural mechanisms are being used to ease future extensions or modifications?
:   We could change the database by switching drivers. Otherwise,
    extensions and modifications can only be done at the design level.
:   New front-end components could be added so long as they access the
    back-end the same way. New plug-in components can be dynamically
    loaded, so long as they satisfy the plug-in API. Otherwise, there is
    no ability to add or exchange components, because this architecture
    uses direct dependencies between its components rather than
    implicit invocation. Extensions and modifications can be made at the
    design-level, but deploying those changes requires recompilation
    and down-time.

### Architectural Scenarios {#architectural-scenarios}

TODO: Provide architecture scenarios that show how objects will
communicate across components, processes, and machines. Focus on
scenarios where the architecture itself is changing, e.g., system
startup, shutdown, adding or upgrading components, load balancing or
fail-over.

The following sequence diagrams give step-by-step descriptions of how
components communicate during some important usage scenarios:

-   [System startup](LINK-TO-DIAGRAM)
-   [System shutdown](LINK-TO-DIAGRAM)
-   [SCENARIO NAME](LINK-TO-DIAGRAM)

### Architecture Checklist {#architecture-checklist}

TODO: Evaluate your architecture with respect to each of your goals.

Ease of integration: Have mechanisms been provided for all needed types of integration?
:   Yes. In this system, all of the new components are designed to
    work together. And, the reused components are integrated via fairly
    simple interfaces.

Extensibility: What types of components can be added later and how?
:   See above.

Capacity matching: How has this architecture matched component resource needs to machines?
:   The database can be on a machine with RAID disks and a hot-swappable
    power supply, while the web front-end components can be on cheaper
    machines that could fail individually without causing
    system downtime. The front-end web servers and application server
    are both CPU-intensive, so they are deployed to different CPUs. The
    database is disk-intensive, so it can be deployed to the same
    machine as the CPU-intensive application server, with only moderate
    competition for resources.

Has the architecture been communicated to the development team and other stakeholders?
:   Yes, everyone understands. Feedback is welcome.
:   No, this is a risk that is noted in the [Risk
    Management](plan#risks) section.

TODO: Check for [words of
wisdom](http://readyset.tigris.org/words-of-wisdom/design-architecture.html)
and discuss ways to improve this template. Or, evaluate the ReadySET Pro
[professional architectural design
template](http://www.readysetpro.com/ "pro use case template and sample test plan").

Company Proprietary

Copyright © 2003-2004 Jason Robbins. All rights reserved. [License
terms](readyset-license.html). Retain this copyright statement whenever
this file is used as a template.


