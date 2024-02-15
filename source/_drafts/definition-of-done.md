---
title: Definition of Done
tags:
- Code quality
- Reviews
- Best practices
categories:
- Software development
---

Introduction

<!-- more -->

## Acceptance criteria are met

- With the required code coverage (as defined for the project)
- 100% of tests pass (no skipped tests, unless very well justified)
- Tests are of the types defined by the team: unit, integration, end to end…

## Code quality is kept

- The new code keeps the quality gates established (automate everything when possible in a CI)
- Linters
- Static code analyzers
- Pull requests
- Code validation with teammates

## The user story is validated inside the development team

- Someone in the development team has validated it:
  - functional: in the deployed environment
  - code: it could be with the PR
- The conversation during validation is important: edge cases may appear and knowledge transfer is important

## The user story is validated by the customer

- Sometimes, it is better to validate a user story without waiting for the sprint review

## Everything is deployed

- It is deployed to an environment similar (if not equal) to the production one
- Deployment should be automated (CD)
- This environment is where the validation will take place
- It could be also used to show the story to the customer

## All feedback has been processed

- This does not mean that all feedback needs to be implemented
- Some feedback may be moved to technical debt (with a real justification)
- Lack of agreement between the reviewer and the author should be solved (when there is a complete tie, a third person may help)

## It has the required documentation

- Documentation should not be left for the end of the project
- Each user story should update the documentation with the information needed:
  - if new passwords and keys are needed, the credential manager should be updated
  - if new developers need to install something on their laptops for run the project, the `REAMD.md` file should be updated
  - if the customer’s user guide needs more information, add it
- Try to avoid typos, grammar errors…
- Review documentation in the story validation

## Conclusion

This is the checklist for your next user story:

- [ ]  All goals in a user story are met
- [ ]  The new functionality has tests (and are green)
- [ ]  Code quality is kept
- [ ]  The user story is validated inside the development team
- [ ]  The user story is validated by the customer
- [ ]  Everything is deployed
- [ ]  All feedback has been processed
- [ ]  It has the required documentation