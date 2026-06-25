# IT Fundamentals

## Incident

Any type of issues faced by the users related to the system that prevents them to access or run any functionality can be an incident.

Example: Users cannot log in.

## Problem

The cause or the root cause behind one or more incidents.

Example: The login server keeps crashing because of a datatbase issue.

## Change

A planned modification to a system, service, configuration, or process. It may fix a problem, add a feature, improve security, or update existing functionality.

Example: - upgrading software version - adding MFA - changing database permissions - updating a workflow

## Enhancement

Improving something that already works for efficiency or user experience.

Example: Making the login page easier to use.

## Example scenario

A user says:

"The employee portal is showing an error and I can't submit my vacation request."

- Qustions
  - Is this an Incident, Problem, Change, or Enhancement?
    - It is an incident

  - What questions would you ask the user?
    - When did the issue start?
    - Is it happening every time or only sometimes?
    - What steps did you take before the error appeared?
    - Are other users having the same issue?
    - Which browser/device are you using?
    - Can you send a screenshot of the error?
    - Were you able to submit vacation requests before?

  - Who might you contact if you cannot solve it?
    - Senior Application Support Analyst
    - System Administrator
    - Developer
    - Database Administrator
    - Network/Infrastructure team
    - HR/business process owner, if the vacation system belongs to HR

  - What information would you document?

    Incident date, time, user info, coversation with the user, Error message, steps already taken to resolve the issue and the statusof the ticket.

## Simple System Flow

    User
     ↓
    Browser
     ↓
    Website (Frontend)
     ↓
    API
     ↓
    Backend Application
     ↓
    Database

- Question
  - Which of these layers might be the issue?
    The issue could be at any layer. I would first collect the error message and steps to reproduce, then check whether it affects only one user or many users. If it affects many users, it is more likely a system/backend/API/database issue. If it affects one user, it may be account, browser, permission, or user-specific data.

## Improved Support Analysis

This is an incident because the user is unable to complete a normal business function.

Questions to ask:

- What exact error message do you see?
- When did the issue start?
- Does it happen every time?
- What steps did you take before the error appeared?
- Are other users having the same issue?
- Which browser/device are you using?
- Can you provide a screenshot?
- Were you able to submit vacation requests before?

Possible escalation:

- Senior Application Support Analyst
- System Administrator
- Developer
- Database Administrator
- HR/business process owner

Information to document:

- Date and time
- User name/department/contact
- System/application name
- Error message/screenshot
- Steps to reproduce
- Impact and urgency
- Troubleshooting steps taken
- Escalation notes
- Current ticket status

Possible issue layers:

- User/account permissions
- Browser/cache/session
- Frontend page issue
- API failure
- Backend application error
- Database/data issue

## Application Support Analyst - What They Do

An Application Support Analyst helps users and business teams when software systems are not working correctly or when support is needed. They investigate issues, collect information, reproduce errors, check possible causes, escalate when needed, test fixes, and document solutions.

Common tasks:

- Monitor ticket queue
- Respond to user issues
- Ask clarifying questions
- Reproduce errors
- Check logs, screenshots, and user steps
- Escalate to technical teams when needed
- Update ticket notes
- Test fixes
- Write documentation
- Support system changes or enhancements
