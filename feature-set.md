[SRS](srs) &gt; Feature Set {#srs-feature-set}
--------------------------------

### Release Information {#release-information}

Project:
:   PROJECTNAME

Internal Release Number:
:   X.Y.Z

Related Documents:
:   [Project proposal](proposal) > [User needs](user-needs)
:   [SRS](srs) > [Use case suite](use-case-suite)
:   [Feature format](feature-format)
:   LINK TO USE CASE DIAGRAM
:   LINKS TO RELEVANT STANDARDS
:   LINKS TO OTHER DOCUMENTS

**Process impact:** A feature set is simply a table of contents for the
individual feature descriptions. Much like a test suite, organizing the
feature set by priority, functional area, actor, business object, or
release can help identify missing, extra, or poorly motivated features
early.

TODO: Before writing individual feature descriptions, list all the
features that you think you will need. Organize them so that missing
features appear as blanks on this page, and extra features will appear
to be extras that don't fit anywhere. See the [feature
format](feature-format#checklist) document for more tips on
specifying features and feature sets.

TIP: Refer back to the user stories in your [user
needs](user-needs) document and to the [use case
suite](use-case-suite). Use them for ideas and make sure that you
cover all of them.

### Features by Release and Priority {#features-by-release-and-priority}

TODO: Select subset of features can be implemented for a given release.
When features are listed in priority order, choosing the features to
implement in a release simply becomes a matter of "drawing a line":
features below the line must wait for a later release. Make sure to also
consider estimated effort and risk.

-   Release 1.0
    -   Essential
        -   [F-00](features#F-00) Site configuration
        -   [F-01](features#F-01) User registration
        -   [F-21](features#F-21) NAME OF FEATURE
        -   [F-31](features#F-31) NAME OF FEATURE
    -   Expected
        -   [F-02](features#F-02) NAME OF FEATURE
        -   [F-03](features#F-03) NAME OF FEATURE
        -   [F-20](features#F-20) NAME OF FEATURE
-   Release 1.1
    -   Expected
        -   [F-22](features#F-22) NAME OF FEATURE
        -   [F-23](features#F-23) NAME OF FEATURE
        -   [F-33](features#F-33) NAME OF FEATURE
    -   Desired
        -   [F-10](features#F-10) NAME OF FEATURE
        -   [F-11](features#F-11) NAME OF FEATURE
        -   [F-12](features#F-12) NAME OF FEATURE
-   Later Releases
    -   Optional
        -   [F-30](features#F-30) NAME OF FEATURE
        -   [F-32](features#F-32) NAME OF FEATURE

### Features by Release and Risk {#features-by-release-and-risk}

-   Release 1.0
    -   [F-00](features#F-00) Safe : Site configuration
    -   [F-01](features#F-01) Safe : User registration
    -   [F-21](features#F-21) Safe : NAME OF FEATURE
    -   [F-31](features#F-31) 1-Risk : NAME OF FEATURE
    -   [F-02](features#F-02) 1-Risk : NAME OF FEATURE
    -   [F-03](features#F-03) 2-Risks : NAME OF FEATURE
    -   [F-20](features#F-20) 2-Risks : NAME OF FEATURE
    -   Total unique risk factors: 4
-   Release 1.1
    -   [F-22](features#F-22) Safe : NAME OF FEATURE
    -   [F-23](features#F-23) Safe : NAME OF FEATURE
    -   [F-33](features#F-33) Safe : NAME OF FEATURE
    -   [F-10](features#F-10) 2-Risks : NAME OF FEATURE
    -   [F-11](features#F-11) 2-Risks : NAME OF FEATURE
    -   [F-12](features#F-12) 3-Risks : NAME OF FEATURE
    -   Total unique risk factors: 5
-   Later Releases
    -   [F-30](features#F-30) Safe : NAME OF FEATURE
    -   [F-32](features#F-32) 2-Risks : NAME OF FEATURE
    -   Total unique risk factors: 2

### Features by Functional Area {#features-by-functional-area}

-   FUNCTIONAL AREA ONE
    -   [F-00](features#F-00) Site configuration
    -   [F-01](features#F-01) User registration
    -   [F-02](features#F-02) NAME OF FEATURE
    -   [F-03](features#F-03) NAME OF FEATURE
-   FUNCTIONAL AREA TWO
    -   [F-10](features#F-10) NAME OF FEATURE
    -   [F-11](features#F-11) NAME OF FEATURE
    -   [F-12](features#F-12) NAME OF FEATURE
    -   [F-13](features#F-13) NAME OF FEATURE
-   FUNCTIONAL AREA THREE
    -   [F-20](features#F-20) NAME OF FEATURE
    -   [F-21](features#F-21) NAME OF FEATURE
    -   [F-22](features#F-22) NAME OF FEATURE
    -   [F-23](features#F-23) NAME OF FEATURE
-   FUNCTIONAL AREA FOUR
    -   N/A: These features are completely automated and internal, users
        never interact with them
-   FUNCTIONAL AREA FIVE
    -   TODO: need to write use cases here
-   Other functional areas
    -   [F-30](features#F-30) NAME OF FEATURE
    -   [F-31](features#F-31) NAME OF FEATURE
    -   [F-32](features#F-32) NAME OF FEATURE
    -   [F-33](features#F-33) NAME OF FEATURE

TODO: Check for [words of
wisdom](http://readyset.tigris.org/words-of-wisdom/feature-set.html) and
discuss ways to improve this template. Or, evaluate the ReadySET Pro
[professional feature set
template](http://www.readysetpro.com/ "pro use case template and sample test plan").

Company Proprietary

Copyright © 2003-2004 Jason Robbins. All rights reserved. [License
terms](readyset-license.html). Retain this copyright statement whenever
this file is used as a template.


