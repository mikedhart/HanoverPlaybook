<!-- ---
title: Ticket Flow
section: guides
layout: page
---
Ticket Flow
============
1. Receive ticket. Make sure it has an acceptance criteria that is clearly marked "Acceptance Criteria". If it does not, assign to the project lead and request one.
2. Read and understand ticket. Ask any questions by assigning the ticket to the relevant person. Repeat this until you have clear knowledge of what you're trying to achieve
3. Do work
	- Checkout a new feature branch from the current working branch. The branch should be called the same as the ticket ID
	- Do work
	- Test your own work against acceptance criteria. Repeat step 3.2 and 3.3 until acceptance criteria passes
4. Publish your work
	- Push your branch to Github
	- Submit pull request
	- Resolve the ticket as "pending code review" and assign to a code reviewer
5. Code review
	- Review code using the code review guide. Any necessary discussion will take place on the the pull request screen
	- Code reviewer will make any minor changes required. If major change is required, the ticket should be reactivated and assigned back to original person with a description in the ticket, at which point the process reverts to step 3
6. Merge
	- Code reviewer will merge into working code base and deploy to dev/beta/live
	- Ticket is resolved as "pending live testing" and assigned to another developer with instructions of which environment in which to test
7. Live test
	- Tester carries out test on dev/beta/live and either
		- Goes to step 8
		- Reactivates ticket and assigns to the original developer. At which point, the process reverts to step 4
	- It is the tester's responsibility for the ticket to pass the acceptance criteria
8. Closing the ticket
	- Tester resolves the ticket to the project primary contact as "live test passed"
	- Project lead closes ticket and notifies client -->
