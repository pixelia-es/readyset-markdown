[SRS](srs) &gt; [Use Case Suite](use-case-suite) &gt; Use Cases {#srs-use-case-suite-use-cases}
-------------------------------------------------------------------------

### Release Information {#release-information}

Project:                      
:	PROJECTNAME

Internal Release Number:      
:	X.Y.Z

Related Documents:            
:	[Project proposal](proposal) > [User needs](user-needs), [SRS](srs) > [Feature set](feature-set)
:	[Use case format](use-case-format)
:	LINK TO USE CASE DIAGRAM
:	LINKS TO RELEVANT STANDARDS
:	LINKS TO OTHER DOCUMENTS

TODO: Note any aspects that are common to all use cases here. This helps
keep the use cases themselves short. If any use case is an exception,
note it's specific value to replace or add to the default.

### Default Aspects of All Use Cases {#default-aspects-of-all-use-cases}

Direct Actors:
:	User: end-user in any role
:	System: The system being built
:	When actors are not listed, assume User is doing it.
:	Items beginning with "see" indicate that System has presented a new screen.

Stakeholders:
:	Project Owners and other members

Prereq:
:	User is logged in

TODO: For each use case listed in the [use case
suite](use-case-suite), create an HTML anchor and heading with it's
unique ID, then fill in the rows of the table to specify the use case in
detail.

TIP: It is OK to simply list the names of a lot of use cases without
actually writing the use case in detail. Document the most important use
cases first and come back to less important ones later.

TIP: See detailed tips in the [guidelines for writing use
cases](use-case-format#guidelines).

### UC-00: Configure the site {#UC-00-configure-the-site}

Summary:
:   The administrator navigates to the site configuration page and uses it to change the behavior of the web application. Specifically, the user-visible timezone is being set.

Priority:
:   Essential

Use Frequency:
:   Rarely

Direct Actors:
:   Admin: Web-site administrator

Main Success Scenario:

:   1. visit SiteConfiguration page
	2. see site configuration options
	3. enter timezone abbreviation for date displays
	4. submit form
	5. confirm changes
	6. see SiteConfiguration page again, with updated values


Alternative Scenario Extensions:
    
:   - If the timezone abbreviation is incorrect, an error message will be displayed and no changes will be made.
    
Notes and Questions
 
:   - How will administrators know the right timezone abbreviation? They would know it if they live in that timezone. Maybe we could provide a drop-down list of all choices, but each would need some explanation.

### UC-01: Register as a new user {#UC-01-register-as-a-new-user}

Summary:
:   Users need to register themselves in this web application.

Priority:
:   Essential

Use Frequency:
:   Once per user

Main Success Scenario:
:

:   1. visit Login page
	2. click to register as new user
	3. enter identifying information: username, email, real name, password (twice)
	4. submit form
	5. check email
	6. reply to confirmation message
	7. log in

Alternative Scenario Extensions:

:   - If the username is taken, then the system will suggest an available username based on the user's email address and/or real name.
    
Notes and Questions
 
:   - NOTE
    - QUESTION

### UC-02: Request new password {#UC-02}

Summary:
:   If a user forgets their password, they can request a new one be emailed to them.

Priority:
:   Expected

Use Frequency:
:   Rarely

Main Success Scenario:

:    - TODO

Notes and Questions

 
:    - Alternatively, we could use password hints.

### UC-03: Edit user profile {#UC-03}



Summary:
:   Users can edit their own account preferences.

Priority:
:   Expected

Use Frequency:
:   Rarely



Main Success Scenario:

:    - TODO


### UC-04: View user profile {#UC-04}

Summary:
:   Users can view the profiles of other users under certain circumstances.

Priority:
:	Expected

Use Frequency:
:	Rarely

Direct Actors:
:   Admin: Web-site administrator

Main Success Scenario:


:   - TODO

### UC-10: Create course {#UC-10}

Summary:
:   An administrator creates dozens of course offerings before the beginning of each school term.

Priority:
:   Essential

Use Frequency:
:   Often

Direct Actors:
:   Admin: Web-site adminisator

Main Success Scenario:

:   - visit administrative function menu
	- click add course
	- enter course information: name, number, instructor, capacity
	- submit form
	- see course list with new course added

### UC-11: View catalog description {#UC-11}

Summary:
:   Students may view the course catalog description of a course before registering. They are especially likely to view it if they are prevented from enrolling in a course because of a missing prerequisite.

Priority:
:   Essential

Use Frequency:
:   Sometimes

Main Success Scenario:

:   - visit one of several in application pages that deal with courses
	- click link to course description
	- see course description in pop-up window
	- close pop-up window to continue using application
    


Notes and Questions
 
:   - How do we accommodate users that configure their browsers to block pop-ups?
    
### UC-20: Enroll in course {#UC-20}

Summary:
:   Students will enroll in courses

Priority:
:   Essential

Use Frequency:
:   Often

Main Success Scenario:

:   - visit main menu
	- click link to enroll in courses
	- enter major and course number
	- select course section from list of available sections
	- submit choice
	- confirm choice
	- see list of current enrolled courses

Alternative Scenario Extensions:

:   - If a course is full, then the student may join the wait-list.
		- Course capacity and number of students currently waiting should be shown so that students may choose the section that they are most likely to be able to get into.

### UC-21: Drop a course {#UC-21}

Summary:
:   A student may drop a course that they are enrolled in.

Priority:
:   Essential

Use Frequency:
:   Sometimes

Main Success Scenario:

:   - visit list of currently enrolled courses
	- select course from list
	- click button to drop course
	- see warning that they may not be able to add this course again
	- confirm choice
	- see revised list of currently enrolled courses

Notes and Questions
 
:   - Only one course can be dropped at a time. There is no need to allow students to quickly drop more than one course.
	- It would be nice to offer an atomic "switch sections" operation that drops and adds another, or does nothing.

### UC-30: View room description {#UC-30}

Summary:
:   Users can view descriptions of classrooms. E.g., is it a lecture hall or a lab? E.g., does it have a built-in LCD projector?

Priority:
:   Optional

Use Frequency:
:   Rarely

Main Success Scenario:

:   - TODO

### UC-31: Assign course to room {#UC-31}

Summary:
:   An administrator assigns each course to a room. This is often done after a course is created, but it can be redone at any time.

Priority:
:   Essential

Use Frequency:
:   Often

Main Success Scenario:

:   - STEP
    - STEP
    - STEP

### UC-40: USE CASE NAME {#UC-40}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
    - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-41: USE CASE NAME {#UC-41}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:
    
:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
    - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-42: USE CASE NAME {#UC-42}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
    - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-50: USE CASE NAME {#UC-50}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
    - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-51: USE CASE NAME {#UC-51}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
    - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-52: USE CASE NAME {#UC-52}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-60: USE CASE NAME {#UC-60}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-61: USE CASE NAME {#UC-61}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-62: USE CASE NAME {#UC-62}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-70: USE CASE NAME {#UC-70}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-71: USE CASE NAME {#UC-71}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-72: USE CASE NAME {#UC-72}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-80: USE CASE NAME {#UC-80}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-81: USE CASE NAME {#UC-81}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-82: USE CASE NAME {#UC-82}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION
    
### UC-90: USE CASE NAME {#UC-90}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

### UC-91: USE CASE NAME {#UC-91}

Summary:
:   1-3 SENTENCES

Priority:
:   Essential | Expected | Desired | Optional

Use Frequency:
:   Always | Often | Sometimes | Rarely | Once

Direct Actors:
:   ACTOR1, ACTOR2, ACTOR3

Stakeholders:
:   STAKEHOLDER, STAKEHOLDER, STAKEHOLDER

Prereq:
:   PRECONDITION
:   PRECONDITION
:   PRECONDITION

Main Success Scenario:

:   - STEP
    - STEP
    - STEP


Alternative Scenario Extensions:

:   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.
   - If CONDITION, then ALTERNATIVE STEPS.
        - NOTES or DETAILS.

Notes and Questions
 
:   - NOTE
    - NOTE
    - QUESTION
    - QUESTION

TODO: Check for [words of wisdom](http://readyset.tigris.org/words-of-wisdom/use-cases.html) and
discuss ways to improve this template. Or, evaluate the ReadySET Pro
[professional use case template](http://www.readysetpro.com/).

Company Proprietary

Copyright © 2003-2004 Jason Robbins. All rights reserved. [License terms](readyset-license.html). Retain this copyright statement whenever this file is used as a template.


