[Plan](plan) &gt; Resource Needs {#plan-resource-needs}
-------------------------------------

### Project Information {#project-information}


Project:
:   [PROJECTNAME](index)

Internal Release Number:
:   X.Y.Z

Project Time-frame:
:   STARTDATE - ENDDATE

Related Documents:
:   [Project proposal](proposal)
:   [Project plan](plan)
:   [QA plan](qa-plan)
:   [Software development methodology](sdm)
:   [Glossary](glossary)


**Process impact:** Based on the project plan and the worksheet below,
this project will need the following resources to meet its goals. If
fewer resources are available, the scope of the release should be
reconsidered or the process must be changed.

TODO: Fill in the information above and below. Add or remove rows as
needed. Use the worksheet to help identify and scope resource needs.
These rows are just examples. The total effort listed in this example
may not even match the totals given in other examples of related
documents.

### Human Resource Needs {#human-resource-needs}

| Need                                    | Resource                           | Amount   | Status   | Comments/Responsibilities |
|-----------------------------------------|------------------------------------|----------|----------|---------------------------|
| Project Management                      | PERSONNAME                         | 20 hours | Pending  |                           |
| Requirements                            | PERSONNAME                         | 20 hours | Assigned |                           |
| Requirements                            | PERSONNAME, PERSONNAME, PERSONNAME | 10 hours | Assigned |                           |
| Consultation with domain expert         | PERSONNAME                         | 2 hours  | Pending  |                           |
| Consultation with topic expert          | PERSONNAME                         | 4 hours  | Pending  |                           |
| Training on use of component/technology | PERSONNAME                         | 8 hours  | Assigned |                           |
| Overall Design                          | PERSONNAME, PERSONNAME, PERSONNAME | 20 hours | Assigned |                           |
| Detailed UI Design                      | PERSONNAME                         | 5 hours  | Pending  |                           |
| Detailed Database Design                | PERSONNAME                         | 5 hours  | Pending  |                           |
| Development                             | PERSONNAME, PERSONNAME, PERSONNAME | 40 hours | Assigned |                           |
| Development                             | PERSONNAME, PERSONNAME             | 80 hours | Assigned |                           |
| Development                             | PERSONNAME                         | 20 hours | Pending  |                           |
| Technical writing                       | PERSONNAME, PERSONNAME             | 10 hours | Assigned |                           |
| QA Planning                             | PERSONNAME                         | 10 hours | Assigned |                           |
| QA Testing                              | PERSONNAME, PERSONNAME, PERSONNAME | 40 hours | Assigned |                           |
| Release Engineering                     | PERSONNAME                         | 4 hours  | Assigned |                           |

### Capital Needs {#capital-needs}

<table>
    <colgroup>
        <col width="20%" />
        <col width="20%" />
        <col width="20%" />
        <col width="20%" />
        <col width="20%" />
    </colgroup>
    <thead>
        <tr class="header">
            <th>Need</th>
            <th>Resource</th>
            <th>Amount</th>
            <th>Status</th>
            <th>Comments</th>
        </tr>
    </thead>
    <tbody>
        <tr class="odd">
            <td>Training materials</td>
            <td>Book/Course on specific technology</td>
            <td>1</td>
            <td>Allocated</td>
            <td>Book ordered</td>
        </tr>
        <tr class="even">
            <td>Development Workstations</td>
            <td>800MHz PC, 256MB RAM</td>
            <td>4</td>
            <td>Satisfied</td>
            <td>Dev group will use existing workstations</td>
        </tr>
        <tr class="odd">
            <td>Development DB Server</td>
            <td>Dual CPU 1GHz PC, 512MB RAM: SERVERNAME.company.com</td>
            <td>1</td>
            <td>Allocated</td>
            <td></td>
        </tr>
        <tr class="even">
            <td>Interactive Testing Workstations</td>
            <td>800MHz PC, 256MB RAM</td>
            <td>2</td>
            <td>Allocated</td>
            <td></td>
        </tr>
        <tr class="odd">
            <td>Load Test Server</td>
            <td>800MHz PC, 256MB RAM: SERVERNAME.company.com</td>
            <td>1</td>
            <td>Pending</td>
            <td></td>
        </tr>
        <tr class="even">
            <td>Load Test Clients</td>
            <td>500MHz PC or Mac, 128MB RAM</td>
            <td>4</td>
            <td>Satisfied</td>
            <td>QA group will use existing machines</td>
        </tr>
        <tr class="odd">
            <td>Automated Testing Slave</td>
            <td>800MHz PC, 256MB RAM: SERVERNAME.company.com</td>
            <td>1</td>
            <td>Satisfied</td>
            <td>QA group will use existing machine</td>
        </tr>
        <tr class="even">
            <td>Testing DB Server</td>
            <td>Dual CPU 1GHz PC, 512MB RAM: SERVERNAME.company.com</td>
            <td>1</td>
            <td>Rejected</td>
            <td>Testing group will use development DB server and do load testing in off hours</td>
        </tr>
        <tr class="odd">
            <td>IDE Licenses</td>
            <td>Standard development licenses</td>
            <td>N/A</td>
            <td>Satisfied</td>
            <td>Will use open source tools</td>
        </tr>
        <tr class="even">
            <td>SCM Licenses</td>
            <td>Standard development licenses</td>
            <td>N/A</td>
            <td>Satisfied</td>
            <td>Will use open source tools</td>
        </tr>
        <tr class="odd">
            <td>Testing Tool Licenses</td>
            <td>Standard development licenses</td>
            <td>N/A</td>
            <td>Satisfied</td>
            <td>Will use open source tools</td>
        </tr>
        <tr class="even">
            <td>DB Licenses</td>
            <td>Standard development licenses</td>
            <td>6</td>
            <td>Pending</td>
            <td></td>
        </tr>
        <tr class="odd">
            <td>DB Licenses</td>
            <td>Production licenses</td>
            <td>4 CPU's</td>
            <td>
                <div>
                    2 Pending
                </div>
                <div>
                    2 Rejected
                </div>
            </td>
            <td>Testing group will use development DB server and do load testing in off hours</td>
        </tr>
        <tr class="even">
            <td>Software component</td>
            <td>GIS Library w/ source code</td>
            <td>1</td>
            <td>Pending</td>
            <td>One time fee, approx. $10,000</td>
        </tr>
        <tr class="odd">
            <td>Software component</td>
            <td>Encryption library</td>
            <td>1</td>
            <td>Pending</td>
            <td>Revenue sharing at 2%</td>
        </tr>
    </tbody>
</table>

#### Possible Status Values {#possible-status-values}

-   Pending: request is awaiting management decision
-   Assigned: task has been assigned to a person in the issue tracker
-   Allocated: capital request approved by management, but resource has
    not arrived
-   Satisfied: request is satisfied, resource has arrived
-   Rejected: requested resource will not be allocated, plan must be
    adjusted to work without this resource

### Resource Needs Checklist {#resource-needs-checklist}

The goal of this checklist is to help expose resource needs that might
otherwise be missed. It does not help with the actual estimated number
of hours needed. Those estimates should be based on the project plan.

TODO: Answer the questions below. If multiple sample answers are
provided, [chip away](glossary-std#chipaway){.def} the ones that do
not apply. Edit any provided answers as needed. Use this exercise to
help you fill in the tables above.

Does this project need more than a few days work?
:   Yes. A project manager role is needed to oversee the project.
:   No. The developers can manage their own work.

Are the requirements already completely defined and validated?
:   Yes. No additional time is needed for requirements.
:   No. Effort is needed for requirements.

What aspects of the system need to be designed?
:   General design. Group developer effort needed.
:   User interface. UI designer and domain experts effort needed.
:   Database design. Developer and DBA effort needed.
:   Security design. Developer and topic expert effort needed.
:   Other design. Developer, domain, and/or topic expert effort needed.

Does the project plan include any new development?
:   Yes. Development resources are needed.
:   No. No developers are needed

Does the project plan include complex configuration of existing components?
:   Yes. Component expert needed. Also need time to coordinate with
    development and operations teams.
:   No. No component experts are needed

Does the development team have knowledge of all tools, components, and technologies to be used?
:   Yes. No training time needed.
:   No. Effort needed for training. Need training materials, courses, or
    time with experts or mentors. List specific training
    needs individually.

Is the entire development team have an agreed upon software development methodology?
:   Yes. No effort needed for defining a methodology.
:   Yes. But, effort is needed to refine the methodology to the project
    at hand.
:   No. Effort needed to define and document a methodology and train all
    team members. Additional effort needed for refinements throughout
    the project.

Does the project plan include end-user documentation?
:   Yes. Technical writing resources must be allocated.
:   No.

What is the complexity of the internal documentation?
:   Significant. Technical writing resources must be allocated.
:   Average. Developers can produce technical documents as they go.

Will the technical support, training, operations, or services groups deal with the product of this project?
:   Yes. Effort must be allocated to train the staff in those groups.
:   No, but other developers will need training to reuse this component.
:   No. Effort put into producing good technical documentation should
    be enough.

Will the product of this project be sold to customers, directly or indirectly?
:   Yes. The full SDM must be followed, including effort by a change
    control board and release engineering.
:   No, it is for internal use only but it will be used repeatedly to
    help build a shipping product. Release engineering and CCB effort is
    still needed.
:   No, it is for internal use only and will only be used once. Release
    engineering and CCB effort not needed.

Does the QA plan call for the running of automated unit tests?
:   Yes. Development effort will be needed to implement unit tests.
:   No. Additional QA effort will be needed for manual testing.

Does the QA plan call for more than the running of automated unit tests?
:   Yes. QA effort will be needed.
:   No. Unit tests will be enough for this component, full QA can be
    done on products that use this component.

How many development workstations will be needed?
:   1 per developer.
:   1 per developer, plus extra for...

What development servers are needed?
:   None.
:   One for the whole team.
:   One for the one aspect of development, another for another aspect.
:   One for the one branch of development, another for another branch.

What database servers are needed?
:   None. No database is being used.
:   None. Database is integrated into product and does not require a
    separate server.
:   One for the whole team.
:   One for the developers, one for QA.
:   One for one branch of development, another for another branch.
:   One for the developers, one for QA, one for load testing.
:   One for each developer or tester, plus one for load testing.

What machines are needed for automated testing?
:   None. Automated testing will not be done.
:   None. Automated testing will be done on workstations.
:   One for all nightly automated tests.
:   One for one aspect of nightly automated tests, another for
    another aspect.
:   One for one branch of development, another for another branch.

What machines are needed for load testing?
:   None. Load testing will not be done.
:   None. Load testing will be done on workstations.
:   One machine will do all load testing.
:   Several machines needed to act as clients and servers.
:   One cluster of load testing machines for each branch of development.

What development tools must be licensed for this project?
:   None. Everything is implemented by us.
:   None. All development tools are open source.
:   Some tools: IDE, database, testing tools. These tools have already
    been purchased, installed, and configured.
:   Some tools: IDE, database, testing tools. Budget must be allocated
    to purchase these tools. Effort must be allocated to research and
    select tools for purchase, install, and configure them.

What software components must be licensed for this project?
:   None. Everything is implemented by us.
:   None. All reused components are open source.
:   Some components: database, server software, libraries. These
    components have already been selected, purchased, installed,
    and configured.
:   Some components: database, server software, libraries. Effort must
    be allocated to research, select, install and configure
    these components. Budget must be allocated to purchase them.

Are any of the personnel assignments of capital allocations conditional?
:   Yes. All such conditions are written in the comments column above.
    We have a contingency plan that will still achieve (an
    acceptable subset) of the project goals.
:   No. Management has set aside these resources as promised, and the
    needs of this project will take priority over any other project that
    is likely to need the same resources.

Have these resource assignments been communicated to the people being assigned and their managers?
:   Yes, everyone understands. Feedback is welcome.
:   No, this is a risk that is noted in the [Risk
    Management](plan#risks) section.

TODO: Check for [words of
wisdom](http://readyset.tigris.org/words-of-wisdom/resource-needs.html)
and discuss ways to improve this template. Or, evaluate the ReadySET Pro
[professional resource needs
template](http://www.readysetpro.com/ "pro use case template and sample test plan").

Company Proprietary

Copyright © 2003-2004 Jason Robbins. All rights reserved. [License
terms](readyset-license.html). Retain this copyright statement whenever
this file is used as a template.


